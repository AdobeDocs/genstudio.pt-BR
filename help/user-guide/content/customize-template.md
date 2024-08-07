---
title: Personalizar modelos
description: Saiba como criar um modelo personalizado para o GenStudio.
level: Intermediate
feature: Templates, Content
source-git-commit: 423956d6fdbf5b31041d44eb434f90d55a87d7c0
workflow-type: tm+mt
source-wordcount: '784'
ht-degree: 0%

---


# Personalizar modelos

Você pode adaptar seus modelos de HTML para o GenStudio usando a linguagem de modelo _Handlebars_. A sintaxe Handlebars usa texto regular com chaves duplas como espaços reservados para o conteúdo. Consulte [`What is Handlebars?`](https://handlebarsjs.com/guide/#what-is-handlebars) no _Guia de linguagem do Handlebars_ para saber como preparar seu modelo.

## Estrutura do modelo

<!-- This is for email. In the future, maybe use tabs to provide guidance for other template types.
-->

Se você não tiver um modelo de HTML pronto para uso no GenStudio, poderá começar definindo a estrutura do email usando as tags de HTML: `DOCTYPE`, `html`, `head` e `body`. É possível incluir estilos CSS para personalizar a aparência do email.

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

>[!TIP]
>
>Nas próximas seções, adicione espaços reservados para o conteúdo de campos de email, oculte elementos desnecessários da pré-visualização e gerencie links para conteúdo estático. Quando o modelo estiver pronto, você poderá [carregá-lo no GenStudio](use-templates.md#upload-a-template) e começar a gerar emails personalizados com base no modelo personalizado.

## Espaços reservados de conteúdo

No cabeçalho ou no corpo do modelo, é possível usar a sintaxe Handlebars para inserir espaços reservados de conteúdo, nos quais é necessário que o GenStudio preencha o email com o conteúdo real. O GenStudio reconhece e interpreta automaticamente os espaços reservados de conteúdo com base no nome do campo.

Por exemplo, você pode usar `{{ headline }}` para indicar onde o título do email deve ser colocado:

```handlebars
<div>{{ headline }}</div>
```

O número máximo de campos permitidos em um modelo personalizado é vinte.

**Nomes de campos reconhecidos**:

| Texto | Função | Modelo de canal |
| -------------- | ---------------------- | -------------------- |
| `pre_header` | Pré-cabeçalho | email |
| `headline` | Título | email<br>anúncio social |
| `body` | Corpo do texto | email<br>anúncio social |
| `cta` | Chamada para ação | email<br>anúncio social |
| `on_image_text` | No texto da imagem | anúncio social |
| `image` | Imagem | email<br>anúncio social |
| `brand_logo` | Logotipo da marca selecionada | anúncio social |

>[!IMPORTANT]
>
>O GenStudio fornece automaticamente ao modelo de email um campo `subject` durante o processo [!DNL Create], de modo que não é necessário incluir o campo de assunto em seu modelo de email.

+++Exemplo: modelo básico

Este é um exemplo básico de um template de HTML para email. O cabeçalho contém CSS simples e em linha para estilo. O corpo contém um espaço reservado de `pre-header`, `headline` e `image` para uso do GenStudio para inserir conteúdo durante o processo de geração de email.

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

### Imagem de fundo

Ao criar um anúncio para Meta, é importante usar uma imagem de fundo complementada por texto e uma sobreposição de logotipo de marca. Para garantir o dimensionamento adequado da imagem, os modelos de Metadados exigem a especificação de um `aspect ratio`. Nesse contexto, você pode fornecer apenas um campo de imagem.

## Seções ou grupos

_As seções_ fornecem uma maneira de informar ao GenStudio que os campos pertencentes a uma seção exigem um alto grau de coerência. O estabelecimento dessa relação ajuda a IA a gerar conteúdo que corresponde aos elementos criativos na seção. Um modelo pode incluir até três seções.

Use um prefixo de sua escolha no nome do campo para indicar que este campo faz parte de uma seção ou grupo. Por exemplo, talvez você queira destacar o conteúdo que aparece em uma área realçada. Você pode optar por identificar o conteúdo dessa área com um prefixo comum:

- `spotlight_headline`
- `spotlight_body`

Cada seção pode ter apenas uma de um tipo de campo. Por exemplo, o grupo de exemplos acima com o prefixo `spotlight` só pode ter um campo `spotlight_headline`.

Quando você tiver várias seções (no máximo três):

- `headline`
- `body`
- `spotlight_headline`
- `spotlight_body`
- `news_headline`
- `news_body`

A GenStudio entende que `spotlight_headline` está mais intimamente relacionado a `spotlight_body` do que a `news_body`.

+++Exemplo: modelo com várias seções

O modelo a seguir é o mesmo modelo de HTML no exemplo acima, mas com mais duas seções. O cabeçalho contém CSS em linha para estilizar um pod. O corpo usa dois pods com espaços reservados de conteúdo usando um prefixo.

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

## Visualização do modelo

Os templates de email às vezes contêm conteúdo especial que não é necessário visualizar no GenStudio. Você pode controlar a visibilidade desse conteúdo usando os Auxiliares integrados, que são expressões especiais na linguagem de modelo Handlebars que ajudam a executar determinadas ações.

O valor `_genStudio.browser` é definido ao renderizar um modelo, e o valor `genStudio.export` é definido ao exportar um modelo. Você pode decidir incluir determinado conteúdo na parte superior dos emails usando um invólucro condicional, por exemplo, quando o modelo for usado para exportação:

```handlebars
{{#if _genStudio.export}}
<%@ include view='emailParent' %>
{{/if}}
```

Outro exemplo pode ser impedir o uso de códigos de rastreamento ao visualizar um modelo de email no GenStudio. Este exemplo mostra como adicionar parâmetros de rastreamento a links no modelo exportado, mantendo os links de visualização limpos:

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
