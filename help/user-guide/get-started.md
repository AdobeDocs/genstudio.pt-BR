---
title: Introdução ao Adobe GenStudio para profissionais de marketing de desempenho
description: Saiba como configurar seu GenStudio para que os profissionais de marketing de desempenho gerem novo conteúdo de marketing alinhado à marca.
level: Beginner
feature: Prompt, Brands Service, Personas Service, Products Service, Generative AI, Guidelines
source-git-commit: c9d09801f0bd3732611b01d4a98cc7ebf38884d7
workflow-type: tm+mt
source-wordcount: '1117'
ht-degree: 1%

---


# Introdução ao Adobe GenStudio para profissionais de marketing de desempenho

O GenStudio para profissionais de marketing de desempenho é uma plataforma abrangente para criar, avaliar e gerenciar experiências de marketing que refletem e seguem a identidade da sua marca.

O acesso das partes interessadas a seus vários recursos é controlado pelas funções de usuário atribuídas. Sua função de usuário atribuída determina as tarefas que você pode executar no GenStudio para profissionais de marketing de desempenho. Um administrador define suas permissões, definidas no email de boas-vindas.

Se você é novo em ferramentas gerativas baseadas em IA ou está simplesmente curioso sobre os princípios básicos do GenStudio for Performance Marketers, consulte [Conceitos](concepts.md) e [Gravar prompts efetivos](effective-prompts.md).

## Funções do usuário

A criação e a implantação de campanhas de marketing modernas exigem a colaboração entre as partes interessadas com diferentes responsabilidades e conjuntos de habilidades.

Três tipos de funções de usuário do GenStudio para profissionais de marketing de desempenho oferecem suporte a essa diversidade de funções organizacionais. As permissões são personalizadas para cada um desses tipos de usuários e oferecem suporte às responsabilidades de cada usuário na organização de marketing.

**Os três tipos de função de usuário são**:

* **Os criadores** usam o GenStudio para os recursos de IA gerativa dos profissionais de marketing de desempenho para criar ativos de campanha de marketing, solicitar revisão e aprovação de conteúdo e publicar rascunhos aprovados desse conteúdo. Todos os usuários do GensStudio podem acessar e usar um ativo depois que seu criador o salvar no Conteúdo.

* **Colaboradores** são a maior variedade de GenStudio para usuários de profissionais de marketing de desempenho. Os colaboradores podem visualizar e aprovar o conteúdo e são uma parte essencial do fluxo de trabalho, garantindo que o conteúdo gerado corresponda às necessidades e padrões da sua organização.

* **Administradores do sistema** têm o mais amplo conjunto de permissões no GenStudio para profissionais de marketing de desempenho. Os administradores do sistema podem adicionar e excluir usuários e conteúdo. Os administradores executam a tarefa essencial de integração de estabelecer as medidas de proteção fundamentais para a criação e a implantação do ativo de campanha. Os administradores implementam essas medidas de proteção carregando informações específicas da marca e da organização, como as [diretrizes da marca](/help/user-guide/guidelines/overview.md).

>[!NOTE]
>Antes que qualquer usuário seja provisionado nessas funções, um administrador deve ser designado como superusuário no Admin Console do Adobe para executar tarefas de configuração únicas. Essa função de superusuário opera somente no contexto do Adobe Admin Console. Ela não tem função na interface da plataforma GenStudio para profissionais de marketing de desempenho. Não há conceito de superusuário nas atribuições de função do GenStudio para profissionais de marketing de desempenho.

### Criadores

**Os criadores** têm as permissões principais necessárias para criar GenStudio para os profissionais de marketing de desempenho [!DNL Brands], [!DNL Campaigns] e [!DNL Content] ativos. Eles também podem editar e excluir os ativos que criaram. O GenStudio para profissionais de marketing de desempenho oferece suporte à criação rápida de centenas de conteúdo. Esses usuários podem gerar fragmentos de conteúdo ou experiências inteiras que orquestram partes distintas de conteúdo aprovado para atender às necessidades de campanhas de marketing específicas.

Os criadores interagem com a GenStudio para obter as tecnologias de IA gerativa dos profissionais de desempenho por meio de _prompts_. A área de prompt na Tela de Pintura fornece ferramentas para colocar prompts no contexto das diretrizes de uma campanha específica. Como resultado, a qualidade e o sucesso do conteúdo gerado dependem parcialmente da qualidade das diretrizes de marca que sua organização carregou e da especificidade do seu prompt.

Consulte [Gravar prompts efetivos](effective-prompts.md).

A tabela a seguir exibe as permissões padrão do criador:

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

**Os colaboradores** podem exibir ativos no GenStudio para profissionais de marketing de desempenho, mas não podem criar, editar nem excluir esses ativos. Os colaboradores incluem participantes essenciais para o sucesso do processo de revisão e aprovação do conteúdo, mas que não precisam criar ou editar diretamente o conteúdo. Juristas e gerentes de criadores são exemplos de colaboradores potenciais. Os colaboradores do GenStudio para Marketing de Desempenho podem ter permissões para criar e visualizar ativos em outros produtos Creative Cloud.

A tabela a seguir exibe as permissões padrão do colaborador:

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

**Os administradores** criam e atribuem usuários a qualquer uma das funções aceitas do GenStudio for Performance Marketers. Eles podem atribuir novas permissões a criadores ou colaboradores individuais, conforme necessário. O trabalho mais crítico é concluir as tarefas iniciais de integração que preparam sua organização para implantar o GenStudio para profissionais de marketing de desempenho.

A tabela a seguir exibe as permissões padrão do administrador do sistema:

| Destaque | Criar | Atualizar o | Excluir | Exibir |
|-----------|----------------|----------------|----------------|----------------|
| [!DNL Brands] | sim | sim | sim | sim |
| [!DNL Campaigns] | sim | sim | sim | sim |
| [!DNL Content] | sim | sim | sim | sim |
| [!DNL Insights] | sim | sim | sim | sim |
| [!DNL Personas] | sim | sim | sim | sim |
| [!DNL Products] | sim | sim | sim | sim |
| [!DNL Reviews and approvals] | sim | sim | sim | sim |


## Preparar o GenStudio para que os profissionais de marketing de desempenho gerem conteúdo

Os administradores de sistema preparam o ambiente GenStudio para profissionais de marketing de desempenho de sua organização para que criadores e colaboradores criem ativos de campanha. Essas tarefas preliminares de configuração incluem:

1. [Adicionar diretrizes](./guidelines/overview.md) para [!DNL Brands], [!DNL Products] e [!DNL Personas]. Configurar os elementos fundamentais da identidade de marca de sua organização é um pré-requisito essencial para o trabalho de criadores e colaboradores. Você pode fazer upload de documentos de diretrizes da marca ou inserir manualmente as informações da marca.
   * **Prepare seus documentos de diretrizes**. Quanto mais descritivas e abrangentes forem as diretrizes da sua marca, melhor será o resultado. Inclua breves exemplos de recursos que você considera essenciais para sua marca e adicione descrições de comportamento que deseja excluir da criação de conteúdo. O GenStudio para profissionais de marketing de desempenho extrai informações desses documentos carregados e começa a criar sua marca. Informações como voz da marca, canal e diretrizes de imagem são preenchidas conforme o GenStudio para profissionais de marketing de desempenho monta cada diretriz dos documentos carregados.
   * **Edite ou preencha os campos de diretriz da marca conforme necessário**. GenStudio As diretrizes abrangentes de marca formam a base da compreensão da marca da sua organização por parte dos profissionais de marketing de desempenho. Depois que o GenStudio para profissionais de marketing de desempenho tiver extraído as informações necessárias dos documentos de diretrizes da marca, você será solicitado a editar ou preencher manualmente os campos das informações extraídas. Especifique áreas de foco de produto individuais para criação de conteúdo adicionando um [!DNL Product]. As diretrizes do [!DNL Personas] ajudam a adaptar a criação de conteúdo para segmentos de clientes definidos.

   Embora a configuração das diretrizes de marca de uma organização possa ser uma ação única, talvez seja necessário revisar e aprimorar essas diretrizes com base na volatilidade, no crescimento e nas mudanças nas circunstâncias do mercado de sua organização.

1. **[Carregar modelos](./content/use-templates.md)**. Os modelos fornecem atalhos e aceleram a criação de conteúdo. Um modelo contém recursos aprovados, como cabeçalhos e rodapés, e estabelece medidas de proteção para a criação de conteúdo. Os administradores normalmente fazem upload e gerenciam modelos para sua organização. Os criadores usam modelos para iniciar rapidamente o processo de criação de conteúdo dentro dos limites estabelecidos da marca organizacional.

1. **[Carregar ativos aprovados](./content/manage-assets.md)**. Os ativos aprovados em [!DNL Content] estão disponíveis para todos os criadores do GenStudio for Performance Marketers. Você pode propagar [!DNL Content] com ativos que os criadores podem usar para criar novas experiências ou ativos.

1. **[Conectar a uma conta Meta (Facebook)](./insights/connect-channel.md)**. Você deve configurar uma conexão entre o GenStudio para profissionais de marketing de desempenho e as contas sociais de sua organização para receber dados de suas campanhas de marketing ativas, ativos e experiências. [[!DNL Insights]](./insights/overview.md) fornece ferramentas para analisar dados derivados de canais.
