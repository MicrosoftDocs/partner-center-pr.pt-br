---
title: Reservas do Azure & assinaturas de servidor
ms.topic: article
ms.date: 08/06/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba mais sobre as oportunidades do provedor de soluções na nuvem para adquirir, provisionar e gerenciar reservas do Azure e assinaturas de servidor para clientes.
author: rbars
ms.author: rbars
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5b8a9cf07f8dace47346c68ade3707d6b12a1532
ms.sourcegitcommit: b79504dbfc335aca995f370e15a654829acdaaff
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/06/2020
ms.locfileid: "87900092"
---
# <a name="acquire-provision--manage-azure-reserved-vm-instances-ri--server-subscriptions-for-customers"></a><span data-ttu-id="fc8a9-103">Adquirir, provisionar & gerenciar instâncias de VM reservadas do Azure (RI) + assinaturas de servidor para clientes</span><span class="sxs-lookup"><span data-stu-id="fc8a9-103">Acquire, provision, & manage Azure reserved VM instances (RI) + server subscriptions for customers</span></span>

<span data-ttu-id="fc8a9-104">Aplica-se a:</span><span class="sxs-lookup"><span data-stu-id="fc8a9-104">Applies to:</span></span>

- <span data-ttu-id="fc8a9-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="fc8a9-105">Partner Center</span></span>

<span data-ttu-id="fc8a9-106">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="fc8a9-106">**Appropriate roles**</span></span>

- <span data-ttu-id="fc8a9-107">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="fc8a9-107">Admin agent</span></span>
- <span data-ttu-id="fc8a9-108">Administrador global</span><span class="sxs-lookup"><span data-stu-id="fc8a9-108">Global admin</span></span>
- <span data-ttu-id="fc8a9-109">Agente de suporte técnico</span><span class="sxs-lookup"><span data-stu-id="fc8a9-109">Helpdesk agent</span></span>
- <span data-ttu-id="fc8a9-110">Agente de vendas</span><span class="sxs-lookup"><span data-stu-id="fc8a9-110">Sales agent</span></span>
- <span data-ttu-id="fc8a9-111">Administrador de gerenciamento de usuário</span><span class="sxs-lookup"><span data-stu-id="fc8a9-111">User management admin</span></span>

> [!NOTE]
> <span data-ttu-id="fc8a9-112">Este artigo se aplica somente a parceiros no programa CSP (provedor de soluções na nuvem).</span><span class="sxs-lookup"><span data-stu-id="fc8a9-112">This article applies only to partners in the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="fc8a9-113">Os clientes que usam outros tipos de assinaturas (como pagamento conforme o uso, individuais, contrato de cliente da Microsoft ou assinaturas de Enterprise Agreement) devem ler [essa documentação de reservas do Azure](https://docs.microsoft.com/azure/cost-management-billing/reservations).</span><span class="sxs-lookup"><span data-stu-id="fc8a9-113">Customers using other types of subscriptions (such as, pay-as-you-go, individual, Microsoft Customer Agreement, or Enterprise Agreement subscriptions) should instead read [this Azure reservations documentation](https://docs.microsoft.com/azure/cost-management-billing/reservations).</span></span>


## <a name="what-are-azure-reservations"></a><span data-ttu-id="fc8a9-114">O que são Reservas do Azure?</span><span class="sxs-lookup"><span data-stu-id="fc8a9-114">What are Azure Reservations?</span></span>

<span data-ttu-id="fc8a9-115">As reservas do Azure ajudam você a economizar dinheiro ao pagar por um ou três anos de máquina virtual, capacidade de computação do banco de dados SQL, taxa de transferência de Azure Cosmos DB ou outros recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="fc8a9-115">Azure Reservations help you save money by pre-paying for one-year or three-years of virtual machine, SQL Database compute capacity, Azure Cosmos DB throughput, or other Azure resources.</span></span> <span data-ttu-id="fc8a9-116">Pagar previamente permite que você obtenha um desconto nos recursos que você usar.</span><span class="sxs-lookup"><span data-stu-id="fc8a9-116">Pre-paying allows you to get a discount on the resources you use.</span></span> <span data-ttu-id="fc8a9-117">As reservas podem reduzir significativamente sua máquina virtual, computação do banco de dados SQL, Azure Cosmos DB e outros custos de recursos de até 72% em comparação com os preços pagos conforme o uso.</span><span class="sxs-lookup"><span data-stu-id="fc8a9-117">Reservations can significantly reduce your virtual machine, SQL database compute, Azure Cosmos DB, and other resource costs up to 72% compared to pay-as-you-go prices.</span></span> <span data-ttu-id="fc8a9-118">As reservas fornecem um desconto de cobrança e não afetam o estado de runtime dos recursos.</span><span class="sxs-lookup"><span data-stu-id="fc8a9-118">Reservations provide a billing discount and don't affect the runtime state of your resources.</span></span> <span data-ttu-id="fc8a9-119">Para obter mais informações, consulte [o que são as reservas do Azure?](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)</span><span class="sxs-lookup"><span data-stu-id="fc8a9-119">For more information see [What are Azure Reservations?](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations)</span></span>

## <a name="why-should-customers-buy-a-reservation"></a><span data-ttu-id="fc8a9-120">Por que os clientes devem comprar uma reserva?</span><span class="sxs-lookup"><span data-stu-id="fc8a9-120">Why should customers buy a reservation?</span></span>

<span data-ttu-id="fc8a9-121">Se os clientes tiverem máquinas virtuais, Azure Cosmos DB ou bancos de dados SQL executados por longos períodos de tempo, a compra de uma reserva lhes dará a opção mais econômica.</span><span class="sxs-lookup"><span data-stu-id="fc8a9-121">If customers have virtual machines, Azure Cosmos DB or SQL databases that run for long periods of time, purchasing a reservation gives them the most cost-effective option.</span></span> <span data-ttu-id="fc8a9-122">Por exemplo, se um cliente executar continuamente quatro instâncias de um serviço sem uma reserva, elas serão cobradas de acordo com as tarifas pagas conforme o uso.</span><span class="sxs-lookup"><span data-stu-id="fc8a9-122">For example, if a customer continuously runs four instances of a service without a reservation, they are charged at pay-as-you-go rates.</span></span> <span data-ttu-id="fc8a9-123">Se eles comprarem uma reserva para esses recursos, eles receberão imediatamente o desconto de reserva.</span><span class="sxs-lookup"><span data-stu-id="fc8a9-123">If they purchase a reservation for those resources, they immediately get the reservation discount.</span></span> <span data-ttu-id="fc8a9-124">Os recursos não serão mais cobrados com base nas taxas pagas conforme o uso.</span><span class="sxs-lookup"><span data-stu-id="fc8a9-124">The resources are no longer charged at the pay-as-you-go rates.</span></span>

### <a name="compelling-new-azure-offer-in-csp"></a><span data-ttu-id="fc8a9-125">Nova oferta atraente do Azure no CSP</span><span class="sxs-lookup"><span data-stu-id="fc8a9-125">Compelling New Azure offer in CSP</span></span>

<span data-ttu-id="fc8a9-126">Ao trazer as reservas do Azure e as assinaturas de servidor para seu programa CSP, a Microsoft está melhorando seus parceiros para atender à demanda de clientes de crescimento rápido para soluções mais econômicas para dar suporte a cargas de trabalho de nuvem persistentes e altamente previsíveis.</span><span class="sxs-lookup"><span data-stu-id="fc8a9-126">By bringing Azure Reservations and Server Subscriptions to its CSP program, Microsoft is better enabling its partners to address fast-growing customer demand for more cost-effective solutions to support highly predictable, persistent cloud workloads.</span></span> <span data-ttu-id="fc8a9-127">O programa CSP permite que os parceiros adquiram, provisionem e gerenciem reservas do Azure e assinaturas de servidor em nome de clientes comerciais por meio do Microsoft Partner Center e portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="fc8a9-127">The CSP program enables partners to acquire, provision and manage Azure Reservations and Server Subscriptions on behalf of commercial customers via Microsoft Partner Center and Azure portal.</span></span>

<span data-ttu-id="fc8a9-128">Até mesmo daremos aos parceiros em nossas opções do programa CSP sobre como as reservas do Azure podem ser adquiridas.</span><span class="sxs-lookup"><span data-stu-id="fc8a9-128">We even give partners in our CSP program choices about how Azure reservations can be purchased.</span></span> <span data-ttu-id="fc8a9-129">Os parceiros CSP podem [comprar reservas do Azure em nome de um cliente](azure-reservations-buying.md) ou podem [permitir que o cliente compre suas próprias reservas](give-customers-permission.md) de uma assinatura anterior do Azure que o parceiro comprou para eles.</span><span class="sxs-lookup"><span data-stu-id="fc8a9-129">CSP partners can [buy Azure reservations on behalf of a customer](azure-reservations-buying.md) or they can [allow the customer to buy their own reservations](give-customers-permission.md) from a prior Azure subscription the partner has purchased for them.</span></span>

<span data-ttu-id="fc8a9-130">As reservas do Azure oferecem aos clientes a flexibilidade da virtualização para uma ampla gama de soluções de computação, incluindo desenvolvimento e teste, execução de aplicativos e extensão do data center.</span><span class="sxs-lookup"><span data-stu-id="fc8a9-130">Azure Reservations give customers the flexibility of virtualization for a wide range of computing solutions, including development and testing, running applications and extending the data center.</span></span>

<span data-ttu-id="fc8a9-131">Com as [instâncias de VM reservadas do Azure](https://azure.microsoft.com/pricing/reserved-vm-instances/) , por exemplo, os clientes comerciais agora podem economizar até 72% versus o preço pago conforme o uso da VM do Azure simplesmente comprando-ou "reservando"-a máquina virtual por um período de 1 ou 3 anos.</span><span class="sxs-lookup"><span data-stu-id="fc8a9-131">With [Azure Reserved VM Instances](https://azure.microsoft.com/pricing/reserved-vm-instances/) for example, commercial customers can now save up to 72% versus pay-as-you-go Azure VM pricing simply by purchasing - or "reserving" - the virtual machine for a 1- or 3-year period.</span></span> <span data-ttu-id="fc8a9-132">Os clientes do Windows Server com o Benefício Híbrido do Azure, incluído com o Software Assurance, poderão economizar até 80% em relação ao preço do pagamento conforme o uso.</span><span class="sxs-lookup"><span data-stu-id="fc8a9-132">Windows Server customers with Azure Hybrid Benefit, included with Software Assurance, will be able to save up to 80% versus pay-as-you-go pricing.</span></span>

<span data-ttu-id="fc8a9-133">Com uma combinação inigualável de preços atraentes e flexibilidade de implantação inigualável, os clientes verão o melhor valor geral quando escolherem as reservas do Azure:</span><span class="sxs-lookup"><span data-stu-id="fc8a9-133">With an unmatched combination of compelling pricing and unmatched deployment flexibility, customers will see the best overall value when they choose Azure Reservations:</span></span>

#### <a name="azure-reservations"></a><span data-ttu-id="fc8a9-134">Reservas do Azure</span><span class="sxs-lookup"><span data-stu-id="fc8a9-134">Azure reservations</span></span>

- <span data-ttu-id="fc8a9-135">Instâncias de VM reservadas do Azure</span><span class="sxs-lookup"><span data-stu-id="fc8a9-135">Azure Reserved VM Instances</span></span>
- <span data-ttu-id="fc8a9-136">Reservas do BD SQL</span><span class="sxs-lookup"><span data-stu-id="fc8a9-136">SQL DB Reservations</span></span>
- <span data-ttu-id="fc8a9-137">Instância Gerenciada de SQL</span><span class="sxs-lookup"><span data-stu-id="fc8a9-137">SQL Managed Instance</span></span>
- <span data-ttu-id="fc8a9-138">Azure Cosmos DB</span><span class="sxs-lookup"><span data-stu-id="fc8a9-138">Azure Cosmos DB</span></span>
- <span data-ttu-id="fc8a9-139">SQL Data Warehouse do Azure</span><span class="sxs-lookup"><span data-stu-id="fc8a9-139">Azure SQL Data Warehouse</span></span>
- <span data-ttu-id="fc8a9-140">Serviços de Aplicativos</span><span class="sxs-lookup"><span data-stu-id="fc8a9-140">App Services</span></span>
- <span data-ttu-id="fc8a9-141">Reservas de unidade de Azure Databricks</span><span class="sxs-lookup"><span data-stu-id="fc8a9-141">Azure Databricks unit reservations</span></span>
- <span data-ttu-id="fc8a9-142">Disco Gerenciado</span><span class="sxs-lookup"><span data-stu-id="fc8a9-142">Managed Disk</span></span>
- <span data-ttu-id="fc8a9-143">Blob de blocos</span><span class="sxs-lookup"><span data-stu-id="fc8a9-143">Block blob</span></span>
- <span data-ttu-id="fc8a9-144">MySQL</span><span class="sxs-lookup"><span data-stu-id="fc8a9-144">MySQL</span></span>
- <span data-ttu-id="fc8a9-145">Gerenciador de dados do Azure</span><span class="sxs-lookup"><span data-stu-id="fc8a9-145">Azure Data explorer</span></span>
- <span data-ttu-id="fc8a9-146">MariaDB</span><span class="sxs-lookup"><span data-stu-id="fc8a9-146">MariaDB</span></span>
- <span data-ttu-id="fc8a9-147">PostgreSQL</span><span class="sxs-lookup"><span data-stu-id="fc8a9-147">PostgreSQL</span></span>

#### <a name="server-subscriptions"></a><span data-ttu-id="fc8a9-148">Assinaturas de servidor</span><span class="sxs-lookup"><span data-stu-id="fc8a9-148">Server subscriptions</span></span>

- <span data-ttu-id="fc8a9-149">Windows Server</span><span class="sxs-lookup"><span data-stu-id="fc8a9-149">Windows Server</span></span>
- <span data-ttu-id="fc8a9-150">CALs de Serviços de Área de Trabalho Remota (RDS)</span><span class="sxs-lookup"><span data-stu-id="fc8a9-150">Remote Desktop Services (RDS) CALs</span></span>
- <span data-ttu-id="fc8a9-151">SQL Server</span><span class="sxs-lookup"><span data-stu-id="fc8a9-151">SQL Server</span></span>

#### <a name="linux-isv-annual-subscriptions"></a><span data-ttu-id="fc8a9-152">Assinaturas anuais do Linux ISV</span><span class="sxs-lookup"><span data-stu-id="fc8a9-152">Linux ISV annual subscriptions</span></span>

- <span data-ttu-id="fc8a9-153">SUSE Linux</span><span class="sxs-lookup"><span data-stu-id="fc8a9-153">SUSE Linux</span></span>
- <span data-ttu-id="fc8a9-154">Red Hat Enterprise Linux</span><span class="sxs-lookup"><span data-stu-id="fc8a9-154">Red Hat Enterprise Linux</span></span>
- <span data-ttu-id="fc8a9-155">Red Hat OpenShift no Azure</span><span class="sxs-lookup"><span data-stu-id="fc8a9-155">Azure Red Hat OpenShift</span></span>

#### <a name="isv-annual-subscriptions"></a><span data-ttu-id="fc8a9-156">Assinaturas anuais do ISV</span><span class="sxs-lookup"><span data-stu-id="fc8a9-156">ISV annual subscriptions</span></span>

- <span data-ttu-id="fc8a9-157">Solução VMware no Azure pela CloudSimple</span><span class="sxs-lookup"><span data-stu-id="fc8a9-157">Azure VMware Solution by CloudSimple</span></span>

## <a name="getting-started"></a><span data-ttu-id="fc8a9-158">Introdução</span><span class="sxs-lookup"><span data-stu-id="fc8a9-158">Getting started</span></span>

<span data-ttu-id="fc8a9-159">Para entender como você pode posicionar as reservas do Azure com seus clientes e colocar a operação em funcionamento o mais rápido possível, recomendamos a seguinte abordagem para revisar os materiais de preparação:</span><span class="sxs-lookup"><span data-stu-id="fc8a9-159">To understand how you can position Azure Reservations with your customers and get up and running operationally as quickly as possible, we recommend the following approach to review the readiness materials:</span></span>

1. <span data-ttu-id="fc8a9-160">Examine as Apresentações de Visão Geral e os webinars associados para obter a proposição de valor e o posicionamento do cliente</span><span class="sxs-lookup"><span data-stu-id="fc8a9-160">Review the Overview Presentations and associated webinars for the customer value proposition and positioning</span></span>
2. <span data-ttu-id="fc8a9-161">Examinar e entender o Guia de Operação de Comércio Moderno</span><span class="sxs-lookup"><span data-stu-id="fc8a9-161">Review and understand the Modern Commerce Operating Guide</span></span>
3. <span data-ttu-id="fc8a9-162">Examinar as perguntas frequentes sobre o Azure RI e as assinaturas de servidor</span><span class="sxs-lookup"><span data-stu-id="fc8a9-162">Review the Azure RI and Server Subscriptions FAQ</span></span>
4. <span data-ttu-id="fc8a9-163">Noções básicas sobre as atualizações para Reservas do Azure e assinaturas de servidor na [API do Partner Center (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)</span><span class="sxs-lookup"><span data-stu-id="fc8a9-163">Understand updates for Azure Reservations and Server Subscriptions in the [Partner Center API (API/SDK)](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)</span></span>

## <a name="resources"></a><span data-ttu-id="fc8a9-164">Recursos</span><span class="sxs-lookup"><span data-stu-id="fc8a9-164">Resources</span></span>

<span data-ttu-id="fc8a9-165">A seguir, uma lista abrangente de recursos para ajudá-lo a se integrar rapidamente às transações de Reservas do Azure por meio do Partner Center:</span><span class="sxs-lookup"><span data-stu-id="fc8a9-165">Below is a comprehensive list of resources to help you onboard quickly to transacting Azure Reservations through Partner Center:</span></span>

### <a name="sales-readiness"></a><span data-ttu-id="fc8a9-166">Preparação para vendas</span><span class="sxs-lookup"><span data-stu-id="fc8a9-166">Sales readiness</span></span>

- [<span data-ttu-id="fc8a9-167">Reservas do Azure e assinaturas de servidor com Benefício Híbrido do Azure visão geral</span><span class="sxs-lookup"><span data-stu-id="fc8a9-167">Azure Reservations and Server Subscriptions with Azure Hybrid Benefit Overview</span></span>](https://assetsprod.microsoft.com/Azure-reservations-and-server-subscriptions-with-azure-hybrid-benefit.pptx)
- [<span data-ttu-id="fc8a9-168">Planilha de Vendas</span><span class="sxs-lookup"><span data-stu-id="fc8a9-168">Sales Sheet</span></span>](https://assetsprod.microsoft.com/mpn/Azure-RI-Sales-Sheet-CSP.pdf)
- [<span data-ttu-id="fc8a9-169">Perguntas frequentes do parceiro para reservas do Azure</span><span class="sxs-lookup"><span data-stu-id="fc8a9-169">Partner FAQ for Azure Reservations</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations.docx)
- [<span data-ttu-id="fc8a9-170">Perguntas frequentes do parceiro para reservas do Azure e BD SQL</span><span class="sxs-lookup"><span data-stu-id="fc8a9-170">Partner FAQ for Azure Reservations and SQL DB</span></span>](https://assetsprod.microsoft.com/Partner-faq-for-azure-reservations-sql-db.docx)
- [<span data-ttu-id="fc8a9-171">CAL (licença de acesso para cliente) do Serviços de Área de Trabalho Remota (RDS) (anúncio)</span><span class="sxs-lookup"><span data-stu-id="fc8a9-171">Remote Desktop Services (RDS) Client Access License (CAL) (announcement)</span></span>](https://cloudblogs.microsoft.com/windowsserver/2018/10/03/remote-desktop-services-2019-generally-available-with-windows-server-2019/)
- [<span data-ttu-id="fc8a9-172">Instâncias de VM reservadas do Azure (portal do Azure)</span><span class="sxs-lookup"><span data-stu-id="fc8a9-172">Azure Reserved VM Instances (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances)
- [<span data-ttu-id="fc8a9-173">Assinaturas de servidor</span><span class="sxs-lookup"><span data-stu-id="fc8a9-173">Server Subscriptions</span></span>](csp-software-subscriptions.md)
- [<span data-ttu-id="fc8a9-174">Visão geral do BD SQL no Azure</span><span class="sxs-lookup"><span data-stu-id="fc8a9-174">SQL DB in Azure Overview</span></span>](https://assetsprod.microsoft.com/Sql-db-in-azure-overview.pptx)
- [<span data-ttu-id="fc8a9-175">Reservas do BD SQL (portal do Azure)</span><span class="sxs-lookup"><span data-stu-id="fc8a9-175">SQL DB Reservations (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-reserved-capacity)
- [<span data-ttu-id="fc8a9-176">Azure Cosmos DB (portal do Azure)</span><span class="sxs-lookup"><span data-stu-id="fc8a9-176">Azure Cosmos DB (Azure portal)</span></span>](https://docs.microsoft.com/azure/cosmos-db/cosmos-db-reserved-capacity)
- [<span data-ttu-id="fc8a9-177">Instância Gerenciada do SQL (portal do Azure)</span><span class="sxs-lookup"><span data-stu-id="fc8a9-177">SQL Managed Instance (Azure portal)</span></span>](https://docs.microsoft.com/azure/sql-database/sql-database-managed-instance)
- [<span data-ttu-id="fc8a9-178">SUSE e Red Hat Enterprise Linux (portal do Azure)</span><span class="sxs-lookup"><span data-stu-id="fc8a9-178">SUSE and Red Hat Enterprise Linux (Azure portal)</span></span>](https://docs.microsoft.com/azure/virtual-machines/linux/prepay-suse-software-charges)
- [<span data-ttu-id="fc8a9-179">Red Hat Linux no Azure</span><span class="sxs-lookup"><span data-stu-id="fc8a9-179">Red Hat Linux on Azure</span></span>](https://azure.com/redhat)
- [<span data-ttu-id="fc8a9-180">SUSE Linux no Azure</span><span class="sxs-lookup"><span data-stu-id="fc8a9-180">SUSE Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/suse/)
- [<span data-ttu-id="fc8a9-181">Linux no Azure</span><span class="sxs-lookup"><span data-stu-id="fc8a9-181">Linux on Azure</span></span>](https://azure.microsoft.com/overview/linux-on-azure/)
- [<span data-ttu-id="fc8a9-182">Visão geral de preços do Azure</span><span class="sxs-lookup"><span data-stu-id="fc8a9-182">Azure Pricing Overview</span></span>](https://azure.microsoft.com/pricing/)
- [<span data-ttu-id="fc8a9-183">Calculadora de Preços do Azure</span><span class="sxs-lookup"><span data-stu-id="fc8a9-183">Azure Pricing Calculator</span></span>](https://azure.microsoft.com/pricing/calculator)
- [<span data-ttu-id="fc8a9-184">Reservas de unidade de Azure Databricks</span><span class="sxs-lookup"><span data-stu-id="fc8a9-184">Azure Databricks unit reservations</span></span>](https://docs.microsoft.com/azure/billing/billing-prepay-databricks-reserved-capacity)
- <span data-ttu-id="fc8a9-185">Listas de preços do CSP: as listas de preços **Microsoft Azure instâncias reservadas** e **assinaturas de software** estão localizadas na página de [ofertas de preços](https://partner.microsoft.com/pcv/sales) do Partner Center &.</span><span class="sxs-lookup"><span data-stu-id="fc8a9-185">CSP Price lists:  The **Microsoft Azure Reserved Instances** and **Software Subscriptions** price lists are both located on the Partner Center [Pricing & Offers](https://partner.microsoft.com/pcv/sales) page.</span></span>

### <a name="training"></a><span data-ttu-id="fc8a9-186">Treinamento</span><span class="sxs-lookup"><span data-stu-id="fc8a9-186">Training</span></span>

<span data-ttu-id="fc8a9-187">Registre-se para exibir os eventos de [webinars de prontidão de licenciamento comercial](https://commercial-licensing.eventbuilder.com/FY2019_ALL) e sob demanda.</span><span class="sxs-lookup"><span data-stu-id="fc8a9-187">Register to view [Commercial Licensing Readiness webinars](https://commercial-licensing.eventbuilder.com/FY2019_ALL) and on-demand events.</span></span>

<span data-ttu-id="fc8a9-188">Os eventos de prontidão de licenciamento sob demanda incluem tópicos como:</span><span class="sxs-lookup"><span data-stu-id="fc8a9-188">Licensing Readiness on-demand events include topics like:</span></span>

- <span data-ttu-id="fc8a9-189">Serviços online do CSP, CSP Azure e atualizações gerais de licenciamento, incluindo o Azure (novembro de 2018)</span><span class="sxs-lookup"><span data-stu-id="fc8a9-189">CSP Online Services, CSP Azure, and general licensing updates, including Azure (November 2018)</span></span>
- <span data-ttu-id="fc8a9-190">Capacidade reservada do banco de BD SQL & flexibilidade de tamanho de instância (agosto de 2018)</span><span class="sxs-lookup"><span data-stu-id="fc8a9-190">SQL DB Reserved Capacity & Instance Size Flexibility (August 2018)</span></span>
- <span data-ttu-id="fc8a9-191">Assinaturas de servidor no CSP (julho de 2018)</span><span class="sxs-lookup"><span data-stu-id="fc8a9-191">Server Subscriptions in CSP (July 2018)</span></span>
- <span data-ttu-id="fc8a9-192">Visão geral das reservas do Azure no CSP (maio de 2018)</span><span class="sxs-lookup"><span data-stu-id="fc8a9-192">Azure Reservations Overview in CSP (May 2018)</span></span>

<span data-ttu-id="fc8a9-193">Outros treinamentos úteis incluem o [módulo de licenciamento do Azure na Universidade do parceiro](https://aka.ms/azure_partner_licensing).</span><span class="sxs-lookup"><span data-stu-id="fc8a9-193">Other useful training includes the [Azure Licensing Module on Partner University](https://aka.ms/azure_partner_licensing).</span></span>

### <a name="operations"></a><span data-ttu-id="fc8a9-194">Operações</span><span class="sxs-lookup"><span data-stu-id="fc8a9-194">Operations</span></span>

- <span data-ttu-id="fc8a9-195">[Guia de operações do comércio moderno](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (atualizado): um guia abrangente que abrange a política de chave e os aspectos operacionais, como contratos, pedidos por meio do Partner Center, fatura, detalhes da lista de preços, incentivos, arquivo de reconciliação, API/SDK, sandbox e serviços compartilhados de parceiros do Azure.</span><span class="sxs-lookup"><span data-stu-id="fc8a9-195">[Modern Commerce Operations Guide](https://assetsprod.microsoft.com/mpn/Partner-Center-Modern-Commerce-Operating-Guide.docx) (updated):  A comprehensive guide covering key policy and operational aspects such as agreements, ordering through Partner Center, invoice, price list details, incentives, reconciliation file, API/SDK, Sandbox, and Azure Partner Shared Services.</span></span>
- [<span data-ttu-id="fc8a9-196">Matriz de Moeda do Cliente e Disponibilidade por País de Ofertas Modernas</span><span class="sxs-lookup"><span data-stu-id="fc8a9-196">Modern Offers Country Availability and Customer Currency Matrix</span></span>](https://assetsprod.microsoft.com/modern-offers-country-currency-availability.xlsx)
- [<span data-ttu-id="fc8a9-197">Vender Instâncias Reservadas do Microsoft Azure</span><span class="sxs-lookup"><span data-stu-id="fc8a9-197">Sell Microsoft Azure Reserved Instances</span></span>](https://go.microsoft.com/fwlink/?linkid=872806)
- [<span data-ttu-id="fc8a9-198">Comprar Reservas do Microsoft Azure em nome de seus clientes</span><span class="sxs-lookup"><span data-stu-id="fc8a9-198">Buy Microsoft Azure reservations on behalf of your customers</span></span>](https://go.microsoft.com/fwlink/?linkid=872807)
- [<span data-ttu-id="fc8a9-199">Gerenciar reservas do Azure em nome dos seus clientes</span><span class="sxs-lookup"><span data-stu-id="fc8a9-199">Manage Azure reservations on behalf of your customers</span></span>](https://go.microsoft.com/fwlink/?linkid=872808)
- [<span data-ttu-id="fc8a9-200">Cobrança das reservas do Azure</span><span class="sxs-lookup"><span data-stu-id="fc8a9-200">Billing for Azure reservations</span></span>](azure-plan-billing.md)
- [<span data-ttu-id="fc8a9-201">Dimensionamento da VM para uso máximo de reserva</span><span class="sxs-lookup"><span data-stu-id="fc8a9-201">VM sizing for maximum reservation usage</span></span>](https://go.microsoft.com/fwlink/?linkid=872810)
- [<span data-ttu-id="fc8a9-202">API do Partner Center (API/SDK)</span><span class="sxs-lookup"><span data-stu-id="fc8a9-202">Partner Center API (API/SDK)</span></span>](https://docs.microsoft.com/partner-center/develop/purchase-azure-reserved-vm-instances)
- [<span data-ttu-id="fc8a9-203">Serviços de área de trabalho remota</span><span class="sxs-lookup"><span data-stu-id="fc8a9-203">Remote Desktop Services</span></span>](https://docs.microsoft.com/windows-server/remote/remote-desktop-services/welcome-to-rds)

## <a name="azure-hybrid-benefit"></a><span data-ttu-id="fc8a9-204">Benefício Híbrido do Azure</span><span class="sxs-lookup"><span data-stu-id="fc8a9-204">Azure Hybrid Benefit</span></span>

<span data-ttu-id="fc8a9-205">O [Benefício Híbrido do Azure](https://azure.microsoft.com/pricing/hybrid-benefit) ajuda você a obter mais valor de suas licenças do Windows Server e a economizar até \*47% em máquinas virtuais.</span><span class="sxs-lookup"><span data-stu-id="fc8a9-205">The [Azure Hybrid Benefit](https://azure.microsoft.com/pricing/hybrid-benefit) helps you get more value from your Windows Server licenses and save up to \*47 percent on virtual machines.</span></span> <span data-ttu-id="fc8a9-206">Use o benefício com as licenças do Windows Server Datacenter e da Edição Standard cobertas no Software Assurance.</span><span class="sxs-lookup"><span data-stu-id="fc8a9-206">You can use the benefit with Windows Server Datacenter and Standard edition licenses covered with Software Assurance.</span></span> <span data-ttu-id="fc8a9-207">Dependendo da edição, você pode converter ou reutilizar suas licenças para executar máquinas virtuais do Windows Server no Azure e pagar uma taxa de computação base mais baixa (taxas de máquina virtual do Linux).</span><span class="sxs-lookup"><span data-stu-id="fc8a9-207">Depending on the edition, you can convert or reuse your licenses to run Windows Server virtual machines in Azure and pay a lower base compute rate (Linux virtual machine rates).</span></span>

<span data-ttu-id="fc8a9-208">Consulte também [Perguntas frequentes sobre o Benefício Híbrido do Azure](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span><span class="sxs-lookup"><span data-stu-id="fc8a9-208">See also [Azure Hybrid Benefit FAQ](https://azure.microsoft.com/pricing/hybrid-benefit/faq/)</span></span>

<span data-ttu-id="fc8a9-209">\* A economia real pode variar com base na região, no tipo de instância ou no uso.</span><span class="sxs-lookup"><span data-stu-id="fc8a9-209">\*Actual savings may vary based on region, instance type, or usage.</span></span>
