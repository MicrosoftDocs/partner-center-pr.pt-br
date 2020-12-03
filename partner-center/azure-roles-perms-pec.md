---
title: Funções, permissões para crédito de parceiro ganho
ms.topic: article
ms.date: 05/04/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba mais sobre as funções e permissões para que os parceiros possam obter os créditos acumulados do parceiro (PEC). Elas diferem das funções para trabalhar no Partner Center.
author: adamyeh
ms.author: adamyeh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8c36883dc7d12b7ea0ce8f2644dbac86595ab131
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534583"
---
# <a name="roles-and-permissions-required-to-earn-partner-earned-credit"></a>Funções e permissões necessárias para ganhar crédito de parceiro Obtido

As seguintes funções são mapeadas para níveis de permissões que determinam se um parceiro é elegível para créditos de parceiros ganhos.

>[!Important]
>Essas funções e permissões não são as mesmas que as funções e permissões que um usuário precisa para trabalhar no Partner Center.

|**Função**   |**Descrição**   |**PEC elegível**   |
|-----------------|:------------------|:--------------|
|Proprietário  |Você gerencia tudo, incluindo o acesso aos recursos.|Yes|
|Colaborador |Você gerencia tudo, exceto concedendo acesso aos recursos.|Yes|
|Leitor|Você pode exibir tudo, mas não fazer nenhuma alteração|No|
|ACRDelete|acr delete|Yes|
|ACRImageSigner|signatário de imagem ACR|Yes|
|ACRPull|acr pull|Yes|
|AcrPush|acr push|Yes|
|AcrQuarantineReader|leitor de dados de quarentena acr|No|
|AcrQuarantineWriter| gravador de dados de quarentena acr|Yes|
|Colaborador de serviço de gerenciamento de API|Pode gerenciar o serviço e as APIs|Yes|
|Função do operador de serviço de gerenciamento da API|Pode gerenciar serviços, mas não as APIs|Yes|
|Função de leitor do Serviço de Gerenciamento de API|Acesso somente leitura ao serviço e APIs|No|
|Colaborador de componente do Application Insights|Gerencia Application Insights componentes|Yes|
|Depurador de Instantâneos do Application Insights|Concede permissão ao usuário para exibir e baixar os instantâneos de depuração coletados com o Depurador de Instantâneos do Application Insights. Observe que essas permissões não estão incluídas nas funções Proprietário ou Colaborador.|Yes|
Operador do Trabalho de Automação | Criar e gerenciar trabalhos usando runbooks de Automação. | Yes | 
Operador de automação | Os Operadores de Automação podem iniciar, interromper, suspender e retomar trabalhos | Yes | 
Operador de Runbook de Automação | Ler propriedades do Runbook - para poder criar Trabalhos do runbook. | Yes | 
Colaborador do Avere | Pode criar e gerenciar um cluster do Avere vFXT. | Yes | 
Operador do Avere | Usado pelo cluster do Avere vFXT para gerenciar o cluster | Yes | 
Proprietário de Dados de Hubs de Eventos do Azure | Permite acesso completo aos recursos dos Hubs de Eventos do Azure. | Yes | 
Receptor de Dados dos Hubs de Eventos do Azure | Permite acesso de recebimento aos recursos dos Hubs de Eventos do Azure. | Yes | 
Remetente de Dados dos Hubs de Eventos do Azure | Permite acesso de envio aos recursos dos Hubs de Eventos do Azure. | Yes | 
Função de Administrador do Cluster do Serviço de Kubernetes do Azure | Liste a ação de credencial de administrador de cluster. | Yes | 
Função de Usuário do Cluster do Serviço de Kubernetes do Azure | Liste a ação de credencial de usuário de cluster. | Yes | 
Leitor de dados do Azure Mapas (versão prévia) | Concede acesso para ler dados relacionados ao mapa de uma conta do Azure Mapas. | No | 
Proprietário de Dados de Barramento de Serviço do Azure | Permite acesso completo aos recursos do Barramento de Serviço do Azure. | Yes | 
Receptor de Dados do Barramento de Serviço do Azure | Permite acesso de recebimento aos recursos do Barramento de Serviço do Azure. | Yes | 
Remetente de Dados do Barramento de Serviço do Azure | Permite o acesso de envio aos recursos do Barramento de Serviço do Azure. | Yes | 
Proprietário de registro do Azure Stack | Permite que você gerencie registros do Microsoft Azure Stack. | Yes | 
Colaborador de Backup | Permite que você gerencie o serviço de backup, mas não pode criar cofres e fornecer acesso a outras pessoas | Yes | 
Operador de Backup | Permite que você gerencie serviços de backup, exceto a remoção de backup, a criação de cofres e o fornecimento de acesso a outras pessoas | Yes | 
Leitor de Backup | Pode exibir serviços de backup, mas não pode fazer alterações | No | 
Leitor de cobrança | Permite o acesso de leitura aos dados de cobrança | No | 
Colaborador do BizTalk | Permite gerenciar serviços do BizTalk, mas não acessá-los. | Yes | 
Acesso de Nó de Membro do Blockchain (Versão Prévia) | Permite acesso a nós de Membro do Blockchain | Yes | 
Colaborador do Blueprint | Pode gerenciar definições de blueprint, mas não as atribuir. | Yes | 
Operador de Blueprint | Pode atribuir blueprints publicados existentes, mas não pode criar novos blueprints. Observação: isso só funcionará se a atribuição for feita com uma identidade gerenciada atribuída pelo usuário. | Yes | 
Colaborador de ponto de extremidade de CDN | Pode gerenciar os pontos de extremidade de CDN, mas não pode conceder acesso a outros usuários. | Yes | 
Leitor de ponto de extremidade de CDN | Pode exibir os pontos de extremidade de CDN, mas não fazer alterações. | No | 
Colaborador de perfil de CDN | Pode gerenciar os perfis de CDN e os respectivos pontos de extremidade, mas não pode conceder acesso a outros usuários. | Yes | 
Leitor de perfil de CDN | Pode exibir os perfis de CDN e os respectivos pontos de extremidade, mas não fazer alterações. | No | 
Colaborador de rede clássica | Permite que você gerencie redes clássicas, mas não acessá-las. | Yes | 
Colaborador da conta de armazenamento clássica | Permite que você gerencie contas de armazenamento clássico, mas não acessá-las. | Yes | 
Função do Serviço de Operador da Chave da Conta de Armazenamento Clássica | Os Operadores da Chave da Conta de Armazenamento Clássica têm permissão para listar e regenerar chaves nas Contas de Armazenamento Clássicas | Yes | 
Colaborador de Máquina Virtual Clássica | Permite gerenciar máquinas virtuais clássicas, mas não o acesso a elas, nem à rede virtual ou conta de armazenamento à qual estão conectadas. | Yes | 
Colaborador dos Serviços Cognitivos | Permite criar, ler, atualizar, excluir e gerenciar chaves dos Serviços Cognitivos. | Yes | 
Leitor de Dados de Serviços Cognitivos (Versão Prévia) | Permite que você leia os dados dos Serviços Cognitivos. | No | 
Usuário dos Serviços Cognitivos | Permite ler e listar as chaves dos Serviços Cognitivos. | No | 
Função de leitor de conta do Cosmos DB | Pode ler dados de contas do Azure Cosmos DB. Consulte Colaborador de conta do DocumentDB para gerenciar contas do Azure Cosmos DB. | No | 
Operador do Cosmos DB | Permite que você gerencie contas do Azure Cosmos DB, mas não acesse os dados nelas. Impede o acesso a chaves de conta e cadeias de conexão. | Yes | 
CosmosBackupOperator | Pode enviar solicitação de restauração de um banco de dados Cosmos DB ou de um contêiner em uma conta | Yes | 
Colaborador do Gerenciamento de Custos | Pode exibir os custos e gerenciar a configuração de custo (por exemplo, orçamentos, exportações) | Yes | 
Leitor do Gerenciamento de Custos | Pode exibir dados e configuração de custos (por exemplo, orçamentos, exportações) | No | 
Colaborador do Data Box | Permite que você gerencie tudo sob o serviço Data Box exceto fornecer acesso a outras pessoas. | Yes | 
Leitor do Data Box | Permite que você gerencie o serviço do Azure Data Box, exceto a ordem de criação ou edição de detalhes do pedido e fornecer acesso a outras pessoas. | No | 
Colaborador da fábrica de dados | Cria e gerencia data factories, assim como os recursos filhos neles. | Yes | 
Desenvolvedor do Data Lake Analytics | Permite enviar, monitorar e gerenciar seus próprios trabalhos, mas não criar nem excluir contas do Data Lake Analytics. | Yes | 
Limpador de Dados | Pode limpar os dados de análise | Yes | 
Usuário do DevTest Labs | Permite conectar, iniciar, reiniciar e encerrar as máquinas virtuais no Azure DevTest Labs. | Yes | 
Colaborador de zona DNS | Permite gerenciar zonas DNS e conjuntos de registros no DNS do Azure, mas não permite controlar quem tem acesso a eles. | Yes | 
Colaborador de Conta do DocumentDB | Pode gerenciar contas do Azure Cosmos DB. O Azure Cosmos DB era anteriormente conhecido como DocumentDB. | Yes | 
Colaborador de EventGrid EventSubscription | Permite que você gerencie operações de assinatura de evento EventGrid. | Yes | 
Leitor de EventGrid EventSubscription | Permite que você gerencie operações de assinatura de evento EventGrid. | No | 
Operador de Cluster do HDInsight | Permite que você leia e modifique as configurações de cluster do HDInsight. | Yes | 
Colaborador dos serviços de domínio do HDInsight | Pode ler, criar, modificar e excluir operações relacionadas aos serviços de domínio necessárias para o Enterprise Security Package do HDInsight | Yes | 
Colaborador de conta do sistemas inteligentes | Permite gerenciar contas do Intelligent Systems, mas não acessá-las. | Yes | 
Colaborador do Key Vault | Permite gerenciar cofres de chaves, mas não acessá-los. | Yes | 
Criador de laboratório | Permite a você criar, gerenciar e excluir os laboratórios gerenciados nas contas de laboratório do Azure. | Yes | 
Colaborador do Log Analytics | O Colaborador do Log Analytics pode ler todos os dados de monitoramento e editar as configurações de monitoramento. A edição das configurações de monitoramento inclui a adição da extensão da VM às VMs, leitura das chaves da conta de armazenamento para poder configurar a coleção de logs do Armazenamento do Microsoft Azure, criação e configuração de contas de Automação, adição de soluções e configuração do diagnóstico do Azure em todos os recursos do Azure. | Yes | 
Leitor do Log Analytics | Um Leitor do Log Analytics pode exibir e pesquisar todos os dados de monitoramento além de exibir as configurações de monitoramento, incluindo a exibição da configuração do diagnóstico do Azure em todos os recursos do Azure. | No | 
Colaborador de aplicativo lógico | Permite o gerenciamento de aplicativos lógicos, mas você não pode alterar o acesso a eles. | Yes | 
Operador de aplicativo lógico | Permite a leitura, habilitação e desabilitação de aplicativos lógicos, mas você não pode editá-los ou atualizá-los. | Yes | 
Função do Operador de Aplicativos Gerenciado | Permite que você leia e execute as ações nos recursos de aplicativo gerenciado | Yes | 
Leitor de aplicativos gerenciados | Permite ler os recursos de um aplicativo gerenciado e solicitar acesso JIT. | No | 
Colaborador de Identidade Gerenciada | Criar, ler, atualizar e excluir a identidade atribuída pelo usuário | Yes | 
Operador de Identidade Gerenciada | Ler e atribuir identidade atribuída pelo usuário | Yes | 
Colaborador do Grupo de Gerenciamento | Função de Colaborador do Grupo de Gerenciamento | Yes | 
Leitor do Grupo de Gerenciamento | Função de Leitor do Grupo de Gerenciamento | No | 
Colaborador de monitoramento | Pode ler todos os dados de monitoramento e editar configurações de monitoramento. Consulte também Introdução às funções, permissões e segurança com o Azure Monitor. | Yes | 
Publicador de Métricas de Monitoramento | Habilita a publicação de métricas com base nos recursos do Azure | Yes | 
Leitor de monitoramento | Pode ler todos os dados de monitoramento (métricas, logs, etc). Consulte também Introdução às funções, permissões e segurança com o Azure Monitor. | No | 
Colaborador de rede | Permite gerenciar redes, mas não acessá-las. | Yes | 
Colaborador de Conta APM do New Relic | Permite que você gerencie contas e aplicativos do Gerenciamento de desempenho de aplicativos da New Relic, mas não tem acesso a eles. | Yes | 
Acesso a Dados e Leitor | Permite que você exiba tudo, mas não permitirá que exclua ou crie uma conta de armazenamento ou um recurso contido. Ele também permitirá o acesso de leitura/gravação a todos os dados contidos em uma conta de armazenamento por meio de acesso às chaves de conta de armazenamento. | Yes | 
Colaborador do Cache Redis | Permite gerenciar caches Redis, mas não acessá-los. | Yes | 
Colaborador da Política de Recursos (Versão prévia) | (Versão prévia) Os usuários com aterramento da EA, com direitos para criar/modificar a política de recursos, criam um tíquete de suporte e recursos/hierarquia de leitura. | Yes | 
Colaborador de Coleções de Trabalho do Agendador | Permite gerenciar as coleções de trabalhos do Agendador, mas não acessá-las. | Yes | 
Colaborador do Serviço de Pesquisa | Permite gerenciar serviços de pesquisa, mas não acessá-las. | Yes | 
Administrador de Segurança | Na Central de Segurança somente: Pode visualizar as políticas de segurança, estados de segurança, editar políticas de segurança, visualizar alertas e recomendações, ignorar alertas e recomendações | Yes | 
Gerenciador de Segurança (Herdado) | Esta é uma função herdada. Em vez disso, use o Administrador de Segurança | Yes | 
Leitor de segurança | Na Central de Segurança somente: Pode visualizar recomendações e alertas, visualizar políticas de segurança, visualizar estados de segurança, mas não pode fazer alterações | No | 
Colaborador do Site Recovery | Permite gerenciar o serviço do Azure Site Recovery, exceto a criação de cofre e atribuição de função | Yes | 
Operador do Site Recovery | Permite failover e failback, mas não executa outras operações de gerenciamento do Azure Site Recovery | Yes | 
Leitor do Site Recovery | Permite visualizar o status do Azure Site Recovery, mas não executar outras operações de gerenciamento | No | 
Colaborador da Conta de Âncoras Espaciais | Permite que você gerencie âncoras espaciais em sua conta, exceto excluí-las | Yes | 
Proprietário da Conta de Âncoras Espaciais | Permite gerenciar âncoras espaciais em sua conta, inclusive excluí-las | Yes | 
Leitor da Conta de Âncoras Espaciais | Permite localizar e ler propriedades de âncoras espaciais em sua conta | No | 
Colaborador do banco de dados SQL | Permite gerenciar Bancos de Dados SQL, mas não acessá-los. Além disso, não é possível gerenciar as políticas relacionadas à segurança ou respectivos servidores SQL pai. | Yes | 
Colaborador da Instância Gerenciada do SQL | Permite que você gerencie instâncias gerenciadas do SQL e a configuração de rede necessária, mas não pode conceder acesso a outras pessoas. | Yes | 
Gerenciador de Segurança do SQL | Permite você gerenciar as políticas relacionadas à segurança de servidores e bancos de dados SQL, mas não acessá-los. | Yes | 
Colaborador do SQL Server | Permite gerenciar servidores e Bancos de Dados SQL, mas não acessá-los, nem as políticas relacionadas à segurança. | Yes | 
Colaborador da Conta de Armazenamento | Permite o gerenciamento de contas de armazenamento. Fornece acesso à chave de conta, que pode ser usada para acessar dados por meio de autorização de chave compartilhada. | Yes | 
Função do Serviço de Operador da Chave da Conta de Armazenamento | Permite listar e regenerar chaves de acesso da conta de armazenamento. | Yes | 
Colaborador de dados de blob de armazenamento | Ler, gravar e excluir contêineres e blobs de Armazenamento do Azure. Para saber quais ações são necessárias para uma determinada operação de dados, consulte Permissões para chamar blob e operações de dados de fila. | Yes | 
Proprietário de Dados do Blob de Armazenamento | Fornece acesso completo aos dados e contêineres de blob do Armazenamento do Azure, incluindo a atribuição de controle de acesso POSIX. Para saber quais ações são necessárias para uma determinada operação de dados, consulte Permissões para chamar blob e operações de dados de fila. | Yes | 
Leitor de Dados do Blob de Armazenamento | Leia e liste contêineres e blobs do Armazenamento do Azure. Para saber quais ações são necessárias para uma determinada operação de dados, consulte Permissões para chamar blob e operações de dados de fila. | No | 
Delegador do Blob de Armazenamento | Obtenha uma chave de delegação de usuário, que pode ser usada para criar uma assinatura de acesso compartilhado para um contêiner ou blob que é assinado com as credenciais do Azure AD. Para obter mais informações, consulte Criar uma SAS de delegação de usuário. | Yes | 
Colaborador de Compartilhamento SMB de Dados do Arquivo de Armazenamento | Permite acesso de leitura, gravação e exclusão em compartilhamentos de arquivos de armazenamento do Azure via SMB | Yes | 
Colaborador com Privilégios Elevados do Compartilhamento SMB de Dados do Arquivo de Armazenamento | Permite ler, gravar, excluir e modificar o acesso de permissão NTFS em compartilhamentos de arquivos de armazenamento do Azure via SMB | Yes | 
Leitor de Compartilhamento SMB de Dados do Arquivo de Armazenamento | Permite o acesso de leitura ao compartilhamento de arquivos do Azure por SMB | No | 
Colaborador de Dados da Fila de Armazenamento | Lê, grava e exclui filas do Armazenamento do Azure e mensagens da fila. Para saber quais ações são necessárias para uma determinada operação de dados, consulte Permissões para chamar blob e operações de dados de fila. | Yes | 
Processador de Mensagens de Dados da Fila de Armazenamento | Espia, recupera e exclui uma mensagem de uma fila de armazenamento do Azure. Para saber quais ações são necessárias para uma determinada operação de dados, consulte Permissões para chamar blob e operações de dados de fila. | Yes | 
Remetente da Mensagem de Dados da Fila de Armazenamento | Adiciona mensagens a uma fila de Armazenamento do Azure. Para saber quais ações são necessárias para uma determinada operação de dados, consulte Permissões para chamar blob e operações de dados de fila. | Yes | 
Leitor de Dados da Fila de Armazenamento | Lê e lista as filas do armazenamento do Azure e as mensagens da fila. Para saber quais ações são necessárias para uma determinada operação de dados, consulte Permissões para chamar blob e operações de dados de fila. | No | 
Colaborador de solicitação de suporte | Permite criar e gerenciar Solicitações de Suporte | Yes | 
Colaborador do Gerenciador de Tráfego | Permite gerenciar perfis do Gerenciador de Tráfego, mas não permite controlar quem tem acesso a eles. | Yes | 
Administrador de Acesso do Usuário | Permite que você gerencie o acesso do usuário aos recursos do Azure. | Yes | 
Logon de administrador da Máquina Virtual | Máquinas Virtuais do Microsoft Azure no portal e logon como administrador | Yes | 
Colaborador de Máquina Virtual | Permite gerenciar máquinas virtuais, mas não o acesso a elas, nem à rede virtual ou conta de armazenamento à qual estão conectadas. | Yes | 
Logon de usuário da Máquina Virtual | Visualize as Máquinas Virtuais do Microsoft Azure no portal e faça logon como usuário. | Yes | 
Colaborador do Plano de Web | Permite gerenciar os planos da Web para sites, mas não o acesso a eles. | Yes | 
Colaborador do Site | Permite que você gerencie sites (não planos da Web), mas não tem acesso a eles | Sim |

## <a name="next-steps"></a>Próximas etapas

- [Crédito ganho pelo parceiro – uma visão geral sobre como ele funciona na nova experiência de comércio no CSP](partner-earned-credit.md)
