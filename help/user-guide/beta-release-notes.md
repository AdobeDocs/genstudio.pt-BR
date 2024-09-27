---
title: Notas de versão do Adobe GenStudio for Performance Marketing Beta
description: Saiba mais sobre os recursos e aprimoramentos mais recentes do Adobe GenStudio for Performance Marketing.
exl-id: 2ae60dcb-ac95-4ed4-bceb-84b396f7fa4e
source-git-commit: ca83beb4d6f5bd0d79a2da69658b6e18c3252f2e
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 0%

---

# Notas de versão do Adobe GenStudio for Performance Marketing Beta

Essas notas destacam correções e aprimoramentos significativos do Adobe GenStudio for Performance Marketing para a semana que terminou em 27 de setembro.

## Novos recursos e melhorias

* O GenStudio agora pode extrair informações pessoais e de produtos de um PDF carregado e preencher campos relacionados. <!-- GS-3806 -->

* Agora os usuários podem filtrar [!DNL Content] ativos e experiências pelo nome do usuário que carregou o ativo. <!-- GS-1808 -->

* A seção [!DNL Additional details] foi renomeada para [!DNL Messaging preferences] na página de detalhes [!DNL Products]. <!-- GS-5133 5134 -->

* Adição de um botão [!DNL Add persona] à página _Adicionar sua primeira persona_. <!-- GS-5132 -->

## Problemas conhecidos

Os seguintes problemas conhecidos estão programados para serem resolvidos na versão do GenStudio for Performance Marketing GA.

* Os modelos podem ser carregados, mas não visualizados. **Solução alternativa**: carregue um ativo com o campo **[!UICONTROL Campanhas]** preenchido. Em seguida, faça upload do template novamente. <!-- GS-4815 5650-->

* Os usuários não podem recortar manualmente os meta anúncios depois de redimensioná-los. <!-- GS-5871 -->

* Os usuários podem criar um novo [!DNL Campaign] a partir de [!DNL Content] fluxos de trabalho. <!-- GS-5650 -->

* Os usuários devem fazer logon duas vezes em uma conta de Metadados do canal quando também estiverem conectados à Facebook. Solução alternativa: Faça logout do Facebook antes de fazer logon em uma conta de Meta ads do canal. <!-- GS-3009 -->

### Melhorias adicionais e problemas corrigidos

* Problemas de latência intermitentes com algumas operações do Canvas [!DNL Create] foram resolvidos. <!-- GS-5203 -->

* Os usuários não precisam mais fazer logon duas vezes em uma conta de Metadados do canal quando também estão conectados ao Facebook. <!-- GS-4806 -->

* A geração de email agora resulta mais em um email incompleto. <!-- GS-5209 -->

* A criação de uma campanha no workflow do template agora armazena IDs conforme esperado.  <!-- GS-4923 -->

* O seletor de vários repositórios agora lista os repositórios em ordem alfabética. <!-- GS-5553 -->

* Problemas com formatos de arquivo de exportação CSV para idiomas diferentes do inglês foram resolvidos. <!-- GS-5141 -->

* Agora os usuários podem clicar no botão [!DNL Create] _Trabalho recente_ área **[!UICONTROL Exibir todos os rascunhos]** enquanto os rascunhos estão carregando. Anteriormente, clicar neste botão antes do carregamento de todos os rascunhos resultava no carregamento de apenas alguns rascunhos, e o botão **[!UICONTROL Exibir todos os rascunhos]** ficava indisponível. <!-- GS-3938 -->

* A Tela de Pintura [!DNL Create] agora exibe o botão **[!UICONTROL Exibir todos os rascunhos]**, conforme esperado, quando a Tela de Pintura exibe mais de quatro rascunhos. <!-- GS-5588 -->

* A pesquisa agora funciona conforme esperado na guia _Atributos_. <!-- GS-5658 -->

* A animação com brilho agora é dimensionada corretamente durante o carregamento da experiência. <!-- GS-5574 -->

* As visualizações de miniaturas para emails de várias partes agora são renderizadas conforme esperado em [!DNL Content]. <!-- GS-5258 -->

* Correção de um problema relacionado ao Workfront com o botão **[!UICONTROL Enviar para aprovação]**. <!-- GS-5847 -->

* Correção de problemas com o carregamento do shimmer na exibição de trabalho [!DNL Create] Recente. <!-- GS-5589 -->

* Inserir um termo de pesquisa agora resulta em apenas uma chamada de pesquisa, conforme esperado.  <!-- GS-2999 -->

* Renderização de imagem corrigida de imagens geradas por metadados após a exportação. <!-- GS-5749 -->

* O símbolo `%` agora é renderizado corretamente nas localidades DEU, FRA e ESP quando os usuários ampliam ou reduzem o zoom de variantes de email na Tela C[!DNL Create]. <!-- GS-5007 -->


#### Localização

Esta versão inclui aprimoramentos na localização em toda a interface do produto, especialmente em [!DNL Create]. Os seguintes componentes de interface foram localizados: <!-- GS-5295 -->

* Todas as cadeias de caracteres na área _Prompt_ (título de parâmetros, nomes de opções de menu suspenso e texto de espaço reservado de prompt) <!-- GS-5027 -->

* Todas as cadeias de caracteres na janela _Redimensionar_ para Metadados gerados em [!DNL Create] <!-- GS-5035 -->

* Todas as cadeias de caracteres na área _Trabalho recente_ em [!DNL Create] <!-- GS-5037 -->

* As cadeias de caracteres da opção de menu suspenso Marcas, Personalidades e Produto na área de Prompt <!-- GS-5293 -->

* A sequência de caracteres **Zoom para caber na tela** exibida durante o email e a geração de metadados <!-- GS-5063 -->

* Formatos de data e hora, sequência de caracteres **Rascunho sem título** e mensagens de erro em emails e nomes de metaanúncios <!-- GS-5023 5022 5048-->

* As cadeias de exibição de galeria de guias [!DNL Content] _Assets_ e o símbolo de porcentagem (%) <!-- GS-4983 4984-->

* O símbolo de porcentagem (%) usado na taxa de cliques de Insights > Experiências <!-- GS-4279 -->

* Mensagem de erro exibida quando ocorre um erro do sistema durante o email ou a criação de Metadados<!-- GS-5061 -->

* Separador decimal da frase &quot;Contagem de Palavras por Frase&quot; na página Detalhes da experiência do Insights <!-- GS-4986 -->

* Cadeias de caracteres no menu Exportar para um Meta anúncio gerado com um modelo. <!-- GS-5031 -->

