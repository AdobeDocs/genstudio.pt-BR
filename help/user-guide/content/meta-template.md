---
title: Preparar um modelo de meta anúncios para o GenStudio
description: Saiba como criar um modelo de meta anúncio personalizado para o GenStudio.
level: Intermediate
feature: Templates, Content
source-git-commit: 31f02218e02b1400ca9f32472acdecae03dbd304
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 0%

---


# Preparar modelo de meta anúncios para o GenStudio

A criação de um modelo de meta anúncios envolve uma abordagem estruturada e personalizada para redes sociais. Depois que um modelo de meta anúncio for criado e testado, você poderá prepará-lo para upload e uso no GenStudio.

## Adicionar diretrizes

Antes de preparar um modelo de Metadados, verifique se você adicionou [diretrizes](/help/user-guide/guidelines/overview.md) à sua GenStudio e as preencheu com informações abrangentes sobre marcas relevantes. As [diretrizes de marca](/help/user-guide/guidelines/brands.md) influenciam diretamente o conteúdo gerado.

**Exemplo**: se você quiser que o corpo de um modelo de Metadados não tenha mais de 500 caracteres, adicione esse requisito às [diretrizes de canal](/help/user-guide/guidelines/brands.md#channel-guidelines) para o campo &quot;corpo&quot;.

Se as diretrizes não forem adicionadas ao GenStudio, os padrões serão usados.

## Criar um modelo

Normalmente, um designer cria o design visual de um modelo em um programa de design, como o Adobe XD.

Consulte [Anatomia de um modelo](/help/user-guide/content/use-templates.md#anatomy-of-a-template) e [Exemplos de modelo](/help/user-guide/content/customize-template.md#template-examples).

### Especificações de publicidade

A GenStudio aceita estas taxas de proporção para Meta anúncios:

* Quadrado (1:1): 1080 x 1080 pixels
* Vertical (4:5): 1080 x 1350 pixels
* História (9:16): 1080 x 1920 pixels

Se o anúncio não for projetado em uma dessas taxas de aspecto, o GenStudio corta automaticamente a imagem no tamanho apropriado.

## Testar um modelo de meta-anúncio

Teste seu modelo usando o Creative Hub do Meta para ver como o anúncio é exibido em diferentes posicionamentos, como em um feed ou como uma história.

Use sua plataforma de entrega ou prova de email para testar seu email e verificar se ele é renderizado corretamente em diferentes clientes e dispositivos de email.

## Definir áreas de conteúdo gerado

Defina as áreas no seu modelo de email que devem ser preenchidas dinamicamente com conteúdo do GenStudio.

Para definir áreas de conteúdo geradas:

* Identifique os elementos de texto no modelo que o GenStudio deve gerar automaticamente, como o título ou o CTA.
* Adapte o modelo de HTML inserindo espaços reservados dentro dele usando a sintaxe Handblebars.

Consulte [Espaços reservados para conteúdo](/help/user-guide/content/customize-template.md#content-placeholders).

## Pré-visualizar o modelo

Controlar a visibilidade de áreas de conteúdo específicas utilizando Auxiliares integrados. Por exemplo, é possível incluir parâmetros de rastreamento para links em um modelo exportado, mantendo links de visualização limpos.

Consulte [Visualização do modelo](/help/user-guide/content/customize-template.md#template-preview).

## Fazer upload e usar modelo

Depois que seu modelo for projetado, codificado, testado e visualizado, você poderá carregá-lo no GenStudio para uso na geração de conteúdo de marketing totalmente novo.

Consulte [Trabalhando com modelos](use-templates.md).
