---
title: Adobe GenStudio para notas de versão do Beta para profissionais de marketing de desempenho
description: Saiba mais sobre os últimos recursos e aprimoramentos do Adobe GenStudio para profissionais de marketing de desempenho.
exl-id: 2ae60dcb-ac95-4ed4-bceb-84b396f7fa4e
source-git-commit: 7085fa5a12a6ed36c9310f8f691969d9c1366d36
workflow-type: tm+mt
source-wordcount: '1348'
ht-degree: 0%

---

# Adobe GenStudio para notas de versão do Beta para profissionais de marketing de desempenho

Essas notas destacam o Adobe GenStudio significativo para correções e aprimoramentos de Profissionais de marketing de desempenho para a semana que terminou em 19 de setembro.

## Novos recursos e melhorias

* **Integração com o Adobe Experience Manager Assets**. O acesso somente leitura ao Adobe Experience Manager Assets agora está disponível. <!-- GS-2432 -->

* **Melhorias no fluxo de trabalho do Modelo de Atualização**.  Os usuários que atualizam modelos agora selecionam o canal para o qual desejam usar o modelo. <!-- GS-4029 -->

* **Desempenho de criação de carregamento de página aprimorado**. As dependências não utilizadas foram removidas do processo de carregamento da página. <!-- GS-3630 -->

* **Suporte a email de várias seções**. Os editores agora podem gerar emails que contêm várias seções e imagens. Eles também podem regenerar fragmentos específicos de um email gerado (por exemplo, um título). <!-- GS-2436 -->

* **Alternar entre exibição móvel e de área de trabalho durante a criação**. Agora os usuários podem alternar entre a exibição para desktop e dispositivo móvel para visualizar as variantes de experiência de email. <!-- GS-4314 -->

* O conteúdo agora gera imagens com dimensões de corte relativas às dimensões do ativo original. <!-- GS-3150 -->

* Agora os usuários podem selecionar variantes de imagem geradas e usar o recurso Ajustar recorte para recortá-las durante o fluxo de trabalho de criação. <!-- GS-5538 2342 -->

* A exibição Detalhes de uma experiência aprovada agora exibe uma imagem em miniatura e o status de todos os ativos referenciados nessa experiência. <!-- GS-3783 -->

## Problemas conhecidos

Os seguintes problemas conhecidos estão programados para resolução na versão do GenStudio para a disponibilidade geral dos profissionais de marketing de desempenho.

* Problemas de latência intermitentes afetam algumas operações do Canvas [!DNL Create]. <!-- GS-5203 -->

* A geração de email resulta em um email incompleto. **Solução alternativa**: atualize a página e gere novamente. <!-- GS-5209 -->

* Os modelos podem ser carregados, mas não visualizados. **Solução alternativa**: carregue um ativo com o campo **[!UICONTROL Campanhas]** preenchido. Em seguida, faça upload do template novamente. <!-- GS-4815 -->

* Os usuários devem fazer logon duas vezes em uma conta de Metadados do canal quando também estiverem conectados à Facebook. **Solução alternativa**: faça logout do Facebook antes de fazer logon em uma conta de Metadados do canal. <!-- GS-4806 -->

### Melhorias adicionais e problemas corrigidos

* Arrastar e soltar agora funciona conforme esperado na área de prompt. <!-- GS-3977 -->

* Correção de problemas com o uso da tecla Tab para navegar pelos elementos na barra de navegação esquerda. Anteriormente, vários cliques eram necessários para navegar de um elemento para o próximo elemento ativo.  <!-- GS-2639 -->

* O GenStudio agora salva nomes de experiência quando os usuários editam o nome enquanto a experiência é carregada. <!-- GS-5242 -->

* Os usuários agora podem editar um título de experiência com sucesso. Anteriormente, o texto do título assumia o padrão do texto original depois que um usuário tentava editá-lo. <!-- GS-5246 -->
* As imagens selecionadas agora são renderizadas na Tela conforme esperado durante a criação de email de várias partes. <!-- GS-5263 -->

* Todas as cadeias de caracteres na página Detalhes das experiências [!DNL Content] foram localizadas. <!-- GS-5016 -->

* Os usuários agora podem excluir um produto cujo modo de exibição de Detalhes esteja aberto em [!DNL Products]. <!-- GS-5057 -->

* A mensagem que o GenStudio exibe quando uma pesquisa não produz resultados correspondentes foi aprimorada. <!-- GS-4544 -->

* `aria-label` valores de atributo para valores de filtro de pesquisa agora são traduzidos conforme esperado. <!-- GS-5388 -->

* Os usuários agora podem excluir ativos duplicados na área de prompt Tela [!DNL Create] com êxito.  <!-- GS-5233 -->

* O filtro Conta agora funciona conforme esperado com experiências, ativos e atributos. <!-- GS-4812 -->

* Problemas de fonte nos modelos de metadados foram resolvidos para melhorar a legibilidade e a acessibilidade. <!-- GS-5354 -->

* As alterações nos títulos de rascunho agora persistem conforme esperado. Anteriormente, os títulos eram revertidos para o nome padrão após a edição. <!-- GS-2951 -->

#### Correções de modelos

* O recurso de redimensionamento agora funciona conforme esperado com várias imagens em modelos de meta-anúncios. Anteriormente, o GenStudio não redimensionava imagens para todos os modelos selecionados. <!-- GS-4696 -->

* A exclusão de um modelo agora atualiza a página [!DNL Content] conforme esperado. <!-- GS-5397 -->

* Os usuários agora podem escolher valores para [!DNL Personas], [!DNL Brands] ou [!DNL Products] somente no menu suspenso. Anteriormente, a caixa de diálogo _Carregamento de modelo_ permitia que os usuários inserissem qualquer nome [!DNL Persona], [!DNL Brand] ou [!DNL Product]. <!-- GS-5072 5071-->

* O botão **[!UICONTROL Voltar]** agora está desabilitado durante o processo de carregamento do Modelo. <!-- GS-5358 -->

* Todas as cadeias de caracteres na exibição de detalhes do modelo Select [!DNL Create] agora estão localizadas. <!-- GS-5025 -->

## Versões anteriores do Beta

As versões anteriores do Beta incluíam os seguintes destaques e correções.

### Destaques

* O seletor de conteúdo [!DNL Create] foi refatorado para melhorar o carregamento de ativos. <!-- GS-2586 -->

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

* **Redimensionamento de metaanúncios**: os editores podem redimensionar as taxas de proporções de metaanúncio. (fixo em 16/08)

* **Contas de logon limitadas do [!DNL Insights]**: o logon do [!DNL Insights] agora dá suporte a apenas uma conta por cliente. (fixo em 16/08)

### Melhorias adicionais e problemas corrigidos

* A Tela do [!DNL Create] agora renderiza imagens em Metadados corretamente. (corrigido em 13/09) <!-- GS-4864 -->

* Embora possam existir discrepâncias entre as visualizações da Tela de metadados e as visualizações exportadas, as experiências exportadas funcionam conforme esperado. (corrigido em 13/09) <!-- GS-4492 4401 -->

* As imagens carregadas agora incluem as tags inteligentes esperadas. (corrigido em 13/09) <!-- GS-4856 -->

* O arquivo CSV de exportação de metadados agora contém imagens, conforme esperado. Anteriormente, o arquivo ZIP continha o arquivo de exportação CSV e arquivos NULL em vez de imagens. (corrigido em 13/09) <!-- GS-5107 -->

* Agora os usuários podem inserir texto no campo Exibição de detalhes do modelo **[!UICONTROL Carregado por]**, conforme esperado. Anteriormente, o ícone de carregamento impedia os usuários de inserir texto. (corrigido em 13/09) <!-- GS-4887 -->

* Os usuários não serão mais redirecionados para a exibição de Detalhes de uma marca depois que ela for excluída. (corrigido em 13/09) <!-- GS-2663 -->

* Os editores não recebem mais o seguinte erro ao enviar variantes para revisão e aprovação: `You have no access to view comments on this Object`. (corrigido em 13/09) <!-- GS-5140 -->

* Atualização do template de email usado pelo fluxo de trabalho de revisão e aprovação. (corrigido em 13/09) <!-- GS-5239 -->

* O GenStudio agora exibe uma mensagem de erro quando ocorre um erro de rede durante o carregamento do seletor de modelo. (corrigido em 13/09) <!-- GS-4682 -->

* Solução de problemas ao navegar de um ativo, experiência ou cartão de modelo para o objeto selecionado. (corrigido em 13/09) <!-- GS-4390 -->

* O pop-up _Adicionar Assets_ agora está localizado quando aberto a partir de Criar Tela. (corrigido em 13/09) <!-- GS-4867 -->

* A validação da marca agora é acionada para variantes regeneradas. Anteriormente, se um editor regenerava variantes de um rascunho existente, a validação não era acionada. (corrigido em 13/09) <!-- GS-3971 -->

* O pop-up _Adicionar Assets_ agora está localizado conforme esperado. (corrigido em 5/9) <!-- GS-3834 -->

* Problemas com o dimensionamento do modelo de experiência de Metadados foram resolvidos. (corrigido em 5/9) <!-- GS-4174 -->

* Os campos de texto no arquivo de exportação CSV para emails de várias partes agora são ordenados conforme esperado. (corrigido em 5/9) <!-- GS-4013 -->

* O campo de pesquisa [!DNL Content] não desaparece mais quando um usuário pressiona repetidamente a tecla **Backspace** para apagar o texto do campo de pesquisa. (corrigido em 5/9) <!-- GS-4543 -->

* O GenStudio para profissionais de marketing de desempenho agora carrega os usuários conforme esperado quando um colaborador adiciona uma menção `@` a um comentário. Anteriormente, os usuários não eram carregados e um erro era exibido: `Unable to load users. Refresh the page`. (corrigido em 29/8) <!-- GS-4113 -->

* O GenStudio não exibe mais a mensagem **Ocorreu um erro** quando um editor clica em **Selecionar conteúdo** durante a criação de email na área de prompt. <!-- GS-4879 -->

* O nome de posicionamento do feed de página _Detalhes da experiência_ agora especifica o feed do Facebook ou do Instagram. (fixo em 16/08)

* O recorte de imagens e vídeos maiores agora é consistente quando o usuário navega da exibição _Visão geral do ativo_ para a exibição _Detalhes do ativo_. (fixo em 16/08)

* A contagem de resultados de pesquisa da tela Atributos não exibe mais `0 of` antes que um usuário faça logon. (corrigido em 16/08) <!-- GS-3665 -->

* Clicar no campo de contagem **[!UICONTROL [!DNL Insights]]** > **[!UICONTROL Ativo]** não limpa mais as configurações de pesquisa e filtro. (corrigido em 16/08) <!-- GS-3476 -->

* O GenStudio exibe um erro quando um usuário tenta inserir credenciais na exibição [!DNL Insights]. (corrigido em 29/8) <!-- GS-4689 -->

* Falha no upload das diretrizes da marca devido a problemas com a plataforma de armazenamento ACP. (corrigido em 22/8) <!-- GS-4369 -->

* O menu suspenso da área de Prompt [!DNL Brands] exibe um ponteiro no final da lista [!DNL Brands] durante a criação do email. (corrigido em 22/8) <!-- GS-4077 -->
