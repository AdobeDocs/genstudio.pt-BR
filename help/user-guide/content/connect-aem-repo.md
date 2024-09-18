---
title: Conectar-se a um repositório do AEM Assets Content Hub
description: Saiba como conectar o GenStudio para profissionais de marketing de desempenho a um repositório do Adobe Experience Manager (AEM) Content Hub e aproveitar o conteúdo aprovado existente.
level: Experienced
feature: Assets, Content
source-git-commit: dc438085cfe7c93b20dc7fb0d5919d2dc8b3dcde
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 0%

---

# Conectar a um repositório [!DNL AEM Assets Content Hub]

Se você tiver ativos no Adobe Experience Manager (AEM), é possível seguir essas etapas para torná-los acessíveis no GenStudio para profissionais de marketing de desempenho.

>[!BEGINSHADEBOX]

**Pré-requisitos**:

As etapas a seguir exigem acesso administrativo ao Admin Console e AEM Assets as a Cloud Service.

>[!ENDSHADEBOX]

## Etapa 1: Habilitar [!DNL AEM Assets Content Hub]

Siga o processo de autoatendimento **Implantar Content Hub** para habilitar o [!DNL Content Hub] para sua AEM Assets existente no Cloud Manager. Consulte [Implantar [!DNL Content Hub]](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub) na documentação do _AEM as a Cloud Service_.

Depois de habilitar [!DNL AEM Assets Content Hub], você tem uma nova instância com o sufixo `contenthub` em [!DNL AEM Assets as a Cloud Service] no Admin Console.

## Etapa 2: integrar usuários do GenStudio

No [!DNL Admin Console], adicione usuários ou grupos de usuários do GenStudio aos perfis de produto do [!DNL AEM Assets Content Hub]. [!DNL AEM Assets Content Hub] usuários podem exibir ativos, mas não podem adicionar ativos ou modificar ativos existentes.

- [Integrar [!DNL Content Hub] administrador](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub#onboard-content-hub-administrator)
- [Integrar [!DNL Content Hub] usuários](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/deploy-content-hub#onboard-content-hub-users)

## Etapa 3: Aprovar ativos

Aprove ativos para uso em [!DNL AEM Assets Content Hub], o que os torna disponíveis no GenStudio para profissionais de marketing de desempenho. Consulte [Aprovar ativos no Experience Manager](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/dynamicmedia/dynamic-media-open-apis/approve-assets) na documentação do _AEM as a Cloud Service_.

## Etapa 4: configurar a visibilidade do ativo

Nas opções de configuração do _[!DNL AEM Assets Content Hub]_, analise cada conjunto de opções de configuração para filtros, detalhes de ativos, pesquisa e identidade visual. Consulte [Configurar interface do usuário do Content Hub](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/content-hub/configure-content-hub-ui-options) na documentação do_ AEM as a Cloud Service _.

## Etapa 5: verificar a conexão

No GenStudio para Conteúdo de Profissionais de Marketing de Desempenho, a lista _[!UICONTROL Local]_ está disponível acima da galeria, no lado direito. A lista não estará disponível se você não tiver acesso ou se sua organização não tiver implantado e conectado um repositório do [!DNL AEM Assets Content Hub].
