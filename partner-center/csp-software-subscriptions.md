---
title: Vender assinaturas de software por meio do CSP | Partner Center
ms.topic: article
ms.date: 11/27/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como os parceiros no programa CSP podem usar o Partner Center para comprar, gerenciar, vender e cancelar as instâncias reservadas do Azure e as assinaturas de servidor para os clientes.
author: MaggiePucciEvans
ms.author: evansma
keywords: Provedor de Soluções na Nuvem, CSP, Serviços baseados na nuvem, Azure, Azure RI, Windows Server, SQL Server, assinaturas de software
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 0e2b735c1b67b49c18f2b83c042ec5a2bb0eefbd
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2019
ms.locfileid: "74721338"
---
# <a name="sell-software-subscriptions-through-csp"></a><span data-ttu-id="a741d-104">Vender assinaturas de software por meio do CSP</span><span class="sxs-lookup"><span data-stu-id="a741d-104">Sell software subscriptions through CSP</span></span>

<span data-ttu-id="a741d-105">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="a741d-105">**Appropriate roles**</span></span>

- <span data-ttu-id="a741d-106">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="a741d-106">Admin agent</span></span>
- <span data-ttu-id="a741d-107">Administração global</span><span class="sxs-lookup"><span data-stu-id="a741d-107">Global admin</span></span>

<span data-ttu-id="a741d-108">Com as reservas do Azure e as assinaturas de servidor (assinaturas do Windows Server e do SQL Server), os parceiros no programa CSP podem abordar melhor a demanda de cliente de crescimento rápido para soluções mais econômicas para dar suporte a altamente previsível e persistente cargas de trabalho de nuvem.</span><span class="sxs-lookup"><span data-stu-id="a741d-108">With Azure reservations and Server subscriptions (Windows Server and SQL Server subscriptions), partners in the CSP program can better address the fast-growing customer demand for more cost-effective solutions to support highly predictable and persistent cloud workloads.</span></span> 

<span data-ttu-id="a741d-109">Agora você pode adquirir, provisionar e gerenciar reservas do Azure e assinaturas de servidor em nome de clientes comerciais por meio do Partner Center e do portal do Azure, aproveitando o Benefício Híbrido do Azure.</span><span class="sxs-lookup"><span data-stu-id="a741d-109">You can now acquire, provision, and manage Azure reservations and Server subscriptions on behalf of commercial customers through Partner Center and the Azure Portal by taking advantage of the Azure Hybrid Benefit.</span></span> 

<span data-ttu-id="a741d-110">O Benefício Híbrido do Azure ajuda você a obter mais valor de suas licenças do Windows Server e a economizar até 40% em máquinas virtuais.</span><span class="sxs-lookup"><span data-stu-id="a741d-110">The Azure Hybrid Benefit helps you get more value from your Windows Server licenses and save up to 40 percent on virtual machines.</span></span> <span data-ttu-id="a741d-111">Você pode usar o benefício com licenças do Windows Server Datacenter e Standard edition cobertas com Software Assurance.</span><span class="sxs-lookup"><span data-stu-id="a741d-111">You can use the benefit with Windows Server Datacenter and Standard edition licenses covered with Software Assurance.</span></span> <span data-ttu-id="a741d-112">Dependendo da edição, você pode converter ou reutilizar suas licenças para executar máquinas virtuais do Windows Server no Azure e pagar uma taxa de computação de base inferior (taxas de máquina virtual do Linux, por exemplo,).</span><span class="sxs-lookup"><span data-stu-id="a741d-112">Depending on the edition, you can convert or re-use your licenses to run Windows Server virtual machines in Azure and pay a lower base compute rate (Linux virtual machine rates, e.g.).</span></span>

> [!NOTE]  
> <span data-ttu-id="a741d-113">As reservas do Azure não estão disponíveis nos seguintes mercados:</span><span class="sxs-lookup"><span data-stu-id="a741d-113">Azure reservations are not available in the following markets:</span></span>  
> * <span data-ttu-id="a741d-114">Argentina</span><span class="sxs-lookup"><span data-stu-id="a741d-114">Argentina</span></span>
> * <span data-ttu-id="a741d-115">Brasil</span><span class="sxs-lookup"><span data-stu-id="a741d-115">Brazil</span></span>
> * <span data-ttu-id="a741d-116">China</span><span class="sxs-lookup"><span data-stu-id="a741d-116">China</span></span>
> * <span data-ttu-id="a741d-117">Indonésia</span><span class="sxs-lookup"><span data-stu-id="a741d-117">Indonesia</span></span>
> * <span data-ttu-id="a741d-118">Liechtenstein</span><span class="sxs-lookup"><span data-stu-id="a741d-118">Liechtenstein</span></span>
> * <span data-ttu-id="a741d-119">Jersey</span><span class="sxs-lookup"><span data-stu-id="a741d-119">Jersey</span></span>
> * <span data-ttu-id="a741d-120">Malásia</span><span class="sxs-lookup"><span data-stu-id="a741d-120">Malaysia</span></span>
> * <span data-ttu-id="a741d-121">México</span><span class="sxs-lookup"><span data-stu-id="a741d-121">Mexico</span></span>
> * <span data-ttu-id="a741d-122">Rússia</span><span class="sxs-lookup"><span data-stu-id="a741d-122">Russia</span></span>
> * <span data-ttu-id="a741d-123">Arábia Saudita</span><span class="sxs-lookup"><span data-stu-id="a741d-123">Saudi Arabia</span></span>
> * <span data-ttu-id="a741d-124">África do Sul</span><span class="sxs-lookup"><span data-stu-id="a741d-124">South Africa</span></span>
> * <span data-ttu-id="a741d-125">Turquia</span><span class="sxs-lookup"><span data-stu-id="a741d-125">Turkey</span></span>

<!--March 20, 2019 - this list of countries was correct as of today. Maggie last updated the list according to FAREAST\v-pubobb in bug 20907186.
-->

## <a name="buy-software-subscriptions-on-behalf-of-customers"></a><span data-ttu-id="a741d-126">Comprar assinaturas de software em nome dos clientes</span><span class="sxs-lookup"><span data-stu-id="a741d-126">Buy software subscriptions on behalf of customers</span></span>

<span data-ttu-id="a741d-127">Para comprar assinaturas de software em nome de um cliente, acesse a página de detalhes do cliente, selecione **Adicionar produtos**e siga as instruções na tela para criar e pagar pelo seu pedido.</span><span class="sxs-lookup"><span data-stu-id="a741d-127">To buy software subscriptions on behalf of a customer, go to the customer's detail page, select **Add products**, and then follow the on-screen instructions to create and pay for your order.</span></span> <span data-ttu-id="a741d-128">Todos os preços comerciais excluem impostos com exceção da Austrália e do Brasil.</span><span class="sxs-lookup"><span data-stu-id="a741d-128">All commercial pricing excludes tax with the exception of Australia and Brazil.</span></span> <span data-ttu-id="a741d-129">Para a Austrália e o Brasil, o preço inclui impostos.</span><span class="sxs-lookup"><span data-stu-id="a741d-129">For Australia and Brazil, the price includes tax.</span></span>

## <a name="activate-and-manage-software-subscriptions"></a><span data-ttu-id="a741d-130">Ativar e gerenciar assinaturas de software</span><span class="sxs-lookup"><span data-stu-id="a741d-130">Activate and manage software subscriptions</span></span>

<span data-ttu-id="a741d-131">Depois de comprar a assinatura de software, siga as etapas abaixo para baixá-la.</span><span class="sxs-lookup"><span data-stu-id="a741d-131">After you purchase the software subscription, follow the steps below to download it.</span></span>

>[!NOTE]
><span data-ttu-id="a741d-132">Você deve ser um agente de administração para baixar o software e obter as chaves de ativação.</span><span class="sxs-lookup"><span data-stu-id="a741d-132">You must be an Admin agent to download software and get activation keys.</span></span>

1. <span data-ttu-id="a741d-133">Acesse a página de detalhes do cliente e então selecione **Software**.</span><span class="sxs-lookup"><span data-stu-id="a741d-133">Go to your customer's detail page and then select **Software**.</span></span> <span data-ttu-id="a741d-134">Você verá uma lista de todos os softwares que comprou em nome do cliente.</span><span class="sxs-lookup"><span data-stu-id="a741d-134">You'll see a list of all the software you've purchased on behalf of the customer.</span></span> 
2.  <span data-ttu-id="a741d-135">Expanda o produto que você deseja baixar.</span><span class="sxs-lookup"><span data-stu-id="a741d-135">Expand the product you want to download.</span></span> <span data-ttu-id="a741d-136">No campo **Selecionar produto**, selecione a **Versão**, o **Idioma** e o **Tipo de arquivo/sistema operacional** desejados.</span><span class="sxs-lookup"><span data-stu-id="a741d-136">In the **Select product** field, select the **Version**, **Language**, and **File type/OS** that you want.</span></span> 
3.  <span data-ttu-id="a741d-137">Selecione **Enviar** para exibir os produtos específicos.</span><span class="sxs-lookup"><span data-stu-id="a741d-137">Select **Submit** to display the specific products.</span></span> 
4.  <span data-ttu-id="a741d-138">Selecione **Obter chaves e downloads**.</span><span class="sxs-lookup"><span data-stu-id="a741d-138">Select **Get keys and downloads**.</span></span> 
5.  <span data-ttu-id="a741d-139">Selecione **Baixar** para iniciar o download ou selecione **Copiar link** para copiar o link e enviá-lo ao cliente.</span><span class="sxs-lookup"><span data-stu-id="a741d-139">Select **Download** to begin downloading, or select **Copy link** to copy the link and send it to the customer.</span></span> 

>[!NOTE]
><span data-ttu-id="a741d-140">Esse link expirará após duas semanas ou 50 downloads, o que ocorrer primeiro.</span><span class="sxs-lookup"><span data-stu-id="a741d-140">This link will expire after two weeks or 50 downloads, whichever comes first.</span></span> <span data-ttu-id="a741d-141">Depois que o link expirar, retorne a essa página e selecione **Obter chaves e downloads** novamente para habilitar outras duas semanas ou 50 downloads.</span><span class="sxs-lookup"><span data-stu-id="a741d-141">Once the link expires, return to this page and select **Get keys and downloads** again to enable another two weeks or 50 downloads.</span></span> <span data-ttu-id="a741d-142">Você pode fazer isso quantas vezes precisar.</span><span class="sxs-lookup"><span data-stu-id="a741d-142">You can do this as many times as you need to.</span></span> 

## <a name="view-activity-for-software-key-access-and-software-downloads"></a><span data-ttu-id="a741d-143">Exibir atividade de acesso a chave de software e downloads de software</span><span class="sxs-lookup"><span data-stu-id="a741d-143">View activity for software key access and software downloads</span></span>
<span data-ttu-id="a741d-144">Para fins de auditoria ou de conformidade, talvez seja necessário verificar uma lista de usuários que acessaram as chaves de software de assinatura do servidor ou o software de assinatura do servidor baixado.</span><span class="sxs-lookup"><span data-stu-id="a741d-144">For auditing or compliance purposes, you may need to check a list of users who have either accessed Server subscription software keys or downloaded Server subscription software.</span></span> <span data-ttu-id="a741d-145">Use o procedimento abaixo para acessar essas informações.</span><span class="sxs-lookup"><span data-stu-id="a741d-145">Use the procedure below to access this information.</span></span> 

>[!NOTE]
><span data-ttu-id="a741d-146">Você deve ser um administrador global, administrador de conta, administrador de referência ou administrador de conteúdo de marketing para ver esses logs de atividade.</span><span class="sxs-lookup"><span data-stu-id="a741d-146">You must be a Global administrator, Account admin, Referral admin, or Marketing content admin to see these activity logs.</span></span> 

1.  <span data-ttu-id="a741d-147">No Partner Center, selecione o ícone de engrenagem no canto superior direito.</span><span class="sxs-lookup"><span data-stu-id="a741d-147">In Partner Center, select the gear icon from the upper right corner.</span></span> 
2.  <span data-ttu-id="a741d-148">No menu, selecione **log de atividades**.</span><span class="sxs-lookup"><span data-stu-id="a741d-148">In the menu, select **Activity log**.</span></span>
3.  <span data-ttu-id="a741d-149">Insira o intervalo de datas para a atividade que você deseja ver.</span><span class="sxs-lookup"><span data-stu-id="a741d-149">Enter the date range for the activity you want to see.</span></span> <span data-ttu-id="a741d-150">O log de atividades exibirá uma lista de usuários que acessaram as chaves de software ou o software baixado durante o tempo especificado.</span><span class="sxs-lookup"><span data-stu-id="a741d-150">The activity log will display a list of users who have either accessed software keys or downloaded software during the time you specified.</span></span> 

## <a name="cancel-a-purchase"></a><span data-ttu-id="a741d-151">Cancelar uma compra</span><span class="sxs-lookup"><span data-stu-id="a741d-151">Cancel a purchase</span></span>

<span data-ttu-id="a741d-152">Você pode cancelar uma compra de software dentro de 60 dias da data de compra.</span><span class="sxs-lookup"><span data-stu-id="a741d-152">You can cancel a software purchase within 60 days of the purchase date.</span></span> <span data-ttu-id="a741d-153">A Microsoft não cobra uma taxa de rescisão antecipada, no entanto, você não pode cancelar uma compra após 60 dias a partir da data de compra.</span><span class="sxs-lookup"><span data-stu-id="a741d-153">Microsoft does not charge an early termination fee, however, you can't cancel a purchase after 60 days from the purchase date.</span></span>

<span data-ttu-id="a741d-154">Depois de cancelar a compra, a chave de software será revogada.</span><span class="sxs-lookup"><span data-stu-id="a741d-154">After you cancel the purchase, the software key will be revoked.</span></span> 

<span data-ttu-id="a741d-155">Siga as etapas abaixo para cancelar uma compra:</span><span class="sxs-lookup"><span data-stu-id="a741d-155">Follow the steps below to cancel a purchase:</span></span>

>[!NOTE]
><span data-ttu-id="a741d-156">Você deve ser um agente administrativo para cancelar uma compra.</span><span class="sxs-lookup"><span data-stu-id="a741d-156">You must be an Admin agent to cancel a purchase.</span></span> 

1.  <span data-ttu-id="a741d-157">Antes do início do processo, verifique se você tem o seguinte:</span><span class="sxs-lookup"><span data-stu-id="a741d-157">Before beginning the process, make sure you have the following:</span></span>
    -   <span data-ttu-id="a741d-158">O GUID do locatário do cliente ou o nome de domínio</span><span class="sxs-lookup"><span data-stu-id="a741d-158">The customer tenant GUID or domain name</span></span>
    -   <span data-ttu-id="a741d-159">ID do Pedido ou ID da Assinatura</span><span class="sxs-lookup"><span data-stu-id="a741d-159">Order ID or Subscription ID</span></span>
    -   <span data-ttu-id="a741d-160">Motivo do reembolso</span><span class="sxs-lookup"><span data-stu-id="a741d-160">Refund reason</span></span>
    -   <span data-ttu-id="a741d-161">Quantidade solicitada</span><span class="sxs-lookup"><span data-stu-id="a741d-161">Amount requested</span></span>

2.  <span data-ttu-id="a741d-162">Na página detalhes do cliente, selecione **software** para ver a lista de todos os softwares que você comprou para o cliente.</span><span class="sxs-lookup"><span data-stu-id="a741d-162">On the customer's details page, select **Software** to see the list of all the software you've purchased for the customer.</span></span> 

3.  <span data-ttu-id="a741d-163">Localize o software que você deseja cancelar e selecione **Cancelar**.</span><span class="sxs-lookup"><span data-stu-id="a741d-163">Locate the software you want to cancel, and then select **Cancel**.</span></span> <span data-ttu-id="a741d-164">A página **Relatar um problema com o Partner Center** abre.</span><span class="sxs-lookup"><span data-stu-id="a741d-164">The **Report a problem with Partner Center** page opens.</span></span> 

4.  <span data-ttu-id="a741d-165">Em **Detalhes**, na lista **Tipo de problema**, selecione **Compra/Reembolso de CSP em nome de clientes**.</span><span class="sxs-lookup"><span data-stu-id="a741d-165">Under **Details**, in the **Type of problem** list, select **CSP Purchase/Refund on behalf of customers**.</span></span>

5.  <span data-ttu-id="a741d-166">Preencha os campos **Impacto** e **Título**.</span><span class="sxs-lookup"><span data-stu-id="a741d-166">Fill in the **Impact** and **Title** fields.</span></span> 

6.  <span data-ttu-id="a741d-167">No campo **Descrição**, forneça o seguinte:</span><span class="sxs-lookup"><span data-stu-id="a741d-167">In the **Description** field, provide the following:</span></span> 
    -   <span data-ttu-id="a741d-168">O GUID do locatário do cliente ou o nome de domínio</span><span class="sxs-lookup"><span data-stu-id="a741d-168">The customer tenant GUID or domain name</span></span>
    -   <span data-ttu-id="a741d-169">ID do Pedido ou ID da Assinatura</span><span class="sxs-lookup"><span data-stu-id="a741d-169">Order ID or Subscription ID</span></span>
    -   <span data-ttu-id="a741d-170">Motivo do reembolso</span><span class="sxs-lookup"><span data-stu-id="a741d-170">Refund reason</span></span>
    -   <span data-ttu-id="a741d-171">Quantidade solicitada</span><span class="sxs-lookup"><span data-stu-id="a741d-171">Amount requested</span></span>

7.  <span data-ttu-id="a741d-172">No campo **Contato**, insira seu nome, email e número de telefone.</span><span class="sxs-lookup"><span data-stu-id="a741d-172">In the **Contact** field, enter your name, email address, and phone number.</span></span> 

8.  <span data-ttu-id="a741d-173">Se você precisar anexar um arquivo por qualquer motivo, selecione **Adicionar arquivos**.</span><span class="sxs-lookup"><span data-stu-id="a741d-173">If you need to attach a file for any reason, select **Add files**.</span></span> <span data-ttu-id="a741d-174">Esta etapa é opcional.</span><span class="sxs-lookup"><span data-stu-id="a741d-174">This step is optional.</span></span> 

9.  <span data-ttu-id="a741d-175">Quando tiver terminado, selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="a741d-175">When you're finished, select **Submit**.</span></span>
