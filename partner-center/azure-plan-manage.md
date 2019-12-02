---
title: Gerenciar assinaturas e recursos no âmbito do plano do Azure | Partner Center
ms.topic: article
ms.date: 11/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como os parceiros podem usar diferentes opções de RBAC (controle de acesso baseado em função) para obter controle operacional e gerenciamento dos recursos do Azure de um cliente.
ms.assetid: ''
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: High
ms.openlocfilehash: 15d1fd3bdff078e752f3b3acb9b200300dc2e64b
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253274"
---
# <a name="manage-subscriptions-and-resources-under-the-azure-plan"></a>Gerenciar assinaturas e recursos no âmbito do plano do Azure

Ao fazer a transição de um cliente para o plano do Azure, você recebe direitos de administrador no Azure (direitos de proprietário da assinatura por meio do recurso Administrador em nome de) por padrão.

 > [!NOTE]
 > Os direitos de administrador na assinatura do Azure podem ser removidos pelo cliente no âmbito da assinatura, do grupo de recursos ou da carga de trabalho. 

 Os parceiros podem obter controle operacional 24x7 e gerenciamento dos recursos do Azure de um cliente no CSP usando diferentes opções fornecidas por meio do recurso de RBAC (controle de acesso baseado em função). 

- **AOBO (Administrador em nome de)** – Com o recurso [AOBO](https://channel9.msdn.com/Series/cspdev/Module-11-Admin-On-Behalf-Of-AOBO), qualquer usuário com a função de agente administrativo no locatário do parceiro terá acesso de proprietário do RBAC às assinaturas do Azure que você criar por meio do programa CSP.

- **Azure Lighthouse**: O AOBO não permite a flexibilidade de criar grupos distintos que funcionem com clientes diferentes ou para habilitar funções diferentes para grupos ou usuários. Usando o Azure Lighthouse, você pode atribuir diferentes grupos a diferentes clientes ou funções. Como os usuários terão o nível apropriado de acesso por meio do gerenciamento de recursos delegado do Azure, você poderá reduzir o número de usuários que têm a função de Agente Administrador (e, portanto, ter acesso total por meio do AOBO). Isso ajuda a melhorar a segurança limitando o acesso desnecessário aos recursos de seus clientes. Isso também proporciona mais flexibilidade para gerenciar vários clientes em escala. Para obter mais informações, leia [Azure Lighthouse e o programa Provedor de Soluções na Nuvem](https://docs.microsoft.com/azure/lighthouse/concepts/cloud-solution-provider).

-  **Diretório ou usuários convidados ou [entidades de serviço](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)** : Você pode delegar acesso granular a assinaturas do CSP adicionando usuários no diretório Customer ou adicionando usuários convidados e atribuindo funções RBAC específicas. 

A Microsoft recomenda que os usuários tenham as permissões mínimas necessárias para realizar seu trabalho como uma prática de segurança. Confira [Recursos do Azure Active Directory Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure). 

## <a name="link-your-partner-id-mpn-idto-your-credentials-for-managing-customers-azure-resources"></a>Vincular sua ID de parceiro (ID de MPN) às suas credenciais para gerenciar os recursos do Azure do cliente

A tabela a seguir mostra os métodos usados para associar sua ID de parceiro a várias opções de acesso RBAC.

|**Categoria**   |**Cenário**   |**Associação de ID de MPN**|
|-----------------|:------------------------|:------------------|
|AOBO   |O parceiro direto do CSP ou o provedor indireto cria a assinatura para o cliente, tornando o parceiro direto do CSP ou provedor indireto o proprietário padrão da assinatura por meio do AOBO. O parceiro direto do CSP ou o provedor indireto concede acesso indireto ao revendedor à assinatura usando o AOBO.|Automático (não requer esforço do parceiro)|
|Azure Lighthouse|O parceiro cria uma nova [oferta de Serviços Gerenciados no Marketplace](https://docs.microsoft.com/azure/lighthouse/concepts/managed-services-offers). Esta oferta é aceita na assinatura do CSP e o parceiro obtém acesso à assinatura do CSP.|Automático (não requer esforço do parceiro)|
|Azure Lighthouse|O parceiro implanta o [modelo ARM](https://docs.microsoft.com/azure/lighthouse/how-to/onboard-customer) na assinatura do Azure|O parceiro precisa associar a ID do MPN ao usuário ou à entidade de serviço no locatário do parceiro. Para obter mais informações – [Vincular ID do Parceiro](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started).|
|Diretório ou usuário convidado|O parceiro cria um novo usuário ou entidade de serviço no diretório do cliente e fornece acesso à assinatura do CSP para o usuário. O parceiro cria um novo usuário ou entidade de serviço no diretório do cliente. O parceiro adiciona o usuário a um grupo e dá acesso à assinatura do CSP para o grupo.|O parceiro precisa associar a ID do MPN ao usuário ou à entidade de serviço no locatário do cliente. Para obter mais informações – [Vincular ID do Parceiro](https://docs.microsoft.com/azure/billing/billing-partner-admin-link-started).|

## <a name="confirm-that-you-have-admin-access"></a>Confirme se você tem acesso de administrador

Você precisa de acesso de administrador para gerenciar os serviços do cliente e receber créditos ganhos. Leia [Créditos ganhos pelo parceiro](partner-earned-credit.md) para obter informações detalhadas sobre os créditos ganhos. Você tem duas maneiras de garantir que tem acesso de administrador.

- Examinar o arquivo de uso diário – isso pode ser determinado examinando o preço unitário e o preço unitário efetivo no arquivo de uso diário e confirmando se existe um desconto sendo aplicado. Se estiver recebendo o desconto, significa que você é o administrador.

- Criar um alerta do Azure monitor – você pode criar um [alerta](https://docs.microsoft.com/azure/azure-monitor/platform/alerts-activity-log) no log de atividades do Azure Monitor para ser notificado quando o seu acesso RBAC for removido da assinatura do CSP.

### <a name="create-an-azure-monitor-alert"></a>Criar um alerta no Azure Monitor

1. Criar alerta.

![alerta do azure](images/azure/azurealert1.png)

2. Selecione o tipo de ação que deseja que o alerta execute. Por exemplo, se especificar que deseja um email, você receberá um email de notificação se ocorrer alguma exclusão de atribuição de função.

![configurar alerta](images/azure/azureconfigurealert2.png)

### <a name="aobo-removal"></a>Remoção do AOBO

Os clientes podem gerenciar o acesso às suas assinaturas por meio do **Controle de Acesso**, no portal do Azure. Na guia **Atribuições de função**, eles selecionam **Remover acesso**. Se isso acontecer, você poderá:

- Conversar com seu cliente para ver se o acesso de administrador pode ser restabelecido.
- Use o acesso fornecido por meio do [RBAC (controle de acesso baseado em função)](https://docs.microsoft.com/azure/role-based-access-control/overview).
- Use o acesso fornecido por meio do [Azure Lighthouse](https://azure.microsoft.com/services/azure-lighthouse/).

O acesso baseado em função difere do acesso de administrador. As funções delimitam com precisão o que você pode ou não pode fazer. O acesso de administrador é mais amplo.

Para ver as funções qualificadas para obter o PEC, leia [Funções e permissões para o crédito ganho pelo parceiro](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QuW2).




**Para saber mais**

- [Revogar e restabelecer privilégios de administrador para assinaturas do Azure CSP](revoke-reinstate-csp.md)

- [Crédito ganho pelo parceiro – visão geral](partner-earned-credit.md)

- [Crédito ganho pelo parceiro para serviços gerenciados](partner-earned-credit-explanation.md)