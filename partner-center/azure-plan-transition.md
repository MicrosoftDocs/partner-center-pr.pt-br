---
title: Transições do cliente para o plano do Azure | Partner Center
ms.topic: article
ms.date: 11/25/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como transferir seus clientes facilmente para o plano do Azure.
author: LauraBrenner
ms.author: labrenne
Keywords: ''
robots: ''
ms.localizationpriority: high
ms.openlocfilehash: d9a283242fb911537004719fd62a58478c511565
ms.sourcegitcommit: c3de2c04d761314116b876ffdd4b2c79641007c1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/24/2020
ms.locfileid: "77567232"
---
# <a name="transition-your-customers-to-azure-plan"></a>Transferir seus clientes para o plano do Azure

**Funções apropriadas**

- Agente administrativo
- Administrador de cobrança
- Administrador global
- Agente de suporte técnico
- Agente de vendas
- Administrador de gerenciamento de usuário

Provedores indiretos e parceiros de cobrança diretos podem fazer a transição para a nova experiência de comércio disponível no Programa CSP (Provedor de Serviços de Nuvem) para o Azure. (Revendedores indiretos precisarão trabalhar por meio dos respectivos provedores indiretos.) Os clientes terão uma maneira simplificada de comprar serviços de nuvem, seja de parceiros, de vendedores da Microsoft ou diretamente na Web.

A funcionalidade de transição é destinada apenas a clientes que estão fazendo a transição para a nova experiência de comércio para o Azure e que assinaram o Contrato de Cliente da Microsoft e não para outras ofertas do CSP, como o Office 365 ou o Dynamics 365.

## <a name="available-azure-services-in-azure-csp"></a>Serviços do Azure disponíveis no CSP do Azure

Esta seção aborda os serviços do Azure que estão e não estão disponíveis no Programa CSP (Provedor de Soluções na Nuvem) do Azure. Também aborda a disponibilidade do serviço nas nuvens nacionais [Microsoft Azure Alemanha](https://azure.microsoft.com/overview/clouds/germany/) e [Microsoft Azure Government](https://azure.microsoft.com/overview/clouds/government/).

>[!Note]
>O [Azure China]( https://www.azure.cn/) não está disponível no Programa CSP do Azure.

### <a name="global-cloud"></a>Nuvem global 

Todos os serviços com base no modelo do Azure Resource Manager estão disponíveis no Programa CSP.  Os serviços que não são do Azure Resource Manager não estão disponíveis no Programa CSP.  

### <a name="csp-specific-service-configurations"></a>Configurações de serviço específicas do CSP

Os seguintes serviços exigem configurações especiais no CSP:

- [StorSimple](https://docs.microsoft.com/azure/storsimple/storsimple-partner-csp-overview)

- [Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-csp)

- [Key Vault](https://azurecsp.blob.core.windows.net/files/key-vault-in-csp.docx) 

- [Azure Time Series Insights](https://azure.microsoft.com/services/time-series-insights/): somente usuários do locatário do cliente podem acessar os dados no ambiente do Time Series Insights. Os parceiros podem gerenciar o ambiente do Time Series Insights do cliente por padrão, mas se precisarem acessar os dados nele, deverão ser adicionados ao locatário do cliente. 

### <a name="visual-studio-marketplace"></a>Visual Studio Marketplace

Agora você pode comprar os itens listados abaixo no Visual Studio Marketplace, com exceção de extensões de terceiros.

- [Azure DevOps](https://www.visualstudio.com/team-services/) 

- [Assinaturas do Visual Studio](https://www.visualstudio.com/subscriptions/)

- [Treinamento na Xamarin University](https://marketplace.visualstudio.com/items?itemName=ms.xamarin-university)

Para ajudar você a começar, criamos vídeos e documentação sobre [como configurar, comprar e gerenciar o Azure DevOps](https://docs.microsoft.com/vsts/billing/csp/set-up-csp-customer) no CSP.

### <a name="azure-marketplace-items-in-azure-csp"></a>Itens do Azure Marketplace no CSP do Azure

Nem todos os itens do Azure Marketplace estão disponíveis atualmente nas assinaturas do CSP do Azure.

- Serviços do Azure baseados na Microsoft: estão disponíveis. Examine a tabela e os comentários anteriores.

- Itens de BYOL (Traga Sua Própria Licença): estão disponíveis. Uma lista completa de itens do Azure Marketplace habilitados para BYOL está disponível na [página de BYOL do Azure Marketplace](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol).

- Itens de terceiros do Azure Marketplace pagos conforme o uso: estarão disponíveis se o provedor tiver publicado no canal do CSP. Para saber mais, confira [Vender assinaturas para produtos do Azure Marketplace](https://aka.ms/marketplaceincsp).   

- Citrix XenApp Essentials: os parceiros podem comprar o XenApp Essentials para clientes no CSP. Para saber mais, confira no blog da Citrix o artigo [A distribuição do XenApp Essentials já está disponível no canal do Provedor de Soluções na Nuvem da Microsoft](https://www.citrix.com/blogs/2018/02/01/xenapp-essentials-now-available-through-microsoft-cloud-solution-provider-channel/) (em inglês).

### <a name="national-clouds"></a>Nuvens nacionais 
A tabela a seguir exibe uma lista regularmente atualizada dos produtos, serviços e recursos de terceiros do Azure disponíveis para o CSP em nuvens nacionais. 

| Produto, serviço ou recurso do Azure | Governo dos EUA | Alemanha |
| ------ | :-----------: | :-----------: |
|  **Computação**  |    |    |
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
|  Banco de dados SQL  |  X  |  X  |
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
|  Barramento de Serviço  |  X  |  X  |
|  Catálogo de Dados  |    |    |
|  SQL Server Stretch Database  |    |  X  |
|  Recurso de Aplicativos Lógicos do Serviço de Aplicativo do Azure  |    |    |
|  **Segurança + Identidade**  |    |    |
|  Azure Active Directory  |  X  |  X  |
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

### <a name="next-steps"></a>Próximas etapas

- [Saiba mais](https://docs.microsoft.com/azure/cloud-solution-provider/overview/partner-center-overview) sobre os recursos disponíveis para o Azure no Partner Center.

- [Crie](https://docs.microsoft.com/azure/cloud-solution-provider/customer-management/create-new-customer) seu primeiro cliente no CSP do Azure e implante serviços do Azure.

## <a name="transition-existing-csp-offers-to-an-azure-plan"></a>Fazer a transição de ofertas do CSP existentes para um plano do Azure

Você pode fazer a transição de um cliente de suas ofertas do CSP do Azure existentes para os serviços do Azure no âmbito do plano do Azure na nova experiência de comércio no programa CSP de dentro do Partner Center. Para fazer isso, o parceiro e o cliente precisam ter uma relação de revendedor estabelecida por meio do Partner Center, e o cliente deve ter assinado o Contrato de Cliente da Microsoft.

### <a name="select-transition-to-azure-plan"></a>Selecione fazer a transição para o plano do Azure

1. Selecione o plano do Azure para o seu cliente.

2. Selecione **Fazer a transição de cobrança para o plano do Azure**.

![transição](images/azure/transition1.png)

3. Selecionar **Continuar**

![transição](images/azure/transition2.png)

Seu cliente será transferido para o plano do Azure.

**O fluxo de trabalho de transição automatiza as etapas de pré-requisito**:

- Compra de plano(s) do Azure
- Um plano por cliente em cenários de CSP direto  
- Um plano por revendedor  

Por exemplo, um parceiro comprou duas ofertas do Microsoft Azure e incluiu duas POR distintas na compra. Nesse caso, o fluxo de trabalho de transição comprará dois planos do Azure (um por revendedor) e mapeará as respectivas assinaturas do Azure nos planos do Azure automaticamente.  

**Como mapear a assinatura do Azure para o plano do Azure**

Após a compra do plano do Azure, nosso sistema mapeará as assinaturas do Azure existentes para os planos do Azure. O progresso pode ser exibido no portal do Azure, bem como no Partner Center. 

4. Volte para a página de **Assinaturas** do Partner Center do cliente a fim de atualizar o limite de orçamento usando a moeda local do cliente. 

![Transição](images/azure/transition3.png)

>[!NOTE]
>O orçamento definido no Partner Center não é transportado para o portal do Azure. Você também deve definir o orçamento e o alerta no portal do Azure.

Ao passar para o plano do Azure, não será mais possível comprar assinaturas do Azure para esse cliente. Você cria as assinaturas no âmbito do plano do Azure, no portal do Azure.

>[!NOTE]
> Todas as assinaturas do Azure adquiridas por meio do RBAC no plano do Azure terão preços na moeda local e serão cobradas nessa mesma moeda. As taxas de câmbio não serão usadas.

### <a name="track-your-transition-details"></a>Acompanhar os detalhes da transição

Siga o progresso da transição no portal do Azure, bem como no Partner Center.

![Mostrar detalhes](images/azure/details1.png)

**Impacto de cobrança para os parceiros**

Se você fizer a transição de um cliente de uma oferta do CSP do Azure existente, você terá os seguintes impactos de cobrança:

- Você será cobrado em sua fatura do CSP existente por todo o uso, até o ponto de saída da assinatura original do CSP do Azure.

- Se você tiver direitos de acesso de administrador à assinatura CSP existente, continuará a ter tal acesso quando essa assinatura for migrada.

Para fazer a transição de Contratos Enterprise diretos para o CSP e o Servidor e os Registros de nuvem para os Serviços do Azure, leia [Obter a propriedade de cobrança das assinaturas do Azure para o Contrato de Parceiro da Microsoft](https://docs.microsoft.com/azure/billing/mpa-request-ownership)

**Log de auditoria**:

Para reconciliar a cobrança, veja seu histórico de assinaturas do "Microsoft Azure" (0145P) na página de **Assinaturas**. 

A assinatura do "Microsoft Azure" (0145P) é composta por duas partes:
1. Assinatura do Commerce 
2. Assinatura do Azure (direito)

Quando a transição for concluída, a assinatura do Azure será movida no novo plano do Azure e a assinatura do Commerce será suspensa para que nenhum uso adicional seja relatado.  

>[Observação]\: Quando a assinatura do Microsoft Azure (0145P) é adquirida no CSP, tanto a assinatura do Commerce quanto a assinatura do Azure (direito) têm o mesmo valor. Somente no caso de alterações ou transferências na propriedade de cobrança é que os valores diferem. 

**Problemas de transição**

Não prevemos nenhum problema durante as transições. Caso ocorra alguma, nós o atualizaremos ao longo do próprio fluxo de trabalho de transição. Não deverá haver distúrbios para o uso do Azure.  

## <a name="next-steps"></a>Próximas etapas

- [Gerenciar assinaturas e recursos no âmbito do plano do Azure](azure-plan-manage.md)

- [Crédito ganho pelo parceiro – visão geral](partner-earned-credit.md)



