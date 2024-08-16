---
title: Preparar um modelo de email para o Adobe GenStudio para profissionais de marketing de desempenho
description: Saiba como criar um modelo de email personalizado para o Adobe GenStudio para profissionais de marketing de desempenho.
level: Intermediate
feature: Templates, Content
source-git-commit: c9d09801f0bd3732611b01d4a98cc7ebf38884d7
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 0%

---


# Preparar modelo de email para o Adobe GenStudio para profissionais de marketing de desempenho

Normalmente, um designer cria o design visual de um modelo em um programa de design, como o Adobe XD. Depois que um modelo de email for projetado, codificado e testado, você poderá prepará-lo para upload e uso no GenStudio para profissionais de marketing de desempenho.

Consulte [Anatomia de um modelo](/help/user-guide/content/use-templates.md#anatomy-of-a-template).

## Adicionar diretrizes

Antes de preparar um modelo de Metadados, verifique se você adicionou [diretrizes](/help/user-guide/guidelines/overview.md) à sua GenStudio para profissionais de marketing de desempenho e se preencheu com informações abrangentes sobre marcas relevantes. As [diretrizes de marca](/help/user-guide/guidelines/brands.md) influenciam diretamente o conteúdo gerado.

**Exemplo**: se você quiser que o corpo de um modelo de email não tenha mais de 500 caracteres, adicione esse requisito às [diretrizes do canal](/help/user-guide/guidelines/brands.md#channel-guidelines) para o campo &quot;corpo&quot;.

Se as diretrizes não forem adicionadas ao GenStudio para profissionais de marketing de desempenho, os padrões serão usados.

## Codifique um modelo de email

Depois que um modelo é projetado, ele é codificado usando HTML e CSS em linha. O código deve ser limpo e responsivo para vários dispositivos.

Consulte [Exemplos de modelo](/help/user-guide/content/customize-template.md#template-examples).

## Testar um modelo de email

Use sua plataforma de entrega ou prova de email para testar seu email e verificar se ele é renderizado corretamente em diferentes clientes e dispositivos de email.

Teste para garantir que seu modelo de email satisfaça o seguinte:

* O layout é ajustado para diferentes tamanhos de tela usando consultas de mídia CSS
* Os botões são clicáveis e navegam até o local desejado
* O modelo de email pode ser lido e usado em dispositivos móveis

## Definir áreas de conteúdo gerado

Defina as áreas no modelo de email que devem ser preenchidas dinamicamente com conteúdo do GenStudio para profissionais de marketing de desempenho.

Para definir áreas de conteúdo geradas:

* Identifique os elementos de texto no modelo que o GenStudio para profissionais de marketing de desempenho devem gerar automaticamente, como o título ou o CTA.
* Adapte o modelo de HTML inserindo espaços reservados dentro dele usando a sintaxe Handblebars.

Consulte [Espaços reservados para conteúdo](/help/user-guide/content/customize-template.md#content-placeholders).

## Pré-visualizar o modelo

Controlar a visibilidade de áreas de conteúdo específicas utilizando Auxiliares integrados. Por exemplo, é possível incluir parâmetros de rastreamento para links em um modelo exportado, mantendo links de visualização limpos.

Consulte [Visualização do modelo](/help/user-guide/content/customize-template.md#template-preview).

## Fazer upload e usar modelo

Depois que seu modelo for criado, codificado, testado e visualizado, você poderá carregá-lo no GenStudio para profissionais de marketing de desempenho para uso na geração de conteúdo de marketing totalmente novo.

Consulte [Trabalhando com modelos](use-templates.md).
