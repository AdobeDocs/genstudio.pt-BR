---
title: Trabalhar com modelos
description: Saiba como usar modelos para criar experiências envolventes no GenStudio.
feature: Templates, Content
source-git-commit: 6870f1b7056219d03cabbcc4e5ddbfa436b1a56d
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 2%

---


# Trabalhar com modelos

Os modelos do GenStudio são essenciais para permitir que os criadores de conteúdo produzam rapidamente conteúdo de marketing consistente na marca. O uso de modelos reduz significativamente o tempo e o esforço necessários para gerar novo conteúdo, fornecendo um ponto de partida que inclui layouts e elementos de design pré-configurados.

Este guia fornece informações detalhadas sobre como:

* Preparar um [modelo de email](email-template.md) ou um modelo de meta anúncio
* [Personalizar modelos](customize-template.md) para o GenStudio
* [Carregar modelos](#upload-a-template) no GenStudio
* [Usar modelos para criar experiências](#use-a-template)

## Anatomia de um modelo

O design básico do modelo inclui os seguintes elementos:

| Elemento | Função | Modelo de canal |
| ------------ | ---------------------- | -------------------- |
| Pré-cabeçalho | Entre 40 e 50 caracteres <br>Atua como uma linha de assunto secundária aprimorando a linha de assunto principal <br>Visível na caixa de entrada ao lado do assunto antes que o email seja aberto | email |
| Cabeçalho | A seção superior do destinatário do email aparece ao abrir o email <br>Define o tom e fornece o contexto do conteúdo incluído | email |
| Título | O primeiro destinatário de conteúdo a perceber <br>Deve ser convincente para capturar interesse | Meta-anúncio |
| Corpo | Área de conteúdo principal onde a mensagem principal é transmitida <br>Pode incluir texto, imagens e outras mídias | email<br>Meta-anúncio |
| CTA | Frase de chamariz incentivando o recipient a realizar uma ação específica, como clicar em um link ou fazer uma compra | email<br>Meta-anúncio |
| Imagens | Aprimora o apelo visual <br>Divide o texto <br>Dá suporte à mensagem <br>Deve ser de alta qualidade e atraente | email<br>Meta-anúncio |
| Rodapé | Contém informações adicionais como detalhes de contato, links de redes sociais, avisos de isenção de responsabilidade e opções de cancelamento de inscrição | email |
| Sobreposição de texto | O texto em uma imagem <br>Deve suportar e aprimorar o título e o corpo | Meta-anúncio |

>[!NOTE]
> 
>É recomendável incluir campos específicos no conteúdo de cada canal para garantir que o GenStudio possa gerar texto para espaços reservados para conteúdo. Consulte [Nomes de campos reconhecidos](customize-template.md#recognized-field-names) para ver quais campos são recomendados para inclusão.

## Fazer upload de um modelo

O GenStudio aceita modelos no formato HTML.

**Para adicionar um modelo**:

1. Em _[!DNL Content]_, selecione a seção **[!UICONTROL Modelos]**.

1. Clique em **[!UICONTROL Adicionar modelo]**.

1. No painel _[!UICONTROL Adicionar modelo aprovado]_, procure o arquivo de modelo de HTML ou arraste o arquivo de modelo de HTML para soltar espaço. Clique em **[!UICONTROL Avançar]**.

1. No painel _[!UICONTROL Detalhes da estrutura de revisão]_, verifique se você está usando o modelo correto e se todos os detalhes estão conforme o esperado. Clique em **[!UICONTROL Avançar]**.

1. No painel _[!UICONTROL Adicionar detalhes do modelo]_, nomeie o modelo e selecione um tipo de **[!UICONTROL Canal]**.

   O nome do modelo e o tipo de canal são obrigatórios.

   * **Meta**: requer taxa de proporção
   <!-- **Display ads**: requires Dimensions -->

1. Adicione quantos detalhes forem possíveis para melhorar a identificação do modelo em pesquisas e filtragem.

1. Clique em **[!UICONTROL Concluído]**.

## Usar um modelo

Localize e use um modelo existente para criar experiências.

**Para criar uma experiência com um modelo**:

1. Em _[!DNL Content]_, selecione a seção **[!UICONTROL Modelos]**.

   ![Lista de modelos de conteúdo](../../assets/content-templates.png)

1. Selecione um modelo para obter uma exibição completa e uma lista de detalhes.

>[!TIP]
>
>Consulte [[!DNL Create] uma experiência de email](/help/tutorials/create-email-experience.md) ou [[!DNL Create] uma Experiência de metadados](/help/tutorials/create-meta-ad.md) para obter tutoriais completos usando modelos.

<!--  The create button in Content Template view does not work yet.
1. Click **[!UICONTROL Create Experience]** (paintbrush) from the upper right corner to use the template.
-->
