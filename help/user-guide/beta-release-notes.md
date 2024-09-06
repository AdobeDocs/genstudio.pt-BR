---
title: Adobe GenStudio para notas de versão do Beta para profissionais de marketing de desempenho
description: Saiba mais sobre os últimos recursos e aprimoramentos do Adobe GenStudio para profissionais de marketing de desempenho.
exl-id: 2ae60dcb-ac95-4ed4-bceb-84b396f7fa4e
source-git-commit: ca5e746850925252679facc321d7522b251cd57a
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 0%

---

# Adobe GenStudio para notas de versão do Beta para profissionais de marketing de desempenho

Essas notas destacam o Adobe GenStudio significativo para correções e aprimoramentos de profissionais de marketing de desempenho para a semana que terminou em 6 de setembro.

## Novos recursos

* O GenStudio agora oferece suporte à opção de visualização de ativos de mídia no [!DNL Insights]. As miniaturas de vídeo incluem um botão **Reproduzir** com uma opção de mudo. <!-- GS-4398 -->

* O Assets agora pode ser filtrado em [!DNL Insights] pelo tipo `video`. <!-- GS-4398 -->

## Problemas conhecidos

Os seguintes problemas conhecidos estão programados para resolução na versão do GenStudio para a disponibilidade geral dos profissionais de marketing de desempenho.

* Os editores ocasionalmente encontram uma mensagem de erro &quot;Algo deu errado&quot; no [!DNL Create Canvas] durante a geração da imagem. **Solução alternativa**: se o erro se repetir, o usuário poderá fazer logoff e, em seguida, fazer logon novamente no GenStudio e gerar a imagem novamente.  <!-- GS-4813 -->

* O [!DNL Create Canvas] renderiza imagens em Metadados incorretamente. <!-- GS-4864 -->

* O Assets sem campanhas pode ser carregado com êxito em [!DNL Content], mas pode não estar visível para os usuários. <!-- GS-4815 -->

* Há discrepância entre as visualizações da Tela do MetaAds e as visualizações exportadas. <!-- GS-4492 4401 -->

* Miniaturas de campanha ausentes em [!DNL Insights]. <!-- GS-4648 -->

* Atualmente, os usuários podem selecionar pequenos ativos que exigem redimensionamento, mas não há suporte para o aumento desses ativos. <!-- GS-3131 -->

* Os usuários devem fazer logon duas vezes em uma conta de Meta Ads de canal quando também estiverem conectados à Facebook. **Solução alternativa**: faça logout do Facebook antes de fazer logon em uma conta de Meta Ads do canal.

* As imagens carregadas nem sempre incluem as tags inteligentes esperadas. <!-- GS-4856 -->

### Melhorias adicionais e problemas corrigidos

* O pop-up _Adicionar Assets_ agora está localizado conforme esperado. <!-- GS-3834 -->

* Problemas com o dimensionamento do modelo de experiência de Metadados foram resolvidos. <!-- GS-4174 -->

* Os modelos de fragmento de conteúdo criados para modelos agora podem ser representados com precisão no AEM. <!-- GS-4716 -->

* Os campos de texto no arquivo de exportação CSV para emails de várias partes agora são ordenados conforme esperado. <!-- GS-4013 -->

* O campo de pesquisa [!DNL Content] não desaparece mais quando um usuário pressiona repetidamente a tecla **Backspace** para apagar o texto do campo de pesquisa.  <!-- GS-4543 -->

* O GenStudio agora carrega os usuários conforme esperado quando um colaborador adiciona uma menção @ a um comentário. Anteriormente, o GenStudio não carregava usuários e exibia este erro: `Unable to load users. Refresh the page`. <!-- GS-4113 -->

* O GenStudio não exibe mais a mensagem **Ocorreu um erro** quando um editor clica em **Selecionar conteúdo** durante a criação de email na área de prompt. <!-- GS-4879 -->

## Versões anteriores do Beta

As versões anteriores do Beta incluíam os seguintes destaques e correções.

### Destaques

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

* **Redimensionamento de metadados**: os editores podem redimensionar as proporções de metadados. (fixo em 16/08)

* **Contas de logon limitadas do [!DNL Insights]**: o logon do [!DNL Insights] agora dá suporte a apenas uma conta por cliente. (fixo em 16/08)

### Melhorias adicionais e problemas corrigidos

* O nome de posicionamento do feed de página _Detalhes da experiência_ agora especifica o feed do Facebook ou do Instagram. (fixo em 16/08)

* O recorte de imagens e vídeos maiores agora é consistente quando o usuário navega da exibição _Visão geral do ativo_ para a exibição _Detalhes do ativo_. (fixo em 16/08)

* A contagem de resultados de pesquisa da tela Atributos não exibe mais `0 of` antes que um usuário faça logon. (corrigido em 16/08) <!-- GS-3665 -->

* Clicar no campo de contagem **[!UICONTROL [!DNL Insights]]** > **[!UICONTROL Ativo]** não limpa mais as configurações de pesquisa e filtro. (corrigido em 16/08) <!-- GS-3476 -->

### Problemas conhecidos resolvidos em versões anteriores do Beta

* O GenStudio exibe um erro quando um usuário tenta inserir credenciais na exibição [!DNL Insights]. (corrigido em 29/8) <!-- GS-4689 -->

* Falha no upload das diretrizes da marca devido a problemas com a plataforma de armazenamento ACP. (corrigido em 22/8) <!-- GS-4369 -->

* O menu suspenso da área de Prompt [!DNL Brands] exibe um ponteiro no final da lista [!DNL Brands] durante a criação do email. (corrigido em 22/8) <!-- GS-4077 -->
