---
title: Adobe GenStudio para notas de versão do Beta para profissionais de marketing de desempenho
description: Saiba mais sobre os últimos recursos e aprimoramentos do Adobe GenStudio para profissionais de marketing de desempenho.
source-git-commit: cbae3aeb1b8282fb64f2a6405a7ad9e07a48dbbd
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%

---


# Adobe GenStudio para notas de versão do Beta para profissionais de marketing de desempenho

Essas notas destacam correções de Adobe GenStudio e aprimoramentos significativos para a semana que terminou em 16 de agosto.

## Destaques

O desenvolvimento de recursos é rápido e contínuo. Os novos recursos notáveis incluem:

### [!DNL Brands]

O painel de validação [!DNL Brand] foi aprimorado para melhorar a experiência do usuário, incluindo estas alterações:

* **Pontuação de validação baseada em porcentagem**: a validação de marca agora exibe a pontuação de validação de marca como uma porcentagem, em vez de um valor aprovado/reprovado.

* **Interface de extração de marca atualizada**: a extração de marca agora mostra a conclusão do processo de extração como uma porcentagem.

* **Carregamento incremental de marca durante a extração**: as diretrizes de marca agora são carregadas de forma incremental na interface do usuário.

* **Simplificação do esquema de Diretriz de Cópia**: os campos `unique attributes` e `frequent keywords` foram removidos do esquema de Diretriz de Cópia, simplificando o processo de configuração de diretriz.

### [!DNL Create]

* **Criação de email de várias seções**: os usuários agora podem criar emails compostos de títulos, imagens, corpo e elementos CTA separados.

* **Redimensionamento de metadados**: os criadores podem redimensionar proporções de metadados.

### [!DNL Insights]

* **Contas de logon do Limited Insights**: o logon do Insights agora oferece suporte a apenas uma conta por cliente.

## Melhorias e problemas corrigidos

Esta versão inclui as seguintes correções adicionais.

### [!DNL Insights]

* O nome de posicionamento do feed de página _Detalhes da experiência_ agora especifica o feed do Facebook ou do Instagram.

* O recorte de imagens e vídeos maiores agora é consistente quando o usuário navega da exibição _Visão geral do ativo_ para a exibição _Detalhes do ativo_.

* A contagem de resultados de pesquisa da tela Atributos não exibe mais `0 of` antes que um usuário faça logon. <!-- GS- 3665 -->

* Clicar no campo de contagem **[!UICONTROL [!DNL Insights]]** > **[!UICONTROL Ativo]** não limpa mais as configurações de pesquisa e filtro. <!-- GS-3476 -->

## Problemas conhecidos

Os seguintes problemas conhecidos serão resolvidos pela versão do GenStudio for Performance Marketers GA.

### Analytics

* As ações acionadas pelos botões **[!UICONTROL Adicionar modelos]** e **[!UICONTROL Carregar]** não são rastreadas no momento. <!-- GS-3505 -->

### [!DNL Insights]

* Vídeos não podem ser reproduzidos do _Assets_. <!-- GS-3846 -->

* Os usuários devem fazer logon duas vezes quando também estiverem conectados à Facebook. **Solução alternativa**: saia da Facebook antes de fazer logon em [!DNL Insights].

* **Os valores de gastos no nível da campanha** não são precisos. No momento, os dados não são consistentes entre o Facebook Ads Manager e o data lake. <!-- GS-3202 -->

### [!DNL Reviews and Approvals]

* Os criadores podem alterar os ativos após a aprovação antes da publicação. Os aprovadores não são notificados sobre essas alterações.

