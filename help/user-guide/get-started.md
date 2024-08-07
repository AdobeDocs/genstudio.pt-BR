---
title: Introdução ao GenStudio
description: Saiba como configurar seu GenStudio para gerar novo conteúdo de marketing alinhado à marca.
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
source-git-commit: 2501d1e36f76d1534a735b9147fb42f762a665e8
workflow-type: tm+mt
source-wordcount: '1066'
ht-degree: 1%

---


# Introdução ao GenStudio

O GenStudio é uma plataforma abrangente para criar, avaliar e gerenciar experiências de marketing que refletem e seguem a identidade da sua marca.

O acesso das partes interessadas a seus vários recursos é controlado pelas funções de usuário atribuídas. Sua função de usuário atribuída determina as tarefas que você pode executar no GenStudio. Um administrador do GenStudio define suas permissões, que são definidas no email de boas-vindas.

Se você é novo em ferramentas generativas baseadas em IA ou está simplesmente curioso sobre os princípios básicos do GenStudio, consulte [Conceitos do GenStudio](concepts.md) e [Comandos efetivos do Write](effective-prompts.md).

## Funções de usuário do GenStudio

A criação e a implantação de campanhas de marketing modernas exigem a colaboração entre as partes interessadas com diferentes responsabilidades e conjuntos de habilidades.

Três tipos de funções de usuário do GenStudio oferecem suporte a essa diversidade de funções organizacionais. As permissões são personalizadas para cada um desses tipos de usuários e oferecem suporte às responsabilidades de cada usuário na organização de marketing.

**Os três tipos de função de usuário são**:

* **Os criadores** usam os recursos de IA gerativa da GenStudio para criar ativos de campanha de marketing, solicitar revisão e aprovação de conteúdo e publicar rascunhos aprovados desse conteúdo. Todos os usuários do GensStudio podem acessar e usar um ativo depois que seu criador o salvar no Conteúdo.

* **Colaboradores** são o maior número de usuários do GenStudio. Os colaboradores podem visualizar e aprovar o conteúdo do GenStudio e são uma parte essencial do fluxo de trabalho, garantindo que o conteúdo gerado corresponda às necessidades e padrões da sua organização.

* **Administradores do sistema** têm o mais amplo conjunto de permissões no GenStudio. Os administradores do sistema podem adicionar e excluir usuários e conteúdo do Genstudio. Os administradores executam a tarefa essencial de integração de estabelecer as medidas de proteção fundamentais para a criação e a implantação do ativo de campanha. Os administradores implementam essas medidas de proteção carregando informações específicas da marca e da organização, como as [diretrizes da marca](/help/user-guide/guidelines/overview.md).

>[!NOTE]
>Antes que qualquer usuário seja provisionado nessas funções, um administrador deve ser designado como superusuário no Admin Console do Adobe para executar tarefas de configuração únicas. Essa função de superusuário opera somente no contexto do Adobe Admin Console. Ele não tem nenhuma função na interface da plataforma do GenStudio. Não há conceito de superusuário nas atribuições de função do GenStudio.

### Criadores

**Os criadores** têm as permissões principais necessárias para criar ativos do GenStudio [!DNL Brands], [!DNL Campaigns] e [!DNL Content]. Eles também podem editar e excluir os ativos que criaram. O GenStudio oferece suporte à criação rápida de centenas de conteúdo. Esses usuários podem gerar fragmentos de conteúdo ou experiências inteiras que orquestram partes distintas de conteúdo aprovado para atender às necessidades de campanhas de marketing específicas.

Os criadores interagem com as tecnologias de IA gerativa da GenStudio por meio de _prompts_. A área de prompt do GenStudio na Tela fornece ferramentas para colocar prompts no contexto das diretrizes de uma campanha específica. Como resultado, a qualidade e o sucesso do conteúdo gerado dependem parcialmente da qualidade das diretrizes de marca que sua organização carregou e da especificidade do seu prompt.

Consulte [Gravar prompts efetivos](effective-prompts.md).

A tabela a seguir exibe as permissões padrão do criador do GenStudio:

| Destaque | Criar | Atualizar o | Excluir | Exibir |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | não | não | não | sim |
| [!DNL Campaigns] | sim | sim | sim | sim |
| [!DNL Content] | sim | sim | sim | sim |
| [!DNL Insights] | pode configurar apenas conectores de anúncios |    |     | sim |
| [!DNL Personas] | sim | sim | sim | sim |
| [!DNL Products] | sim | sim | sim | sim |
| [!DNL Reviews and approvals] | sim | sim | sim | sim |

### Colaboradores

**Os colaboradores** podem exibir ativos na GenStudio, mas não podem criar, editar nem excluir esses ativos. Os colaboradores incluem participantes essenciais para o sucesso do processo de revisão e aprovação do conteúdo do GenStudio, mas que não precisam criar ou editar diretamente o conteúdo. Juristas e gerentes de criadores são exemplos de colaboradores potenciais. Os colaboradores da GenStudio podem ter permissões para criar e visualizar ativos em outros produtos Creative Cloud.

A tabela a seguir exibe as permissões padrão do GenStudio collaborator:

| Destaque | Criar | Atualizar o | Excluir | Exibir |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | sim | sim | sim | sim |
| [!DNL Campaigns] | sim | sim | sim | sim |
| [!DNL Content] | sim | sim | sim | sim |
| [!DNL Insights] | não | não | não | sim |
| [!DNL Personas] | sim | sim | sim | sim |
| [!DNL Products] | sim | sim | sim | sim |
| [!DNL Reviews and approvals] | não | não | não | sim |

### Administradores

Os usuários administradores criam e atribuem usuários a qualquer uma das funções compatíveis com o GenStudio. Eles podem atribuir novas permissões a criadores ou colaboradores individuais, conforme necessário. O trabalho mais importante é concluir as tarefas iniciais de integração que preparam sua organização para implantar o GenStudio.

A tabela a seguir exibe as permissões padrão de administrador do sistema do GenStudio:

| Destaque | Criar | Atualizar o | Excluir | Exibir |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | sim | sim | sim | sim |
| [!DNL Campaigns] | sim | sim | sim | sim |
| [!DNL Content] | sim | sim | sim | sim |
| [!DNL Insights] | sim | sim | sim | sim |
| [!DNL Personas] | sim | sim | sim | sim |
| [!DNL Products] | sim | sim | sim | sim |
| [!DNL Reviews and approvals] | sim | sim | sim | sim |


## Preparar o GenStudio para gerar conteúdo

Os administradores de sistema preparam o ambiente GenStudio de sua organização para que criadores e colaboradores criem ativos de campanha. Essas tarefas preliminares de configuração incluem:

1. [Configurar diretrizes](./guidelines/overview.md) para [!DNL Brands], [!DNL Products] e [!DNL Personas]. Configurando os blocos de construção principais da marca da sua organização **[Adicione diretrizes](./guidelines/overview.md)** ([!DNL Brands], [!DNL Products] e [!DNL Personas]) à GenStudio. Configurar os elementos fundamentais da identidade de marca de sua organização é um pré-requisito essencial para o trabalho dos criadores e colaboradores da GenStudio. Você pode fazer upload de documentos de diretrizes da marca ou inserir manualmente as informações da marca.
   * **Prepare seus documentos de diretrizes**. Quanto mais descritivas e abrangentes forem as diretrizes da sua marca, melhor será o resultado da GenStudio. Inclua exemplos resumidos de recursos que você considera essenciais para sua marca e adicione descrições de comportamento que deseja excluir da criação de conteúdo do GenStudio. O GenStudio extrai informações desses documentos carregados e começa a criar sua marca. Informações como voz da marca, canal e diretrizes de imagem são preenchidas conforme a GenStudio monta cada diretriz dos documentos carregados.
   * **Edite ou preencha os campos de diretriz da marca conforme necessário**. As diretrizes abrangentes da marca formam a base da compreensão da GenStudio sobre a marca da sua organização. Depois que a GenStudio tiver extraído as informações necessárias dos documentos de diretrizes da marca, você será solicitado a editar ou preencher manualmente os campos das informações extraídas. Especifique áreas de foco de produto individuais para criação de conteúdo adicionando um [!DNL Product]. As diretrizes do [!DNL Personas] ajudam a adaptar a criação de conteúdo para segmentos de clientes definidos.

   Embora a configuração das diretrizes de marca de uma organização possa ser uma ação única, talvez seja necessário revisar e aprimorar essas diretrizes com base na volatilidade, no crescimento e nas mudanças nas circunstâncias do mercado de sua organização.

1. **[Carregar modelos](./content/use-templates.md)**. Os modelos fornecem atalhos e aceleram a criação de conteúdo. Um modelo contém recursos aprovados, como cabeçalhos e rodapés, e estabelece medidas de proteção para a criação de conteúdo. Os administradores normalmente fazem upload e gerenciam modelos para sua organização. Os criadores usam modelos para iniciar rapidamente o processo de criação de conteúdo dentro dos limites estabelecidos da marca organizacional.

1. **[Carregar ativos aprovados](./content/manage-assets.md)**. Os ativos aprovados no GenStudio [!DNL Content] estão disponíveis para todos os criadores do GenStudio. Você pode propagar [!DNL Content] com ativos que os criadores podem usar para criar novas experiências ou ativos.

1. **[Conectar a uma conta Meta (Facebook)](./insights/connect-channel.md)**. Você deve configurar uma conexão entre o GenStudio e as contas sociais de sua organização para receber dados de suas campanhas de marketing ativas, ativos e experiências. O [Insights](./insights/overview.md) do GenStudio fornece ferramentas para analisar dados derivados de canais.
