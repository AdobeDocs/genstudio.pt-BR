---
title: Personalizar modelos
description: Saiba como criar um modelo personalizado para o GenStudio.
level: Intermediate
feature: Templates, Content
source-git-commit: c9cf7da078e84cf7696f32ca2278aa71b7b1b7cc
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 0%

---


# Personalizar modelos

Adapte seus modelos de HTML para o GenStudio usando a linguagem de modelo _Handlebars_. A sintaxe Handlebars usa texto regular com chaves duplas como espaços reservados para o conteúdo. Consulte [`What is Handlebars?`](https://handlebarsjs.com/guide/#what-is-handlebars) no _Guia de linguagem do Handlebars_ para saber como preparar seu modelo.

<!-- This is for email. In the future, maybe use tabs to provide guidance for other template types.
-->If you do not have an HTML template ready to use in GenStudio, you can start by defining the structure of your email using HTML tags: `DOCTYPE`, `html`, `head`, and `body`. You can include CSS styles to customize the appearance of your email.

```html
<!DOCTYPE html>
<html>
<head>
    <title>Title</title>
    <style>
    </style>
</head>
<body>
</body>
</html>
```

Consulte [Exemplos de modelo](#template-examples).

>[!TIP]
>
>Nas próximas seções, adicione espaços reservados para o conteúdo de campos de email. Consulte exemplos de modelos, oculte elementos desnecessários da pré-visualização e gerencie links para conteúdo estático. Quando o modelo estiver pronto, você poderá [carregá-lo no GenStudio](use-templates.md#upload-a-template) e começar a gerar emails personalizados com base no modelo personalizado.

## Espaços reservados de conteúdo

Dentro do cabeçalho ou do corpo de um modelo, você pode usar a sintaxe Handlebars para inserir espaços reservados de conteúdo, nos quais é necessário que o GenStudio preencha o modelo com conteúdo real. O GenStudio reconhece e interpreta automaticamente os espaços reservados de conteúdo com base no nome do campo.

Por exemplo, você pode usar `{{ headline }}` para indicar onde o título do email deve ser colocado:

```handlebars
<div>{{ headline }}</div>
```

### Nomes de campos

O número máximo de campos permitidos em um modelo personalizado é vinte.

#### Nomes de campo reconhecidos

A tabela a seguir lista os nomes de campo reconhecidos pelo GenStudio para preenchimento em modelos.

| Texto | Função | Modelo de canal |
| -------------- | ---------------------- | -------------------- |
| `pre_header` | Pré-cabeçalho | email (recomendado) |
| `headline` | Título | email (recomendado)<br>Meta-anúncio |
| `body` | Corpo do texto | email (recomendado)<br>Meta-anúncio |
| `cta` | Chamada para ação | email (recomendado)<br>Meta-anúncio |
| `on_image_text` | No texto da imagem | Meta-anúncio (recomendado) |
| `image` | Imagem | email (recomendado)<br>Meta-anúncio (recomendado) |
| `brand_logo` | Logotipo da marca selecionada | email<br>Meta-anúncio |

O GenStudio preenche automaticamente determinados campos em modelos, portanto, não é necessário incluí-los em seus designs de modelo:

* Campo `subject` (modelo de email)
* Campos `headline`, `body` e `CTA` (Modelo de metadados)

>[!WARNING]
>
>Para anúncios do Instagram, o título gerado não aparece na experiência final.

#### Nome do campo de logotipo da marca

Para adicionar um logotipo de marca no modelo, use um dos métodos a seguir para renderizar o logotipo padrão.

_Exemplo_:

```bash
<img src="{{#if brand_logo}}{{brand_logo}}{{else}}<default image>{{/if}}" alt="WKND" style="max-width: 88px; margin: 10px auto; display: block;"> 
```

_Exemplo_:

```bash
{{#if brand_logo}}

                    <img src="{{brand_logo}}" alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">

                {{else}}

                    <img src="data:image/png;base64,iVBORw0KGgo..." alt="img alt text" style="width: 120px; height: 45px; margin: 10px auto; display: block;">

                {{/if}}
```

#### Nomes de campo manuais

Todos os outros nomes de campo são tratados como campos preenchidos manualmente. Se quiser que uma seção seja editável, adicione colchetes duplos ao redor da seção que deseja editar.

_Exemplo_: ``{{customVariable}}`` (`customVariable` é a seção editável manualmente)

## Seções ou grupos

_As seções_ informam à GenStudio que os campos desta seção exigem um alto grau de coerência. O estabelecimento dessa relação ajuda a IA a gerar conteúdo que corresponde aos elementos criativos na seção.

Use um prefixo de sua escolha no nome do campo para indicar que um campo faz parte de uma seção ou grupo.

Por exemplo, talvez você queira destacar o conteúdo que aparece em uma área destacada:

* `spotlight_headline`
* `spotlight_body`

Cada seção pode ter apenas uma de cada tipo de campo. No exemplo acima, o prefixo `spotlight` só pode ter um campo `spotlight_headline`.

Um modelo pode incluir até três seções:

* `headline`
* `body`
* `spotlight_headline`
* `spotlight_body`
* `news_headline`
* `news_body`

A GenStudio entende que `spotlight_headline` está mais intimamente relacionado a `spotlight_body` do que a `news_body`.

## Exemplos de modelo

+++Exemplo: modelo de email com uma seção

Este é um exemplo básico de um modelo de HTML para um email que contém uma seção. O cabeçalho contém CSS simples e em linha para estilo. O corpo contém um `pre-header`, `headline`, e `image` [espaço reservado](#content-placeholders) para uso do GenStudio para inserir conteúdo durante o processo de geração de email.

```handlebars {line-numbers="true" highlight="13"}
<!DOCTYPE html>
<html>
<head>
    <title>Adobe</title>
    <style>
        .container {
            width: 100%;
            padding: 20px;
            font-family: Arial, sans-serif;
        }
    </style>
</head>
<body>{{ pre_header }}
    <div class="container">
        <h1>{{ headline }}</h1>
        <p><img alt="{{ headline }}"
                src="{{ image }}"
                width="600" height="600"
                border="0"/></p>
        <p>{{ body }}</p>
    </div>
</body>
</html>
```

+++

+++Exemplo: modelo de email com várias seções

O modelo a seguir é o mesmo modelo de HTML no exemplo acima, mas com mais duas seções. O cabeçalho contém CSS em linha para estilizar um grupo. O corpo usa dois grupos com [espaços reservados para o conteúdo](#content-placeholders) usando um prefixo.

```handlebars {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
<head>
    <title>Adobe</title>
    <style>
        .container {
            width: 100%;
            padding: 20px;
            font-family: Arial, sans-serif;
        }
        .pod {
            background-color: #f8f8f8;
            margin: 10px;
            padding: 20px;
            border-radius: 5px;
        }
        .pod h2 {
            color: #333;
        }
        .pod p {
            color: #666;
        }
    </style>
</head>
<body>{{ pre_header }}
    <div class="container">
        <h1>{{ headline }}</h1>
        <p><img alt="{{ headline }}"
                src="{{ image }}"
                width="600" height="600"
                border="0"/></p>
        <p>{{ body }}</p>
        <div class="pod">
            <h2>{{ pod1_headline }}</h2>
            <p>This is Pod 1 content.</p>
        </div>
        <div class="pod">
            <h2>{{ pod2_headline }}</h2>
            <p>This is Pod 2 content.</p>
        </div>
    </div>
</body>
</html>
```

+++

+++Exemplo: modelo de metadados

Este é um exemplo básico de um modelo de Meta-anúncio. O cabeçalho contém CSS em linha para estilo. O corpo usa [espaços reservados para o conteúdo](#content-placeholders) usando um prefixo.

```handlebars {line-numbers="true" highlight="33"}
<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Adobe</title>
    <style>
        .ad-container {
            width: 300px;
            border: 1px solid #ddd;
            padding: 16px;
            font-family: Arial, sans-serif;
        }
        .ad-image {
            width: 100%;
            height: auto;
        }
        .ad-headline {
            font-size: 18px;
            font-weight: bold;
            margin: 12px 0;
        }
        .ad-body {
            font-size: 14px;
            margin: 12px 0;
        }
        .ad-cta {
            display: inline-block;
            padding: 10px 20px;
            background-color: #007bff;
            color: #fff;
            text-decoration: none;
            border-radius: 4px;
            text-align: center;
        }
    </style>
</head>
<body>
<div class="ad-container">
    <img src="{{ image }}" alt="Ad Image" class="ad-image">
    <div class="ad-headline">"{{ headline }}"</div>
    <div class="ad-body">"{{ body }}"</div>
    <a href="(https://example.com)" class="ad-cta">"{{ CTA }}"</a>
</div>

</body>
</html>
```

+++

## Visualização do modelo

Controle a visibilidade de conteúdo especial usando Auxiliares incorporados (expressões especiais na linguagem de modelo Handlebars que executa determinadas ações). Por exemplo, é possível adicionar parâmetros de rastreamento a links no modelo exportado, mantendo os links de visualização limpos.

O valor `_genStudio.browser` é definido ao renderizar um modelo, e o valor `genStudio.export` é definido ao exportar um modelo. Você pode decidir incluir determinado conteúdo na parte superior de um email usando um invólucro condicional, por exemplo, quando o modelo for usado para exportação:

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

Outro exemplo pode ser impedir o uso de códigos de rastreamento ao visualizar um modelo no GenStudio. Este exemplo mostra como adicionar parâmetros de rastreamento a links no modelo exportado, mantendo os links de visualização limpos:

```handlebars
<a class="button" {{#if _genStudio.browser }}
   href="{{ link }}"{{/if}}{{#if _genStudio.export }}
   href="{{ link }}?trackingid=<%=getTrackingId()%>&mv=email"{{/if}}
   target="_blank">{{ cta }}</a>
```

## Conteúdo estático

Os modelos de email e meta geralmente vinculam a imagens e arquivos CSS hospedados fora do GenStudio. Quando o GenStudio gera miniaturas para esses modelos ou as experiências derivadas deles, ele pode ignorar esses recursos externos se eles não tiverem os cabeçalhos corretos do CORS (Cross-Origin Resource Sharing, Compartilhamento de recursos entre origens).

Para garantir que esses recursos estejam disponíveis durante o processo de geração de miniaturas, considere duas opções:

1. **Usar cabeçalhos CORS**: o servidor host deve enviar respostas com um cabeçalho `Access-Control-Allow-Origin` definido como valor `https://experience.adobe.com` para ambientes de produção. Esse método permite que o GenStudio acesse e inclua os recursos.
1. **Usar URLs de Dados**: Incorpore os recursos externos diretamente no modelo usando URLs de Dados. Esse método ignora as restrições do CORS e garante que os recursos estejam disponíveis durante a geração de miniaturas.
