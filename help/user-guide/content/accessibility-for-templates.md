---
title: Criar modelos acessíveis
description: Crie modelos capazes de atingir todos os públicos-alvo para uso no Adobe GenStudio para profissionais de marketing de desempenho.
feature: Templates, Content
source-git-commit: 26d1b9c7b392e93e87ffcd9444f391c2980d1c3c
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 0%

---


# Criar modelos acessíveis

O Adobe tem o compromisso de fornecer uma experiência ideal para todos os públicos-alvo. Consulte [Iniciativas de acessibilidade em Adobe](https://www.adobe.com/trust/accessibility/initiatives.html) para obter mais informações.

No GenStudio para profissionais de marketing de desempenho, você pode fazer upload de ativos e modelos que permitem a criação de conteúdo para uma variedade de experiências. A adesão aos padrões de acessibilidade ajuda seu conteúdo a alcançar o público-alvo máximo desejado.

Use as seguintes recomendações para preparar seus modelos usando os padrões de acessibilidade ideais.

## Texto alternativo

Fornecer alternativas em texto para conteúdo não textual, como imagens.

```html
<img alt="Collage of ideas, books, man holding giant pencil, computer" src="card-create-assets.png">
```

![Colagem de ideias, livros, homem segurando lápis gigante, computador](../../assets/card-create-assets.png){width="400"}

## Finalidade do link (somente link)

Crie um texto de link claro que descreva a finalidade e o local do link.

Por exemplo, usar o texto do link como &quot;Clique aqui&quot; ou &quot;Leia mais&quot; não descreve claramente a finalidade do link:

```html
<a href="product-site.html">Click here</a>
```

Como prática recomendada, você deve usar um texto que descreva claramente para onde o link vai. Um exemplo melhor pode usar o título da fonte do link e a finalidade:

```html
<a href="product-site.html">Explore Product Site</a>
```

## Idioma

Muitos produtos e serviços usam a linguagem de forma criativa ou única. Evite jargões, frases longas e frases complexas. Use um idioma claro, conciso e fácil de ler, compatível com seu público-alvo.

- Use descrições claras, definições em linha ou exemplos relacionáveis quando possível. Pode ser difícil traduzir um vernáculo único.

- Soletre ou vincule a uma definição para as primeiras instâncias de um acrônimo ou abreviação. Pode ser difícil traduzir abreviações.

- Use elementos visuais para complementar texto ou ideias complexas quando possível.
