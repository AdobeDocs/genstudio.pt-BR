---
title: Adobe GenStudio para notas de versão do Beta para profissionais de marketing de desempenho
description: Saiba mais sobre os últimos recursos e aprimoramentos do Adobe GenStudio para profissionais de marketing de desempenho.
exl-id: 2ae60dcb-ac95-4ed4-bceb-84b396f7fa4e
source-git-commit: 5f729070a3a4c162ebac0fde9814c649c9984b4d
workflow-type: tm+mt
source-wordcount: '881'
ht-degree: 0%

---

# Adobe GenStudio para notas de versão do Beta para profissionais de marketing de desempenho

Essas notas destacam o Adobe GenStudio significativo para correções e aprimoramentos de Profissionais de marketing de desempenho para a semana que terminou em 13 de setembro.

## Aprimoramentos

* O seletor de conteúdo [!DNL Create] foi refatorado para melhorar o carregamento de ativos. <!-- GS-2586 -->

## Problemas conhecidos

Os seguintes problemas conhecidos estão programados para resolução na versão do GenStudio para a disponibilidade geral dos profissionais de marketing de desempenho.

* Problemas de latência intermitentes afetam algumas operações do Canvas [!DNL Create]. <!-- GS-5203 -->

* A geração de email resulta em um email incompleto. **Solução alternativa**: atualize a página e gere novamente. <!-- GS-5209 -->

* Os modelos podem ser carregados, mas não visualizados. **Solução alternativa**: criar ou carregar um ativo e inserir um nome de grupo de ativos no campo **[!UICONTROL Campanhas]**. Atribuir o ativo a um [!DNL Campaign] adiciona o valor de metadados do nome do grupo. Em seguida, faça upload do template novamente. <!-- GS-4815 -->

* Miniaturas de campanha ausentes em [!DNL Insights]. <!-- GS-4648 -->

* Os usuários devem fazer logon duas vezes em uma conta de Meta Ads de canal quando também estiverem conectados à Facebook. **Solução alternativa**: faça logout do Facebook antes de fazer logon em uma conta de Meta Ads do canal. <!-- GS-4806 -->

### Melhorias adicionais e problemas corrigidos

* A Tela de Pintura [!DNL Create] renderiza imagens em Meta Ads incorretamente. <!-- GS-4864 -->

* Embora possam existir discrepâncias entre as visualizações do Meta Ads Canvas e as visualizações exportadas, as experiências exportadas funcionam conforme esperado. <!-- GS-4492 4401 -->

* As imagens carregadas nem sempre incluem as tags inteligentes esperadas. <!-- GS-4856 -->

* O arquivo CSV de exportação de metadados agora contém imagens conforme esperado. Anteriormente, o arquivo ZIP continha o arquivo de exportação CSV e arquivos NULL em vez de imagens.  <!-- GS-5107 -->

* Agora os usuários podem inserir texto no campo Exibição de detalhes do modelo **[!UICONTROL Carregado por]**, conforme esperado. Anteriormente, o ícone de carregamento impedia os usuários de inserir texto. <!-- GS-4887 -->

* Os usuários não serão mais redirecionados para a exibição de Detalhes de uma marca depois que ela for excluída. <!-- GS-2663 -->

* Os editores não recebem mais o seguinte erro ao enviar variantes para revisão e aprovação: `You have no access to view comments on this Object`. <!-- GS-5140 -->

* Atualização do template de email usado pelo fluxo de trabalho de revisão e aprovação. <!-- GS-5239 -->

* O GenStudio agora exibe uma mensagem de erro quando ocorre um erro de rede durante o carregamento do seletor de modelo. <!-- GS-4682 -->

* Solução de problemas ao navegar de um ativo, experiência ou cartão de modelo para o objeto selecionado. <!-- GS-4390 -->

* O pop-up _Adicionar Assets_ agora está localizado quando aberto a partir de Criar Tela.  <!-- GS-4867 -->

* A validação da marca agora é acionada para variantes regeneradas. Anteriormente, se um editor regenerava variantes de um rascunho existente, a validação não era acionada. <!-- GS-3971 -->

## Versões anteriores do Beta

As versões anteriores do Beta incluíam os seguintes destaques e correções.

### Destaques

* O GenStudio agora oferece suporte à opção de pré-visualização de ativos de mídia nas exibições de tabelas e galerias do [!DNL Insights]. As miniaturas de vídeo incluem um botão **Reproduzir** com uma opção de mudo. <!-- GS-4398 -->

* As diretrizes de canal do instagram e do Facebook foram combinadas nas diretrizes da marca Meta.

* [!DNL Create] Os elementos de navegação da tela de desenho foram otimizados. A página de aterrissagem [!DNL Create] exibe o painel de navegação esquerdo, mas os usuários agora usam o botão **[!UICONTROL Voltar]** para navegar para este espaço a partir de outras áreas de trabalho [!DNL Create].

* Os elementos de navegação foram aprimorados para oferecer suporte ao foco do usuário enquanto executam tarefas em todo o produto, incluindo estas áreas de produtos:

   * Detalhes do ativo, da experiência e do modelo em [!DNL Content]
   * Detalhes de Experiência, Ativo e Atributo em [!DNL Insights]
   * Detalhes da marca em [!DNL Brands]
   * Detalhes de produto e persona em Produtos e personas

* Os usuários não precisam mais clicar no botão **[!UICONTROL Atualizar]** para ver as atualizações das Experiências em [!DNL Content].

* A página _Detalhes da experiência_ agora renderiza miniaturas de ativos externos como HTML.

* A latência da interface do usuário após adicionar ou excluir o Assets e a Experiências foi aprimorada.

* As visualizações do modelo agora incluem mais texto padrão descritivo. Consulte [Personalizar um modelo](https://experienceleague.adobe.com/en/docs/genstudio/user-guide/content/templates/customize-template#template-preview).

* **Pontuação de validação baseada em porcentagem**: a validação de marca agora exibe a pontuação de validação de marca como uma porcentagem, em vez de um valor aprovado/reprovado. (fixo em 16/08)

* **Interface de extração de marca atualizada**: a extração de marca agora mostra a conclusão do processo de extração como uma porcentagem. (fixo em 16/08)

* **Carregamento incremental de marca durante a extração**: as diretrizes de marca agora são carregadas de forma incremental na interface do usuário. (fixo em 16/08)

* **Criação de email de várias seções**: os usuários agora podem criar emails compostos de títulos, imagens, corpo e elementos CTA separados. (fixo em 16/08)

* **Redimensionamento de MetaAds**: editores podem redimensionar as taxas de proporções de MetaAd. (fixo em 16/08)

* **Contas de logon limitadas do [!DNL Insights]**: o logon do [!DNL Insights] agora dá suporte a apenas uma conta por cliente. (fixo em 16/08)

### Melhorias adicionais e problemas corrigidos

* O pop-up _Adicionar Assets_ agora está localizado conforme esperado. <!-- GS-3834 -->

* Problemas com o dimensionamento do modelo de experiência de Metadados foram resolvidos. <!-- GS-4174 -->

* Os campos de texto no arquivo de exportação CSV para emails de várias partes agora são ordenados conforme esperado. <!-- GS-4013 -->

* O campo de pesquisa [!DNL Content] não desaparece mais quando um usuário pressiona repetidamente a tecla **Backspace** para apagar o texto do campo de pesquisa.  <!-- GS-4543 -->

* O GenStudio para profissionais de marketing de desempenho agora carrega os usuários conforme esperado quando um colaborador adiciona uma menção `@` a um comentário. Anteriormente, os usuários não eram carregados e um erro era exibido: `Unable to load users. Refresh the page`. <!-- GS-4113 -->

* O GenStudio não exibe mais a mensagem **Ocorreu um erro** quando um editor clica em **Selecionar conteúdo** durante a criação de email na área de prompt. <!-- GS-4879 -->

* O nome de posicionamento do feed de página _Detalhes da experiência_ agora especifica o feed do Facebook ou do Instagram. (fixo em 16/08)

* O recorte de imagens e vídeos maiores agora é consistente quando o usuário navega da exibição _Visão geral do ativo_ para a exibição _Detalhes do ativo_. (fixo em 16/08)

* A contagem de resultados de pesquisa da tela Atributos não exibe mais `0 of` antes que um usuário faça logon. (corrigido em 16/08) <!-- GS-3665 -->

* Clicar no campo de contagem **[!UICONTROL [!DNL Insights]]** > **[!UICONTROL Ativo]** não limpa mais as configurações de pesquisa e filtro. (corrigido em 16/08) <!-- GS-3476 -->

* O GenStudio exibe um erro quando um usuário tenta inserir credenciais na exibição [!DNL Insights]. (corrigido em 29/8) <!-- GS-4689 -->

* Falha no upload das diretrizes da marca devido a problemas com a plataforma de armazenamento ACP. (corrigido em 22/8) <!-- GS-4369 -->

* O menu suspenso da área de Prompt [!DNL Brands] exibe um ponteiro no final da lista [!DNL Brands] durante a criação do email. (corrigido em 22/8) <!-- GS-4077 -->
