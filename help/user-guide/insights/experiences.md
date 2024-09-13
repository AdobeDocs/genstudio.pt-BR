---
title: Visão geral das experiências
description: Consulte uma visão geral do engajamento do cliente, orçamento e despesas para experiências e desempenho do ativo no Adobe GenStudio para profissionais de marketing de desempenho.
feature: Insights, Experiences
source-git-commit: ed0ddb10ee65c2691f8ecbfe23533508e9174bf9
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 0%

---


# Visão geral das experiências

A exibição [!DNL Insights] _[!UICONTROL Experiências]_ mostra uma lista de anúncios e experiências para a conta de anúncio do canal conectado.

A tabela [!UICONTROL Experiências] é organizada com [!UICONTROL Nomes de anúncios]. O ícone de filtro (funil) acima do lado esquerdo da tabela abre o menu **[!UICONTROL Filtro]**, onde você pode selecionar nas listas [!UICONTROL Conta] e [!UICONTROL Campanha] para filtrar os nomes de anúncios na tabela.

![Filtro e tabela de experiências](../../assets/insights-experiences-filter.png)

## Detalhes do anúncio

Ao selecionar um nome de anúncio, é possível visualizar as métricas e os atributos de desempenho do anúncio, que permitem analisar as métricas de uma experiência com base no posicionamento do anúncio em um intervalo de datas especificado.

A exibição de detalhes inclui uma métrica para o anúncio geral `click-through rate`, `cost per click`, e quanto do orçamento foi `spent` no anúncio. Como os anúncios podem ter vários posicionamentos, como um feed ou um banner, você pode ver um detalhamento das mesmas métricas para cada posicionamento de anúncio. Use as setas para a esquerda e para a direita em **[!UICONTROL Desempenho por posicionamento de anúncio]** para percorrer as métricas de posicionamento de anúncios.

![Detalhes do anúncio com métricas e posicionamentos de anúncios](../../assets/insights-ad-details.png)

### Atributos de texto

Abaixo da visualização do anúncio está uma lista de [!UICONTROL Atributos de texto] associados ao anúncio. Quando ativos e experiências são aprovados e armazenados no [!DNL Content], o GenStudio for Performance Marketers gera tags com base em seus recursos inerentes. Consulte [detalhes do ativo](../content/asset-details.md#system-metadata) para obter detalhes sobre metadados do sistema.

### Posicionamentos de anúncios

No momento em que você criou uma campanha com Meta Ads, você pode ter selecionado onde executar seus anúncios com base no [objetivo](channels.md#objectives) da campanha. Os posicionamentos de anúncios ampliam o alcance do público-alvo do seu anúncio.

O GenStudio para profissionais de marketing de desempenho é compatível com formatos de anúncios, como feeds de ativos, anúncios de links e imagem ou vídeo únicos. Veja a seguir uma lista de formatos de anúncios por plataforma:

| Instagram | Facebook/Meta | Messenger | Rede de público-alvo |
| --- | --- | --- | --- |
| Explorar<br>Explorar Página Inicial<br>Explorar Página Inicial Do Grid<br>Feed<br>Rolos<br>Feed De Perfil<br>Pesquisa<br>Compras<br>Histórias | Business Explore<br>Feed<br>Vídeo em fluxo<br>Marketplace<br>Reels<br>Sobreposição de Reels<br>Coluna à direita<br>Pesquisa<br>Histórias<br>Feeds de vídeo<br>Anúncios em Facebook Reels | Caixa de entrada<br>Histórias | Nativo, banner e intersticial<br>Nativo<br>Vídeo recompensado |

## Métricas

As métricas de Insights podem ajudar a avaliar quais experiências contribuem para o sucesso de uma campanha e quais posicionamentos de anúncios são mais eficazes.

### Detalhes das métricas

A tabela a seguir fornece definições e insights para as métricas principais de marketing digital na exibição [!UICONTROL Experiências]. Cada métrica inclui uma breve definição, pois se relaciona a nomes de anúncios, como a métrica é calculada, e um ou mais insights para ajudar a entender sua importância e impacto em uma experiência.

| Métrica | Definição | Insight |
| ---------------------- | ----------------------------- | -------------------------------- |
| **[!UICONTROL Campanha]** | Uma campanha é um conjunto de experiências e anúncios projetados para atingir um objetivo específico. | |
| **[!UICONTROL Posicionamentos de anúncios]** | Uma contagem de posicionamentos de anúncios para o anúncio ou experiência. | Os posicionamentos de anúncios aumentam o alcance do público-alvo. |
| **[!UICONTROL Assets]** | Uma contagem dos ativos usados no anúncio ou na experiência. | |
| **[!UICONTROL Impressões]** | As impressões são contadas sempre que o conteúdo é carregado na tela, independentemente da interação ou da visualização. | Uma contagem de alta impressão pode indicar ampla visibilidade, mas, para obter um verdadeiro insight sobre o desempenho, considere com outras métricas de envolvimento. |
| **[!UICONTROL Cliques]** | Número de vezes que os usuários interagem com um elemento clicável em um anúncio. Os cliques podem incluir clicar em um perfil de página ou imagem, uma reação de publicação, compartilhamentos, comentários ou para expandir a mídia para tela inteira. | Uma alta contagem de cliques indica forte interesse e envolvimento com o conteúdo, que pode ser eficaz e alcançar o público-alvo correto. |
| **[!UICONTROL CTR]** | Porcentagem (%) de usuários que clicaram em um anúncio.<br>**Cálculo**: `clicks` dividido por `impressions` | Uma alta taxa de cliques indica que o conteúdo é altamente relevante e motivador para o público-alvo nas mensagens e no design e está efetivamente direcionando os interesses do público-alvo. |
| **[!UICONTROL CPM]** | Medição de desempenho do custo ($) por mil impressões de anúncios.<br>**Cálculo**: valor total `spent` dividido pelo alcance, então multiplicado por 1000 | Um valor baixo pode indicar visibilidade com boa relação custo-benefício, especialmente quando combinado a uma alta taxa de cliques. |
| **[!UICONTROL CPC]** | Custo médio ($) associado a cada clique em uma experiência.<br>**Cálculo**: valor total `spent` dividido por `clicks` | Custos médios mais baixos podem indicar anúncios e gastos econômicos, especialmente quando comparados a um aumento nas conversões. |
| **[!UICONTROL Gastar]** | O valor gasto do orçamento durante um determinado período. | Um alto valor de gasto em um curto período pode indicar uso rápido, o que pode levar ao esgotamento antecipado de recursos. Acompanhe o valor dos gastos em relação às principais métricas de desempenho para ajudar a monitorar o retorno geral sobre o investimento. |
