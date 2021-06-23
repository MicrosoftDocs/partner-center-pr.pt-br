---
title: Criar uma associação do cliente
ms.topic: article
ms.date: 10/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
description: Crie associações de clientes com o modelo de CPOR (parceiro de registro) de reivindicação. Ajuda a gerenciar vendas, uso e incentivos para os clientes Microsoft 365 & Dynamics 365.
author: MalloryPrincipe
ms.author: mallp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 196009d9271324377be02d0b2d12ba8a4d7a993c
ms.sourcegitcommit: 09eabb559aae25518caf3f2a59ef16a3e123c207
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2021
ms.locfileid: "112489944"
---
# <a name="customer-associations-via-the-claimed-partner-of-record-cpor-model-for-microsoft-365-and-dynamics-365"></a><span data-ttu-id="16f05-104">Associações de clientes por meio do modelo CPOR (parceiro de registro) solicitado para Microsoft 365 e Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="16f05-104">Customer associations via the Claimed Partner of Record (CPOR) model for Microsoft 365 and Dynamics 365</span></span>


<span data-ttu-id="16f05-105">**Funções apropriadas**: administrador de incentivos</span><span class="sxs-lookup"><span data-stu-id="16f05-105">**Appropriate roles**: Incentives admin</span></span>

<span data-ttu-id="16f05-106">Em 1º de outubro de 2019, a Microsoft começou a usar o modelo de CPOR (parceiro de registro) para gerenciar as associações que você tem com os clientes do Microsoft 365 e do Dynamics 365 em relação à venda de serviços online (OSA), Microsoft 365 o uso do Online Services (OSU) e OSU-Business incentivos de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="16f05-106">On October 1, 2019, Microsoft began using the Claiming Partner of Record (CPOR) model to manage the associations you have with your Microsoft 365 and Dynamics 365 customers with regard to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365, and OSU-Business Application incentives.</span></span>

>[!Important]
> <span data-ttu-id="16f05-107">As declarações de CPOR (Associação de cliente) se aplicam apenas ao aviso de venda do serviço online (OSA), uso de serviços online (OSU)-Microsoft 365 e OSU-Business os programas de incentivos de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="16f05-107">Customer Association (CPOR) claims only apply to the Online Services Advisory (OSA) Sell, Online Services Usage (OSU)-Microsoft 365 and OSU-Business Application incentive programs.</span></span> <span data-ttu-id="16f05-108">Se você estiver enviando uma declaração de cooperação para outro programa, como provedor de soluções de nuvem (CSP), revendedor gerenciado, hospedagem ou superfície, consulte o processo de declarações de cooperação descrito aqui.</span><span class="sxs-lookup"><span data-stu-id="16f05-108">If you are submitting a co-op claim for another program such as Cloud Solution Provider (CSP), Managed Reseller, Hosting, or Surface, please refer to Co-op claims process outlined here.</span></span> <br><br><span data-ttu-id="16f05-109">Quando você envia sua declaração, a Microsoft a valida.</span><span class="sxs-lookup"><span data-stu-id="16f05-109">When you submit your claim, Microsoft validates it.</span></span> <span data-ttu-id="16f05-110">Poderemos solicitar mais informações neste ponto.</span><span class="sxs-lookup"><span data-stu-id="16f05-110">We may ask you for more information at this point.</span></span> <span data-ttu-id="16f05-111">Também notificaremos o cliente sobre sua solicitação de associação.</span><span class="sxs-lookup"><span data-stu-id="16f05-111">We'll also notify the customer of your association request.</span></span> <span data-ttu-id="16f05-112">Os clientes têm cinco dias úteis para recusar. Se eles não recusarem, sua associação com esse locatário e carga de trabalho específicos será oficial.</span><span class="sxs-lookup"><span data-stu-id="16f05-112">Customers have five business days to opt out. If they don't opt out, your association with this specific tenant and workload will be official.</span></span> <span data-ttu-id="16f05-113">Neste ponto, você terá acesso aos dados de uso do cliente.</span><span class="sxs-lookup"><span data-stu-id="16f05-113">At this point you'll have access to the customer's usage data.</span></span> 

<span data-ttu-id="16f05-114">Você precisará das seguintes informações para concluir uma declaração:</span><span class="sxs-lookup"><span data-stu-id="16f05-114">You'll need the following information to complete a claim:</span></span>

- <span data-ttu-id="16f05-115">A **ID de MPN** (id de Microsoft Partner Network) para sua entidade que faz a declaração</span><span class="sxs-lookup"><span data-stu-id="16f05-115">The **MPN ID** (Microsoft Partner Network ID) for your entity that makes the claim</span></span>

- <span data-ttu-id="16f05-116">Nome de **domínio** do cliente (para obter mais informações, consulte [Localizar ID de locatário, nome de domínio, ID de objeto de usuário](find-ids-and-domain-names.md))</span><span class="sxs-lookup"><span data-stu-id="16f05-116">Customer's **domain name** (for more information, see [Find tenant ID, domain name, user object ID](find-ids-and-domain-names.md))</span></span>

- <span data-ttu-id="16f05-117">ID do **diretório** ou ID do **locatário** do cliente (para obter mais informações, consulte [Localizar ID de locatário, nome de domínio, ID de objeto de usuário](find-ids-and-domain-names.md))</span><span class="sxs-lookup"><span data-stu-id="16f05-117">Customer's **Directory ID** or **Tenant ID** (for more information, see [Find tenant ID, domain name, user object ID](find-ids-and-domain-names.md))</span></span>

- <span data-ttu-id="16f05-118">A **área da solução**, como Business Applications ou Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="16f05-118">The **Solution area**, such as Business Applications or Microsoft 365</span></span>

- <span data-ttu-id="16f05-119">A **atividade** que você realizou e o tipo de declaração que deseja fazer, como pré-vendas, uso ou associação de receita</span><span class="sxs-lookup"><span data-stu-id="16f05-119">The **Activity** you have performed and the type of claim you want to make, such as Pre-sales, Usage, or Revenue association</span></span>

- <span data-ttu-id="16f05-120">O nome do **contato** do seu cliente, o título e o endereço de email</span><span class="sxs-lookup"><span data-stu-id="16f05-120">Your customer's **Contact name**, title, and email address</span></span>

- <span data-ttu-id="16f05-121">Para o Dynamics 365, você também precisa fornecer o nome do **contato técnico** do cliente, o título e o endereço de email</span><span class="sxs-lookup"><span data-stu-id="16f05-121">For Dynamics 365, you also need to provide your customer's **Technical contact** name, title, and email address</span></span>

- <span data-ttu-id="16f05-122">O **nome de contato** e o endereço de email da sua própria empresa</span><span class="sxs-lookup"><span data-stu-id="16f05-122">Your own company's **Contact name** and email address</span></span>

- <span data-ttu-id="16f05-123">Você criará um **nome** para esta declaração</span><span class="sxs-lookup"><span data-stu-id="16f05-123">You'll create a **Name** for this claim</span></span>

- <span data-ttu-id="16f05-124">Os **produtos** ou as cargas de trabalho que você está reivindicando</span><span class="sxs-lookup"><span data-stu-id="16f05-124">The **Product(s)** or workload(s) you're claiming</span></span>

- <span data-ttu-id="16f05-125">**Poe (prova de execução)**, como uma declaração de trabalho assinada pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="16f05-125">**Proof of execution (PoE)**, such as a statement of work signed by the customer.</span></span> <span data-ttu-id="16f05-126">Você também pode baixar um modelo PoE para usar o.</span><span class="sxs-lookup"><span data-stu-id="16f05-126">You can also download a PoE template to use.</span></span>

- <span data-ttu-id="16f05-127">Para parceiros que alegam somente Associação de receita: **nome do vendedor da solução Dynamics**, **nome do cliente** e **nome do produto/solução ISV**.</span><span class="sxs-lookup"><span data-stu-id="16f05-127">For partners claiming revenue association only: **Dynamics solution seller name**, **Customer name**, and **Name of ISV product/solution**.</span></span> 

<span data-ttu-id="16f05-128">Você também deve entender os seguintes pontos:</span><span class="sxs-lookup"><span data-stu-id="16f05-128">You should also understand the following points:</span></span>

- <span data-ttu-id="16f05-129">Se você tiver clientes Microsoft 365 existentes, será necessário reassociá-los com aqueles que deseja continuar a obter incentivos de OSU usando esse processo.</span><span class="sxs-lookup"><span data-stu-id="16f05-129">If you have existing Microsoft 365 customers, you'll need to reassociate with those you want to continue to earn OSU incentives by using this process.</span></span>

- <span data-ttu-id="16f05-130">Se você tiver associações existentes com os clientes do Dynamics 365 ou Power BI, essas associações permanecerão válidas até a expiração de suas assinaturas.</span><span class="sxs-lookup"><span data-stu-id="16f05-130">If you have existing associations with Dynamics 365 or Power BI customers, these associations will remain valid, until the expiration of their subscriptions.</span></span>

- <span data-ttu-id="16f05-131">Um cliente pode ter vários parceiros, mas cada carga de trabalho (para OSU-Microsoft 365) ou assinatura (para OSA-Sell e OSU-Business aplicativos) só pode ser associada a um parceiro.</span><span class="sxs-lookup"><span data-stu-id="16f05-131">A customer can have multiple partners, but each workload (for OSU-Microsoft 365) or subscription (for OSA-Sell and OSU-Business Applications) can only be associated with one partner.</span></span>

## <a name="create-a-customer-association"></a><span data-ttu-id="16f05-132">Criar uma associação do cliente</span><span class="sxs-lookup"><span data-stu-id="16f05-132">Create a customer association</span></span>

1. <span data-ttu-id="16f05-133">Entre no [Painel do Partner Center](https://partner.microsoft.com/dashboard/).</span><span class="sxs-lookup"><span data-stu-id="16f05-133">Sign in to the [Partner Center dashboard](https://partner.microsoft.com/dashboard/).</span></span>

2. <span data-ttu-id="16f05-134">Selecione a guia **incentivos** , selecione **visão geral** e, em seguida, selecione **associações de cliente**.</span><span class="sxs-lookup"><span data-stu-id="16f05-134">Select the **Incentives** tab, select **Overview**, and then select **Customer associations**.</span></span>

3. <span data-ttu-id="16f05-135">Na parte superior da página associações do cliente, selecione **+ Associação de cliente**.</span><span class="sxs-lookup"><span data-stu-id="16f05-135">At the top of the Customer associations page, select **+ Customer association**.</span></span>

4. <span data-ttu-id="16f05-136">Selecione o **ID do MPN** do local do parceiro a ser associado ao cliente e, em seguida, adicione o nome de domínio e a ID do diretório do cliente.</span><span class="sxs-lookup"><span data-stu-id="16f05-136">Select the **MPN ID** of the partner location to be associated with the customer, and then add the customer's domain name and Directory ID.</span></span> [<span data-ttu-id="16f05-137">Localizar isso</span><span class="sxs-lookup"><span data-stu-id="16f05-137">Find this</span></span>](find-ids-and-domain-names.md)

5. <span data-ttu-id="16f05-138">Selecione **Continuar**.</span><span class="sxs-lookup"><span data-stu-id="16f05-138">Select **Continue**.</span></span>

6. <span data-ttu-id="16f05-139">Selecione a **área da solução** e a **atividade**.</span><span class="sxs-lookup"><span data-stu-id="16f05-139">Select the **Solution area** and **Activity**.</span></span> 

   >[!Note]
   >
   ><span data-ttu-id="16f05-140">Se você selecionar Business Applications, selecione **uso e/ou pré-vendas** ou associação de **receita** e, em seguida, selecione **continuar**.</span><span class="sxs-lookup"><span data-stu-id="16f05-140">If you select Business Applications, select either **Usage and/or Pre-sales**, or **Revenue association**, and then select **Continue**.</span></span> 
   <br><br><span data-ttu-id="16f05-141">Se você escolher Associação de Receita, será solicitado a fornecer informações ligeiramente diferentes das que estão listadas abaixo.</span><span class="sxs-lookup"><span data-stu-id="16f05-141">If you select Revenue association, you'll be prompted for slightly different information than what's listed below.</span></span>

7. <span data-ttu-id="16f05-142">Insira as informações apropriadas na página **associar cliente** e, em seguida, selecione **criar declaração**.</span><span class="sxs-lookup"><span data-stu-id="16f05-142">Enter the appropriate information on the **Associate customer** page, and then select **Create claim**.</span></span>

8. <span data-ttu-id="16f05-143">Selecione os produtos associados a essa associação de cliente e selecione **continuar**.</span><span class="sxs-lookup"><span data-stu-id="16f05-143">Select the product(s) associated with this customer association, and then select **Continue**.</span></span>

9. <span data-ttu-id="16f05-144">Preencha as informações de contato do cliente e da sua empresa.</span><span class="sxs-lookup"><span data-stu-id="16f05-144">Complete the customer contact information and your company's contact information.</span></span> <span data-ttu-id="16f05-145">Todos os campos são obrigatórios.</span><span class="sxs-lookup"><span data-stu-id="16f05-145">All fields are required.</span></span> 

   >[!NOTE]
   ><span data-ttu-id="16f05-146">Se o seu produto for o Dynamics 365 e o produto escolhido tiver várias assinaturas para esse cliente específico, você também precisará inserir a ID da assinatura.</span><span class="sxs-lookup"><span data-stu-id="16f05-146">If your product is Dynamics 365, and the product you choose has multiple subscriptions for this particular customer, you'll also need to enter the subscription ID.</span></span>

10. <span data-ttu-id="16f05-147">Forneça sua PoE.</span><span class="sxs-lookup"><span data-stu-id="16f05-147">Supply your PoE.</span></span> <span data-ttu-id="16f05-148">Você pode arrastá-la para a caixa, navegar até sua própria documentação de apoio ou usar um modelo selecionando **Baixar modelo**.</span><span class="sxs-lookup"><span data-stu-id="16f05-148">You can drag it to the box, browse to your own supporting documentation, or use a template by selecting **Download template**.</span></span> 

11. <span data-ttu-id="16f05-149">Adicione e salve comentários, se desejar, e, em seguida, escolha **Enviar declaração**.</span><span class="sxs-lookup"><span data-stu-id="16f05-149">Add and save comments if you like, and then select **Submit claim**.</span></span> <span data-ttu-id="16f05-150">Enviaremos um email para o cliente solicitando aprovação da sua associação de cliente.</span><span class="sxs-lookup"><span data-stu-id="16f05-150">We'll send an email to the customer requesting approval of your customer association.</span></span>

   >[!NOTE]
   ><span data-ttu-id="16f05-151">Depois de enviar sua associação de cliente, você não poderá editá-la.</span><span class="sxs-lookup"><span data-stu-id="16f05-151">Once you submit your customer association, you can't edit it.</span></span>

<span data-ttu-id="16f05-152">O status da sua associação de cliente aparece no campo **Status**.</span><span class="sxs-lookup"><span data-stu-id="16f05-152">The status of your customer association appears in the **Status** field.</span></span>

<span data-ttu-id="16f05-153">Selecione **Histórico** para ver o histórico de uma associação de cliente.</span><span class="sxs-lookup"><span data-stu-id="16f05-153">Select **History** to view the history of a customer association.</span></span>

## <a name="next-steps"></a><span data-ttu-id="16f05-154">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="16f05-154">Next steps</span></span>

- [<span data-ttu-id="16f05-155">Gerenciar associações do cliente</span><span class="sxs-lookup"><span data-stu-id="16f05-155">Manage customer associations</span></span>](incentives-manage-customer-associations.md)