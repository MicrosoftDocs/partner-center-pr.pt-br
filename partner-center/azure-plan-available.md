---
title: Serviços do Azure disponíveis no CSP do Azure
description: Esta seção aborda os serviços do Azure que estão e não estão disponíveis no Programa CSP (Provedor de Soluções na Nuvem) do Azure.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: high
ms.date: 05/13/2020
ms.custom: SEOMAY.20
ms.openlocfilehash: dad65d2237a4446bd6a555a600193e7885bc6f5e
ms.sourcegitcommit: 775a13540d6576201a900e517a0696a6ff4897d8
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/05/2020
ms.locfileid: "84458332"
---
# <a name="azure-services-available-in-the-azure-cloud-solution-provider-csp-program"></a>Serviços do Azure disponíveis no programa CSP (Provedor de Soluções de Nuvem) do Azure

**Funções apropriadas**

- Agente administrativo
- Administrador de cobrança
- Administrador global
- Agente de suporte técnico
- Agente de vendas
- Administrador de gerenciamento de usuário

## <a name="available-azure-services-in-azure-csp"></a>Serviços do Azure disponíveis no CSP do Azure

Este artigo lista os serviços do Azure que estão e não estão disponíveis no programa CSP (Provedor de Soluções de Nuvem) do Azure. Também aborda a disponibilidade do serviço nas nuvens nacionais [Microsoft Azure Alemanha](https://azure.microsoft.com/overview/clouds/germany/) e [Microsoft Azure Government](https://azure.microsoft.com/overview/clouds/government/).

>[!Note]
> O [Azure China](https://www.azure.cn/) não está disponível no Programa CSP do Azure.

## <a name="global-cloud"></a>Nuvem global

Todos os serviços com base no modelo do Azure Resource Manager estão disponíveis no Programa CSP.  Os serviços que não são do Azure Resource Manager não estão disponíveis no Programa CSP.  

## <a name="csp-specific-service-configurations"></a>Configurações de serviço específicas do CSP

Os seguintes serviços exigem configurações especiais no CSP:

- [StorSimple](https://docs.microsoft.com/azure/storsimple/storsimple-partner-csp-overview)

- [Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-csp)

- [Cofre da Chave](https://azurecsp.blob.core.windows.net/files/key-vault-in-csp.docx)

- [Azure Time Series Insights](https://azure.microsoft.com/services/time-series-insights/): somente usuários do locatário do cliente podem acessar os dados no ambiente do Time Series Insights. Os parceiros podem gerenciar o ambiente do Time Series Insights do cliente por padrão, mas se precisarem acessar os dados nele, deverão ser adicionados ao locatário do cliente.

## <a name="visual-studio-marketplace"></a>Visual Studio Marketplace

Agora você pode comprar os itens listados abaixo no Visual Studio Marketplace, com exceção de extensões de terceiros.

- [Azure DevOps](https://www.visualstudio.com/team-services/)

- [Assinaturas do Visual Studio](https://www.visualstudio.com/subscriptions/)

- [Treinamento na Xamarin University](https://marketplace.visualstudio.com/items?itemName=ms.xamarin-university)

Para ajudar você a começar, criamos vídeos e documentação sobre [como configurar, comprar e gerenciar o Azure DevOps](https://docs.microsoft.com/vsts/billing/csp/set-up-csp-customer) no CSP.

## <a name="azure-marketplace-items-in-azure-csp"></a>Itens do Azure Marketplace no CSP do Azure

Nem todos os itens do Azure Marketplace estão disponíveis atualmente nas assinaturas do CSP do Azure.

- Serviços do Azure baseados na Microsoft: estão disponíveis. Examine a tabela e os comentários anteriores.

- Itens de BYOL (Traga Sua Própria Licença): estão disponíveis. Uma lista completa de itens do Azure Marketplace habilitados para BYOL está disponível na [página de BYOL do Azure Marketplace](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol).

- Itens de terceiros do Azure Marketplace pagos conforme o uso: estarão disponíveis se o provedor tiver publicado no canal do CSP. Para saber mais, confira [Vender assinaturas para produtos do Azure Marketplace](https://aka.ms/marketplaceincsp).

- Citrix XenApp Essentials: os parceiros podem comprar o XenApp Essentials para clientes no CSP. Para saber mais, confira no blog da Citrix o artigo [A distribuição do XenApp Essentials já está disponível no canal do Provedor de Soluções na Nuvem da Microsoft](https://www.citrix.com/blogs/2018/02/01/xenapp-essentials-now-available-through-microsoft-cloud-solution-provider-channel/) (em inglês).

## <a name="national-clouds"></a>Nuvens nacionais

A tabela a seguir exibe uma lista regularmente atualizada dos produtos, serviços e recursos de terceiros do Azure disponíveis para o CSP em nuvens nacionais.

| Produto, serviço ou recurso do Azure | Governo dos EUA | Alemanha |
| ------ | :-----------: | :-----------: |
|  **Compute**  |    |    |
|  Máquinas virtuais  |  X  |  X  |
|  Serviços de nuvem  |    |    |
|  Conjuntos de dimensionamento de máquinas virtuais  |  X  |  X  |
|  Funções  |    |    |
|  Serviço de Contêiner do Azure  |    |    |
|  **Rede**  |    |    |
|  DNS do Azure  |    |    |
|  Rede de Distribuição de Conteúdo  |    |    |
|  Gerenciador de Tráfego  |    |    |
|  ExpressRoute  |  X  |  X  |
|  Rede Virtual  |  X  |  X  |
|  Balanceador de carga  |  X  |  X  |
|  Gateway de VPN  |  X  |  X  |
|  Gateway de Aplicativo  |  X  |  X  |
|  Observador de Rede  |  X  |  X  |
|  **Armazenamento**  |    |    |
|  Armazenamento  |  X  |  X  |
|  Backup  |  X  |  X  |
|  StorSimple  |    |  X  |
|  Site Recovery  |  X  |  X  |
|  Data Lake Store  |    |    |
|  Managed Disks  |  X  |  X  |
|  **Web + Celular**  |    |    |
|  Serviço de Aplicativo  |  X  |  X  |
|  Serviço de Aplicativo no Linux  |    |  X  |
|  Gerenciamento de API  |  X  |    |
|  Rede de Distribuição de Conteúdo  |    |    |
|  Serviços de Mídia  |  X  |  X  |
|  Hubs de Notificação  |  X  |  X  |
|  Azure Search  |    |    |
|  Recurso de Aplicativos Lógicos do Serviço de Aplicativo do Azure  |    |    |
|  **Contêineres**  |    |    |
|  Serviço de Aplicativo  |  X  |  X  |
|  Serviço de Aplicativo no Linux  |    |  X  |
|  Batch  |  X  |  X  |
|  Registro de Contêiner  |    |    |
|  Instâncias de Contêiner  |    |    |
|  Service Fabric  |  X  |  X  |
|  Serviço de Contêiner  |    |    |
|  **Bancos de dados**  |    |    |
|  Banco de dados do SQL  |  X  |  X  |
|  Azure Cosmos DB  |  X  |  X  |
|  SQL Data Warehouse  |  X  |  X  |
|  Cache Redis  |  X  |  X  |
|  SQL Server Stretch Database  |  X  |  X  |
|  Banco de Dados do Azure para MySQL  |    |    |
|  Banco de Dados do Azure para PostgreSQL  |    |    |
|  **Dados + Análise**  |    |    |
|  Databricks  |    |    |
|  HDInsight  |  X  |  X  |
|  Stream Analytics  |    |  X  |
|  Data Factory  |    |    |
|  Log Analytics  |  X  |    |
|  Catálogo de Dados  |    |    |
|  Data Lake Store  |    |    |
|  Data Lake Analytics  |    |    |
|  Azure Analysis Services  |    |    |
|  Power BI Embedded  |    |    |
|  **IA + Serviços Cognitivos**  |    |    |
|  Machine Learning  |    |  X  |
|  Serviço de Bot do Azure  |    |    |
|  Serviços Cognitivos  |    |    |
|  IA do Lote do Azure  |    |    |
|  **Internet das Coisas**  |    |    |
|  Hub IoT  |  X  |  X  |
|  IoT Central  |    |    |
|  Machine Learning  |    |  X  |
|  Stream Analytics  |    |  X  |
|  Hubs de Eventos  |  X  |  X  |
|  Serviços baseados na Localização  |    |    |
|  Hubs de Notificação  |  X  |  X  |
|  Time Series Insights  |    |    |
|  **Enterprise Integration**  |    |    |
|  StorSimple  |  X  |    |
|  Gerenciamento de API  |    |    |
|  Grade de Eventos  |    |    |
|  Data Factory  |    |    |
|  Service Bus  |  X  |  X  |
|  Catálogo de Dados  |    |    |
|  SQL Server Stretch Database  |    |  X  |
|  Recurso de Aplicativos Lógicos do Serviço de Aplicativo do Azure  |    |    |
|  **Segurança + Identidade**  |    |    |
|  Active Directory do Azure  |  X  |  X  |
|  Azure Active Directory B2C  |    |    |
|  Autenticação Multifator  |    |    |
|  Azure Active Directory Domain Services  |    |    |
|  Key Vault  |  X  |  X  |
|  Central de Segurança  |  X  |  X  |
|  **Ferramentas para desenvolvedores**  |    |    |
|  Visual Studio Team Services  |    |    |
|  Application Insights  |    |    |
|  DevTest Labs  |    |    |
|  Visual Studio App Center  |    |    |
|  Xamarin University  |    |    |
|  **Monitoramento + Gerenciamento**  |    |    |
|  Supervisor  |    |    |
|  Backup  |  X  |  X  |
|  Site Recovery  |  X  |  X  |
|  Agendador  |  X  |  X  |
|  Automação  |  X  |  X  |
|  Log Analytics  |  X  |    |
|  Azure Monitor  |    |    |
|  Aplicativos gerenciados pelo Azure  |    |    |
|  Migrações para Azure  |    |    |
|  Grupos de Gerenciamento  |    |  

## <a name="next-steps"></a>Próximas etapas

- [Saiba mais](https://docs.microsoft.com/azure/cloud-solution-provider/overview/partner-center-overview) sobre os recursos disponíveis para o Azure no Partner Center.

- [Crie](https://docs.microsoft.com/azure/cloud-solution-provider/customer-management/create-new-customer) seu primeiro cliente no CSP do Azure e implante serviços do Azure.
