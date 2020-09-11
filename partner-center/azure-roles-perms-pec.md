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
ms.openlocfilehash: f48774cb830ceb575a84177efb57431afdcb9b25
ms.sourcegitcommit: 5fc28f6f81eaebb84e1faa71848afb504e181f37
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/11/2020
ms.locfileid: "90011736"
---
# <a name="roles-and-permissions-eligible-to-earn-partner-earned-credit"></a>Funções e permissões qualificadas para conquistar crédito ganho de parceiro

As seguintes funções são mapeadas para níveis de permissões que determinam se um parceiro é elegível para créditos de parceiros ganhos.

>[!Important]
>Essas funções e permissões não são as mesmas que as funções e permissões que um usuário precisa para trabalhar no Partner Center.

|**Função**   |**Descrição**   |**PEC elegível**   |
|-----------------|:------------------|:--------------|
|Proprietário  |Você gerencia tudo, incluindo o acesso aos recursos.|Sim|
|Colaborador |Você gerencia tudo, exceto concedendo acesso aos recursos.|Sim|
|Leitor|Você pode exibir tudo, mas não fazer nenhuma alteração|Não|
|ACRDelete|acr delete|Sim|
|ACRImageSigner|signatário de imagem ACR|Sim|
|ACRPull|acr pull|Sim|
|AcrPush|acr push|Sim|
|AcrQuarantineReader|leitor de dados de quarentena acr|Não|
|AcrQuarantineWriter| gravador de dados de quarentena acr|Sim|
|Colaborador de serviço de gerenciamento de API|Pode gerenciar o serviço e as APIs|Sim|
|Função do operador de serviço de gerenciamento da API|Pode gerenciar serviços, mas não as APIs|Sim|
|Função de leitor do Serviço de Gerenciamento de API|Acesso somente leitura ao serviço e APIs|Não|
|Colaborador de componente do Application Insights|Gerencia Application Insights componentes|Sim|
|Depurador de Instantâneos do Application Insights|Concede permissão ao usuário para exibir e baixar os instantâneos de depuração coletados com o Depurador de Instantâneos do Application Insights. Observe que essas permissões não estão incluídas nas funções Proprietário ou Colaborador.|Sim|
Operador do Trabalho de Automação | Criar e gerenciar trabalhos usando runbooks de Automação. | Sim | 
Operador de automação | Os Operadores de Automação podem iniciar, interromper, suspender e retomar trabalhos | Sim | 
Operador de Runbook de Automação | Ler propriedades do Runbook - para poder criar Trabalhos do runbook. | Sim | 
Colaborador do Avere | Pode criar e gerenciar um cluster do Avere vFXT. | Sim | 
Operador do Avere | Usado pelo cluster do Avere vFXT para gerenciar o cluster | Sim | 
Proprietário de Dados de Hubs de Eventos do Azure | Permite acesso completo aos recursos dos Hubs de Eventos do Azure. | Sim | 
Receptor de Dados dos Hubs de Eventos do Azure | Permite acesso de recebimento aos recursos dos Hubs de Eventos do Azure. | Sim | 
Remetente de Dados dos Hubs de Eventos do Azure | Permite acesso de envio aos recursos dos Hubs de Eventos do Azure. | Sim | 
Função de Administrador do Cluster do Serviço de Kubernetes do Azure | Liste a ação de credencial de administrador de cluster. | Sim | 
Função de Usuário do Cluster do Serviço de Kubernetes do Azure | Liste a ação de credencial de usuário de cluster. | Sim | 
Leitor de dados do Azure Mapas (versão prévia) | Concede acesso para ler dados relacionados ao mapa de uma conta do Azure Mapas. | Não | 
Proprietário de Dados de Barramento de Serviço do Azure | Permite acesso completo aos recursos do Barramento de Serviço do Azure. | Sim | 
Receptor de Dados do Barramento de Serviço do Azure | Permite acesso de recebimento aos recursos do Barramento de Serviço do Azure. | Sim | 
Remetente de Dados do Barramento de Serviço do Azure | Permite o acesso de envio aos recursos do Barramento de Serviço do Azure. | Sim | 
Proprietário de registro do Azure Stack | Permite que você gerencie registros do Microsoft Azure Stack. | Sim | 
Colaborador de Backup | Permite que você gerencie o serviço de backup, mas não pode criar cofres e fornecer acesso a outras pessoas | Sim | 
Operador de Backup | Permite que você gerencie serviços de backup, exceto a remoção de backup, a criação de cofres e o fornecimento de acesso a outras pessoas | Sim | 
Leitor de Backup | Pode exibir serviços de backup, mas não pode fazer alterações | Não | 
Leitor de cobrança | Permite o acesso de leitura aos dados de cobrança | Não | 
Colaborador do BizTalk | Permite gerenciar serviços do BizTalk, mas não acessá-los. | Sim | 
Acesso de Nó de Membro do Blockchain (Versão Prévia) | Permite acesso a nós de Membro do Blockchain | Sim | 
Colaborador do Blueprint | Pode gerenciar definições de blueprint, mas não as atribuir. | Sim | 
Operador de Blueprint | Pode atribuir blueprints publicados existentes, mas não pode criar novos blueprints. Observação: isso só funcionará se a atribuição for feita com uma identidade gerenciada atribuída pelo usuário. | Sim | 
Colaborador de ponto de extremidade de CDN | Pode gerenciar os pontos de extremidade de CDN, mas não pode conceder acesso a outros usuários. | Sim | 
Leitor de ponto de extremidade de CDN | Pode exibir os pontos de extremidade de CDN, mas não fazer alterações. | Não | 
Colaborador de perfil de CDN | Pode gerenciar os perfis de CDN e os respectivos pontos de extremidade, mas não pode conceder acesso a outros usuários. | Sim | 
Leitor de perfil de CDN | Pode exibir os perfis de CDN e os respectivos pontos de extremidade, mas não fazer alterações. | Não | 
Colaborador de rede clássica | Permite que você gerencie redes clássicas, mas não acessá-las. | Sim | 
Colaborador da conta de armazenamento clássica | Permite que você gerencie contas de armazenamento clássico, mas não acessá-las. | Sim | 
Função do Serviço de Operador da Chave da Conta de Armazenamento Clássica | Os Operadores da Chave da Conta de Armazenamento Clássica têm permissão para listar e regenerar chaves nas Contas de Armazenamento Clássicas | Sim | 
Colaborador de Máquina Virtual Clássica | Permite gerenciar máquinas virtuais clássicas, mas não o acesso a elas, nem à rede virtual ou conta de armazenamento à qual estão conectadas. | Sim | 
Colaborador dos Serviços Cognitivos | Permite criar, ler, atualizar, excluir e gerenciar chaves dos Serviços Cognitivos. | Sim | 
Leitor de Dados de Serviços Cognitivos (Versão Prévia) | Permite que você leia os dados dos Serviços Cognitivos. | Não | 
Usuário dos Serviços Cognitivos | Permite ler e listar as chaves dos Serviços Cognitivos. | Não | 
Função de leitor de conta do Cosmos DB | Pode ler dados de contas do Azure Cosmos DB. Consulte Colaborador de conta do DocumentDB para gerenciar contas do Azure Cosmos DB. | Não | 
Operador do Cosmos DB | Permite que você gerencie contas do Azure Cosmos DB, mas não acesse os dados nelas. Impede o acesso a chaves de conta e cadeias de conexão. | Sim | 
CosmosBackupOperator | Pode enviar solicitação de restauração de um banco de dados Cosmos DB ou de um contêiner em uma conta | Sim | 
Colaborador do Gerenciamento de Custos | Pode exibir os custos e gerenciar a configuração de custo (por exemplo, orçamentos, exportações) | Sim | 
Leitor do Gerenciamento de Custos | Pode exibir dados e configuração de custos (por exemplo, orçamentos, exportações) | Não | 
Colaborador do Data Box | Permite que você gerencie tudo sob o serviço Data Box exceto fornecer acesso a outras pessoas. | Sim | 
Leitor do Data Box | Permite que você gerencie o serviço do Azure Data Box, exceto a ordem de criação ou edição de detalhes do pedido e fornecer acesso a outras pessoas. | Não | 
Colaborador da fábrica de dados | Cria e gerencia data factories, assim como os recursos filhos neles. | Sim | 
Desenvolvedor do Data Lake Analytics | Permite enviar, monitorar e gerenciar seus próprios trabalhos, mas não criar nem excluir contas do Data Lake Analytics. | Sim | 
Limpador de Dados | Pode limpar os dados de análise | Sim | 
Usuário do DevTest Labs | Permite conectar, iniciar, reiniciar e encerrar as máquinas virtuais no Azure DevTest Labs. | Sim | 
Colaborador de zona DNS | Permite gerenciar zonas DNS e conjuntos de registros no DNS do Azure, mas não permite controlar quem tem acesso a eles. | Sim | 
Colaborador de Conta do DocumentDB | Pode gerenciar contas do Azure Cosmos DB. O Azure Cosmos DB era anteriormente conhecido como DocumentDB. | Sim | 
Colaborador de EventGrid EventSubscription | Permite que você gerencie operações de assinatura de evento EventGrid. | Sim | 
Leitor de EventGrid EventSubscription | Permite que você gerencie operações de assinatura de evento EventGrid. | Não | 
Operador de Cluster do HDInsight | Permite que você leia e modifique as configurações de cluster do HDInsight. | Sim | 
Colaborador dos serviços de domínio do HDInsight | Pode ler, criar, modificar e excluir operações relacionadas aos serviços de domínio necessárias para o Enterprise Security Package do HDInsight | Sim | 
Colaborador de conta do sistemas inteligentes | Permite gerenciar contas do Intelligent Systems, mas não acessá-las. | Sim | 
Colaborador do Key Vault | Permite gerenciar cofres de chaves, mas não acessá-los. | Sim | 
Criador de laboratório | Permite a você criar, gerenciar e excluir os laboratórios gerenciados nas contas de laboratório do Azure. | Sim | 
Colaborador do Log Analytics | O Colaborador do Log Analytics pode ler todos os dados de monitoramento e editar as configurações de monitoramento. A edição das configurações de monitoramento inclui a adição da extensão da VM às VMs, leitura das chaves da conta de armazenamento para poder configurar a coleção de logs do Armazenamento do Microsoft Azure, criação e configuração de contas de Automação, adição de soluções e configuração do diagnóstico do Azure em todos os recursos do Azure. | Sim | 
Leitor do Log Analytics | Um Leitor do Log Analytics pode exibir e pesquisar todos os dados de monitoramento além de exibir as configurações de monitoramento, incluindo a exibição da configuração do diagnóstico do Azure em todos os recursos do Azure. | Não | 
Colaborador de aplicativo lógico | Permite o gerenciamento de aplicativos lógicos, mas você não pode alterar o acesso a eles. | Sim | 
Operador de aplicativo lógico | Permite a leitura, habilitação e desabilitação de aplicativos lógicos, mas você não pode editá-los ou atualizá-los. | Sim | 
Função do Operador de Aplicativos Gerenciado | Permite que você leia e execute as ações nos recursos de aplicativo gerenciado | Sim | 
Leitor de aplicativos gerenciados | Permite ler os recursos de um aplicativo gerenciado e solicitar acesso JIT. | Não | 
Colaborador de Identidade Gerenciada | Criar, ler, atualizar e excluir a identidade atribuída pelo usuário | Sim | 
Operador de Identidade Gerenciada | Ler e atribuir identidade atribuída pelo usuário | Sim | 
Colaborador do Grupo de Gerenciamento | Função de Colaborador do Grupo de Gerenciamento | Sim | 
Leitor do Grupo de Gerenciamento | Função de Leitor do Grupo de Gerenciamento | Não | 
Colaborador de monitoramento | Pode ler todos os dados de monitoramento e editar configurações de monitoramento. Consulte também Introdução às funções, permissões e segurança com o Azure Monitor. | Sim | 
Publicador de Métricas de Monitoramento | Habilita a publicação de métricas com base nos recursos do Azure | Sim | 
Leitor de monitoramento | Pode ler todos os dados de monitoramento (métricas, logs, etc). Consulte também Introdução às funções, permissões e segurança com o Azure Monitor. | Não | 
Colaborador de rede | Permite gerenciar redes, mas não acessá-las. | Sim | 
Colaborador de Conta APM do New Relic | Permite que você gerencie contas e aplicativos do Gerenciamento de desempenho de aplicativos da New Relic, mas não tem acesso a eles. | Sim | 
Acesso a Dados e Leitor | Permite que você exiba tudo, mas não permitirá que exclua ou crie uma conta de armazenamento ou um recurso contido. Ele também permitirá o acesso de leitura/gravação a todos os dados contidos em uma conta de armazenamento por meio de acesso às chaves de conta de armazenamento. | Sim | 
Colaborador do Cache Redis | Permite gerenciar caches Redis, mas não acessá-los. | Sim | 
Colaborador da Política de Recursos (Versão prévia) | (Versão prévia) Os usuários com aterramento da EA, com direitos para criar/modificar a política de recursos, criam um tíquete de suporte e recursos/hierarquia de leitura. | Sim | 
Colaborador de Coleções de Trabalho do Agendador | Permite gerenciar as coleções de trabalhos do Agendador, mas não acessá-las. | Sim | 
Colaborador do Serviço de Pesquisa | Permite gerenciar serviços de pesquisa, mas não acessá-las. | Sim | 
Administrador de Segurança | Na Central de Segurança somente: Pode visualizar as políticas de segurança, estados de segurança, editar políticas de segurança, visualizar alertas e recomendações, ignorar alertas e recomendações | Sim | 
Gerenciador de Segurança (Herdado) | Esta é uma função herdada. Em vez disso, use o Administrador de Segurança | Sim | 
Leitor de segurança | Na Central de Segurança somente: Pode visualizar recomendações e alertas, visualizar políticas de segurança, visualizar estados de segurança, mas não pode fazer alterações | Não | 
Colaborador do Site Recovery | Permite gerenciar o serviço do Azure Site Recovery, exceto a criação de cofre e atribuição de função | Sim | 
Operador do Site Recovery | Permite failover e failback, mas não executa outras operações de gerenciamento do Azure Site Recovery | Sim | 
Leitor do Site Recovery | Permite visualizar o status do Azure Site Recovery, mas não executar outras operações de gerenciamento | Não | 
Colaborador da Conta de Âncoras Espaciais | Permite que você gerencie âncoras espaciais em sua conta, exceto excluí-las | Sim | 
Proprietário da Conta de Âncoras Espaciais | Permite gerenciar âncoras espaciais em sua conta, inclusive excluí-las | Sim | 
Leitor da Conta de Âncoras Espaciais | Permite localizar e ler propriedades de âncoras espaciais em sua conta | Não | 
Colaborador do banco de dados SQL | Permite gerenciar Bancos de Dados SQL, mas não acessá-los. Além disso, não é possível gerenciar as políticas relacionadas à segurança ou respectivos servidores SQL pai. | Sim | 
Colaborador da Instância Gerenciada do SQL | Permite que você gerencie instâncias gerenciadas do SQL e a configuração de rede necessária, mas não pode conceder acesso a outras pessoas. | Sim | 
Gerenciador de Segurança do SQL | Permite você gerenciar as políticas relacionadas à segurança de servidores e bancos de dados SQL, mas não acessá-los. | Sim | 
Colaborador do SQL Server | Permite gerenciar servidores e Bancos de Dados SQL, mas não acessá-los, nem as políticas relacionadas à segurança. | Sim | 
Colaborador da Conta de Armazenamento | Permite o gerenciamento de contas de armazenamento. Fornece acesso à chave de conta, que pode ser usada para acessar dados por meio de autorização de chave compartilhada. | Sim | 
Função do Serviço de Operador da Chave da Conta de Armazenamento | Permite listar e regenerar chaves de acesso da conta de armazenamento. | Sim | 
Colaborador de dados de blob de armazenamento | Ler, gravar e excluir contêineres e blobs de Armazenamento do Azure. Para saber quais ações são necessárias para uma determinada operação de dados, consulte Permissões para chamar blob e operações de dados de fila. | Sim | 
Proprietário de Dados do Blob de Armazenamento | Fornece acesso completo aos dados e contêineres de blob do Armazenamento do Azure, incluindo a atribuição de controle de acesso POSIX. Para saber quais ações são necessárias para uma determinada operação de dados, consulte Permissões para chamar blob e operações de dados de fila. | Sim | 
Leitor de Dados do Blob de Armazenamento | Leia e liste contêineres e blobs do Armazenamento do Azure. Para saber quais ações são necessárias para uma determinada operação de dados, consulte Permissões para chamar blob e operações de dados de fila. | Não | 
Delegador do Blob de Armazenamento | Obtenha uma chave de delegação de usuário, que pode ser usada para criar uma assinatura de acesso compartilhado para um contêiner ou blob que é assinado com as credenciais do Azure AD. Para obter mais informações, consulte Criar uma SAS de delegação de usuário. | Sim | 
Colaborador de Compartilhamento SMB de Dados do Arquivo de Armazenamento | Permite acesso de leitura, gravação e exclusão em compartilhamentos de arquivos de armazenamento do Azure via SMB | Sim | 
Colaborador com Privilégios Elevados do Compartilhamento SMB de Dados do Arquivo de Armazenamento | Permite ler, gravar, excluir e modificar o acesso de permissão NTFS em compartilhamentos de arquivos de armazenamento do Azure via SMB | Sim | 
Leitor de Compartilhamento SMB de Dados do Arquivo de Armazenamento | Permite o acesso de leitura ao compartilhamento de arquivos do Azure por SMB | Não | 
Colaborador de Dados da Fila de Armazenamento | Lê, grava e exclui filas do Armazenamento do Azure e mensagens da fila. Para saber quais ações são necessárias para uma determinada operação de dados, consulte Permissões para chamar blob e operações de dados de fila. | Sim | 
Processador de Mensagens de Dados da Fila de Armazenamento | Espia, recupera e exclui uma mensagem de uma fila de armazenamento do Azure. Para saber quais ações são necessárias para uma determinada operação de dados, consulte Permissões para chamar blob e operações de dados de fila. | Sim | 
Remetente da Mensagem de Dados da Fila de Armazenamento | Adiciona mensagens a uma fila de Armazenamento do Azure. Para saber quais ações são necessárias para uma determinada operação de dados, consulte Permissões para chamar blob e operações de dados de fila. | Sim | 
Leitor de Dados da Fila de Armazenamento | Lê e lista as filas do armazenamento do Azure e as mensagens da fila. Para saber quais ações são necessárias para uma determinada operação de dados, consulte Permissões para chamar blob e operações de dados de fila. | Não | 
Colaborador de solicitação de suporte | Permite criar e gerenciar Solicitações de Suporte | Sim | 
Colaborador do Gerenciador de Tráfego | Permite gerenciar perfis do Gerenciador de Tráfego, mas não permite controlar quem tem acesso a eles. | Sim | 
Administrador de Acesso do Usuário | Permite que você gerencie o acesso do usuário aos recursos do Azure. | Sim | 
Logon de administrador da Máquina Virtual | Máquinas Virtuais do Microsoft Azure no portal e logon como administrador | Sim | 
Colaborador de Máquina Virtual | Permite gerenciar máquinas virtuais, mas não o acesso a elas, nem à rede virtual ou conta de armazenamento à qual estão conectadas. | Sim | 
Logon de usuário da Máquina Virtual | Visualize as Máquinas Virtuais do Microsoft Azure no portal e faça logon como usuário. | Sim | 
Colaborador do Plano de Web | Permite gerenciar os planos da Web para sites, mas não o acesso a eles. | Sim | 
Colaborador do Site | Permite que você gerencie sites (não planos da Web), mas não tem acesso a eles | Sim |
