---
title: Gravar prompts efetivos
description: Saiba como escrever prompts efetivos para o GenStudio.
feature: Prompt, Generative AI, Brands Service, Personas Service, Products Service, Guidelines
source-git-commit: 5e17996ee3a86cf664ee468d6b9cf178c8853992
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---


# Gravar prompts efetivos

A comunicação com a IA gerativa é essencial para trabalhar com eficiência no GenStudio.

O GenStudio fornece um prompt de IA generativo sempre que há uma oportunidade de modificar um ativo. Os componentes de um prompt efetivo devem incluir linguagem descritiva, exemplos e informações não fornecidas através das diretrizes configuradas.

Como prática recomendada, forneça à GenStudio as informações da sua marca usando as [diretrizes](/help/user-guide/guidelines/overview.md) e, em seguida, você poderá aproveitar totalmente a IA gerativa para produzir experiências de conteúdo alinhadas à marca.

## Linguagem descritiva

Você pode usar a linguagem natural para articular suas ideias e criar experiências. Seu prompt orienta a IA a gerar conteúdo de canal personalizado e imagens que complementam sua visão. Quanto mais detalhes você fornecer, maior a chance de produzir uma imagem ou experiência que atenda às suas necessidades. Use uma linguagem clara e descritiva para fornecer o máximo de detalhes possível:

- Para **imagens**, use palavras que descrevam ambiente, humor, cor, composição e estilo.
- Para **copiar**, use palavras que descrevam o público-alvo, a finalidade, as descrições dos novos recursos, exemplos e ações.

Veja a seguir um exemplo de prompt que articula informações sobre sua intenção, público-alvo e estilo.

```bash
Write an email to motivate infrequent users of Photoshop to follow an in-app tutorial that teaches them to combine elements of two photos into a beautiful work of art. Highlight the generative AI capabilities of Photoshop and use references to natural imagery.
```

+++Ver resultados de exemplo

![três emails gerados](/help/assets/sample-email.png)

+++

## Critérios de solicitação

No GenStudio [[!DNL Create]](/help/user-guide/create/overview.md), você pode usar **[!UICONTROL Critérios de solicitação]** ([_Parâmetros_](/help/user-guide/create/overview.md#parameters) e um prompt) na área de prompt para adicionar detalhes por meio da seleção para melhorar a interpretação da IA.

Para [emails](/help/tutorials/create-email-experience.md), os critérios de prompt podem incluir a adição de [diretrizes](/help/user-guide/guidelines/overview.md) em _Parâmetros_, o carregamento de um ativo para usar nas variantes de email e um prompt descritivo. Para um [Meta ad](/help/tutorials/create-meta-ad.md), os critérios de prompt podem incluir uma diretriz de marca em _Parâmetros_, a seleção ou o upload de um ativo existente, configurações relacionadas a imagens ou ativos, como proporção, e um prompt. A verdadeira potência começa com [configurando as diretrizes do GenStudio](/help/user-guide/guidelines/add-guidelines.md).

>[!NOTE]
>
>Se as diretrizes forem adicionadas em _Parâmetros_ na área de prompt, não será necessário incluir referência a elas no prompt. O GenStudio utilizará [!DNL Brands], [!DNL Products] e [!DNL Personas] na geração de conteúdo.

### Diretrizes

As diretrizes do GenStudio ajudam a IA generativa a personalizar a composição de ativos do GenStudio. Quando apresentado com os critérios de prompt, você pode escolher um [[!DNL Brand]](/help/user-guide/guidelines/brands.md), um [[!DNL Persona]](/help/user-guide/guidelines/personas.md) e um [[!DNL Product]](/help/user-guide/guidelines/products.md) a partir das diretrizes configuradas.

>[!TIP]
>
>Você controla como e quando a GenStudio usa suas diretrizes do [!DNL Brand]. Consulte [Diretrizes](/help/user-guide/guidelines/overview.md) para saber como configurar e gerenciar as diretrizes da sua marca.

## Tente novamente

A solicitação é um processo iterativo. Se os resultados não atenderem às suas expectativas, revise seu prompt e faça algumas alterações ou adicione mais detalhes. Você pode refinar seu prompt fornecendo um URL como exemplo ou uma fonte para obter mais informações.

```bash
Write an email to motivate infrequent users of Photoshop to follow an in-app tutorial that teaches them to combine elements of two photos into a beautiful work of art. Highlight the generative AI capabilities of Photoshop and use references to natural imagery.

Use information from https://www.adobe.com/products/photoshop.html to inspire users with the latest features.
```

Ou você pode colar seções de um resumo da campanha. Você pode até solicitar que o GenStudio evite determinadas palavras, elementos ou temas.

## Práticas recomendadas

Algumas práticas recomendadas simples para criar prompts eficazes no GenStudio:

- Seja específico e forneça detalhes sobre o que fazer ou não fazer.
- Fornecer contexto usando referências externas.
- Aproveite as diretrizes do GenStudio.
- Revise e ajuste as diretrizes regularmente.
- Iterar e refinar.
- Aprenda por meio da experimentação.
