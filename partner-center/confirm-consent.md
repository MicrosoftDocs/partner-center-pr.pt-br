---
title: Confirmar a aceitação do cliente do Contrato de Cliente da Microsoft
description: Aprenda a confirmar a aceitação do cliente do Contrato de Cliente da Microsoft. Isso pode ser necessário para solicitar serviços e produtos da Microsoft para clientes.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/30/2020
ms.openlocfilehash: aacca72e9af45b2777364734c2b07dbe8101989d
ms.sourcegitcommit: 22af0997d52a87417b62f44fb0a7d711bec77b35
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/19/2020
ms.locfileid: "92333908"
---
# <a name="updated-method-to-confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a><span data-ttu-id="1701e-104">Atualização do método para confirmar a aceitação do cliente do Contrato de Cliente da Microsoft</span><span class="sxs-lookup"><span data-stu-id="1701e-104">Updated method to confirm customer acceptance of the Microsoft Customer Agreement</span></span>

<span data-ttu-id="1701e-105">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="1701e-105">**Applies to**</span></span>

-  <span data-ttu-id="1701e-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="1701e-106">Partner Center</span></span>

<span data-ttu-id="1701e-107">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="1701e-107">**Appropriate roles**</span></span>

- <span data-ttu-id="1701e-108">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="1701e-108">Admin agent</span></span>
- <span data-ttu-id="1701e-109">Agente de vendas</span><span class="sxs-lookup"><span data-stu-id="1701e-109">Sales agent</span></span>

> [!NOTE]
> <span data-ttu-id="1701e-110">No momento, há suporte para o recurso Contrato no Partner Center somente na nuvem pública da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1701e-110">The Agreement resource is currently supported by Partner Center in the Microsoft public cloud only.</span></span> <span data-ttu-id="1701e-111">Não é aplicável a:</span><span class="sxs-lookup"><span data-stu-id="1701e-111">It is not applicable to:</span></span>
> * <span data-ttu-id="1701e-112">Partner Center operado pela 21Vianet</span><span class="sxs-lookup"><span data-stu-id="1701e-112">Partner Center operated by 21Vianet</span></span>
> * <span data-ttu-id="1701e-113">Partner Center do Microsoft Cloud Germany</span><span class="sxs-lookup"><span data-stu-id="1701e-113">Partner Center for Microsoft Cloud Germany</span></span>
> * <span data-ttu-id="1701e-114">Partner Center do Microsoft Cloud for US Government</span><span class="sxs-lookup"><span data-stu-id="1701e-114">Partner Center for Microsoft Cloud for US Government</span></span>

>[!NOTE]
><span data-ttu-id="1701e-115">A partir de 31 de janeiro de 2020, todos os clientes, existentes e novos, devem assinar o novo Contrato de Cliente da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1701e-115">As of January 31, 2020, all customers, existing and new, must sign the new Microsoft Customer Agreement.</span></span> <span data-ttu-id="1701e-116">Para saber mais, leia [Confirmar a aceitação pelo cliente do Contrato de Cliente da Microsoft](confirm-customer-agreement.md).</span><span class="sxs-lookup"><span data-stu-id="1701e-116">To learn more, read [Confirm customer acceptance of the Microsoft Customer Agreement](confirm-customer-agreement.md).</span></span>

<span data-ttu-id="1701e-117">Como parceiro, você precisa obter a aceitação pelo cliente do Contrato de Cliente da Microsoft antes de poder solicitar produtos e serviços da Microsoft para esse cliente.</span><span class="sxs-lookup"><span data-stu-id="1701e-117">As a partner, you need to obtain your customer's acceptance of the Microsoft Customer Agreement before you can order Microsoft products and services for that customer.</span></span> <span data-ttu-id="1701e-118">Para ajudar mais os parceiros a atender os requisitos de conformidade, a Microsoft solicita que os parceiros confirmem a aceitação fornecendo os detalhes a seguir em relação à pessoa que aceitou o contrato:</span><span class="sxs-lookup"><span data-stu-id="1701e-118">To better help partners meet compliance requirements, Microsoft asks partners to confirm acceptance by providing the following details regarding the person who accepted the agreement:</span></span>

- <span data-ttu-id="1701e-119">Nome</span><span class="sxs-lookup"><span data-stu-id="1701e-119">First name</span></span>

- <span data-ttu-id="1701e-120">Sobrenome</span><span class="sxs-lookup"><span data-stu-id="1701e-120">Last name</span></span>

- <span data-ttu-id="1701e-121">Endereço de email</span><span class="sxs-lookup"><span data-stu-id="1701e-121">Email address</span></span>

- <span data-ttu-id="1701e-122">Número de telefone (opcional)</span><span class="sxs-lookup"><span data-stu-id="1701e-122">Phone number (optional)</span></span>

- <span data-ttu-id="1701e-123">Data da aceitação</span><span class="sxs-lookup"><span data-stu-id="1701e-123">Date of acceptance</span></span>

<span data-ttu-id="1701e-124">Parceiros de cobrança direta e Provedores Indiretos devem confirmar a aceitação pelo cliente do Contrato de Cliente da Microsoft ao fazer transações por meio do Partner Center ou da API do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="1701e-124">Direct bill partners and Indirect Providers must confirm customer acceptance of the Microsoft Customer Agreement when transacting through Partner Center or Partner Center API.</span></span> <span data-ttu-id="1701e-125">A confirmação é *obrigatória* .</span><span class="sxs-lookup"><span data-stu-id="1701e-125">Confirmation is *mandatory* .</span></span>

<span data-ttu-id="1701e-126">Se a confirmação não for fornecida por um determinado cliente:</span><span class="sxs-lookup"><span data-stu-id="1701e-126">If confirmation is not provided for a given customer:</span></span>

- <span data-ttu-id="1701e-127">Você não conseguirá criar pedidos para esse cliente.</span><span class="sxs-lookup"><span data-stu-id="1701e-127">You won't be able to create new orders for this customer.</span></span>

- <span data-ttu-id="1701e-128">Você não poderá alterar a contagem de licenças das assinaturas baseadas em licenças existentes para esse cliente.</span><span class="sxs-lookup"><span data-stu-id="1701e-128">You won't be able to change the license count of existing license-based subscriptions for this customer.</span></span>

<span data-ttu-id="1701e-129">A confirmação da aceitação pelo cliente poderá ser feita por meio do Partner Center ou da API do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="1701e-129">Confirmation of customer acceptance can be done via Partner Center or the Partner Center API.</span></span> <span data-ttu-id="1701e-130">Para fazer isso por meio da API do Partner Center, confira os seguintes tópicos:</span><span class="sxs-lookup"><span data-stu-id="1701e-130">To do this through the Partner Center API, see the following topics:</span></span>

- [<span data-ttu-id="1701e-131">Obter confirmação de consentimento do cliente</span><span class="sxs-lookup"><span data-stu-id="1701e-131">Get confirmation of customer consent</span></span>](/partner-center/develop/get-confirmation-of-customer-consent)

- [<span data-ttu-id="1701e-132">Obter metadados do contrato</span><span class="sxs-lookup"><span data-stu-id="1701e-132">Get agreement metadata</span></span>](/partner-center/develop/get-agreement-metadata)

- [<span data-ttu-id="1701e-133">Confirmar o consentimento do cliente</span><span class="sxs-lookup"><span data-stu-id="1701e-133">Confirm customer consent</span></span>](/partner-center/develop/confirm-customer-consent)

<span data-ttu-id="1701e-134">Isso se aplica a ambientes de produção e área restrita.</span><span class="sxs-lookup"><span data-stu-id="1701e-134">This applies to both production and sandbox environments.</span></span>

## <a name="confirm-customer-acceptance-for-a-new-customer"></a><span data-ttu-id="1701e-135">Confirmar a aceitação do cliente para um novo cliente</span><span class="sxs-lookup"><span data-stu-id="1701e-135">Confirm customer acceptance for a new customer</span></span>

<span data-ttu-id="1701e-136">Use o procedimento a seguir para confirmar a aceitação do cliente enquanto você cria um locatário do cliente no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="1701e-136">Use the following procedure to confirm customer acceptance while you create a new customer tenant in Partner Center.</span></span> <span data-ttu-id="1701e-137">Você deve ser um Agente administrativo ou Agente de vendas para fazer isso.</span><span class="sxs-lookup"><span data-stu-id="1701e-137">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="1701e-138">Selecione **Clientes** e, em seguida, **Novo cliente** e, em seguida, selecione **Informações da conta** .</span><span class="sxs-lookup"><span data-stu-id="1701e-138">Select **Customers** , and then **New customer** and then select **Account info** .</span></span>

2. <span data-ttu-id="1701e-139">Insira as informações sobre a **Empresa** e o **Contato principal** .</span><span class="sxs-lookup"><span data-stu-id="1701e-139">Enter the information about the **Company** and **Primary contact** .</span></span>

   :::image type="content" source="images/mca/mca1.png" alt-text="Informações da empresa":::

3. <span data-ttu-id="1701e-141">Em **contrato de cliente da Microsoft** , selecione **O cliente aceitou o contrato de cliente da Microsoft mais recente** .</span><span class="sxs-lookup"><span data-stu-id="1701e-141">Under **Microsoft customer agreement** , select **The customer has accepted the latest Microsoft customer agreement** .</span></span>

4. <span data-ttu-id="1701e-142">Em **Data de aceitação do contrato** , insira a data apropriada.</span><span class="sxs-lookup"><span data-stu-id="1701e-142">Under **Agreement acceptance date** , enter the appropriate date.</span></span> <span data-ttu-id="1701e-143">Você não pode definir isso como uma data futura.</span><span class="sxs-lookup"><span data-stu-id="1701e-143">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="1701e-144">Insira os detalhes do usuário que forneceu a aceitação.</span><span class="sxs-lookup"><span data-stu-id="1701e-144">Enter the details of the user who provided the acceptance.</span></span>

   :::image type="content" source="images/mca/MCA3.png" alt-text="Adicionar data de aceitação":::

   <span data-ttu-id="1701e-146">Por padrão, as informações de usuário do contato principal são exibidas.</span><span class="sxs-lookup"><span data-stu-id="1701e-146">By default, the primary contact user information is displayed.</span></span> <span data-ttu-id="1701e-147">Se isso não estiver correto, selecione **Atualizar** e insira o **Nome** , **Sobrenome** , **Endereço de email** e \* *Número de telefone* (opcional) da pessoa que aceitou o contrato.</span><span class="sxs-lookup"><span data-stu-id="1701e-147">If this isn't correct, select **Update** and then enter the **First name** , **Last name** , **Email address** , and \* *Phone number* (optional) of the person who accepted the agreement.</span></span>

6. <span data-ttu-id="1701e-148">Selecione **Avançar** para continuar com as etapas restantes para criar o locatário do cliente.</span><span class="sxs-lookup"><span data-stu-id="1701e-148">Select **Next** to continue with the remaining steps to create the customer tenant.</span></span>

## <a name="confirm-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="1701e-149">Confirmar a aceitação do cliente para um cliente existente</span><span class="sxs-lookup"><span data-stu-id="1701e-149">Confirm customer acceptance for an existing customer</span></span>

<span data-ttu-id="1701e-150">Você deve ser um Agente administrativo ou Agente de vendas para fazer isso.</span><span class="sxs-lookup"><span data-stu-id="1701e-150">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="1701e-151">Selecione **Clientes** e então localize e selecione o cliente que você deseja ver.</span><span class="sxs-lookup"><span data-stu-id="1701e-151">Select **Customers** , and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="1701e-152">Selecione **Informações da Conta** .</span><span class="sxs-lookup"><span data-stu-id="1701e-152">Select **Account info** .</span></span>

3. <span data-ttu-id="1701e-153">Em **Contrato de cliente da Microsoft** , selecione **Atualizar** .</span><span class="sxs-lookup"><span data-stu-id="1701e-153">Under **Microsoft customer agreement** , select **Update** .</span></span>

   :::image type="content" source="images/mca/mca4.png" alt-text="Atualização":::

4. <span data-ttu-id="1701e-155">Insira o **Nome** , **Sobrenome** , **Endereço de email** e **Número de telefone** (opcional) do usuário que aceitou o contrato.</span><span class="sxs-lookup"><span data-stu-id="1701e-155">Enter the **First name** , **Last name** , **Email address** , and **Phone number** (optional) of the user who accepted the agreement.</span></span>

5. <span data-ttu-id="1701e-156">Em **Data de aceitação do contrato** , insira a data apropriada.</span><span class="sxs-lookup"><span data-stu-id="1701e-156">Under **Agreement acceptance date** , enter the appropriate date.</span></span> <span data-ttu-id="1701e-157">Você não pode definir isso como uma data futura.</span><span class="sxs-lookup"><span data-stu-id="1701e-157">You cannot set this to a future date.</span></span>

6. <span data-ttu-id="1701e-158">Selecione **Salvar e continuar** .</span><span class="sxs-lookup"><span data-stu-id="1701e-158">Select **Save and continue** .</span></span>

## <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a><span data-ttu-id="1701e-159">Confirmar a aceitação do cliente ao criar o pedido para um cliente existente</span><span class="sxs-lookup"><span data-stu-id="1701e-159">Confirm customer acceptance while creating new order for an existing customer</span></span>

<span data-ttu-id="1701e-160">Se você tentar criar um pedido para um cliente existente que não fez a confirmação antes, receberá um aviso para concluir a confirmação.</span><span class="sxs-lookup"><span data-stu-id="1701e-160">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="1701e-161">Use o procedimento a seguir para fazer isso.</span><span class="sxs-lookup"><span data-stu-id="1701e-161">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="1701e-162">Insira o **Nome** , **Sobrenome** , **Endereço de email** e **Número de telefone** (opcional) do usuário que aceitou o contrato.</span><span class="sxs-lookup"><span data-stu-id="1701e-162">Enter the **First name** , **Last name** , **Email address** , and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="1701e-163">Em **Data de aceitação do contrato** , insira a data apropriada.</span><span class="sxs-lookup"><span data-stu-id="1701e-163">Under **Agreement acceptance date** , enter the appropriate date.</span></span> <span data-ttu-id="1701e-164">Você não pode definir isso como uma data futura.</span><span class="sxs-lookup"><span data-stu-id="1701e-164">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="1701e-165">Selecione **Salvar e continuar** .</span><span class="sxs-lookup"><span data-stu-id="1701e-165">Select **Save and continue** .</span></span>

## <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a><span data-ttu-id="1701e-166">Recuperar a confirmação da aceitação do cliente para um cliente existente</span><span class="sxs-lookup"><span data-stu-id="1701e-166">Retrieve confirmation of customer acceptance for an existing customer</span></span>

<span data-ttu-id="1701e-167">Você pode recuperar a confirmação da aceitação do cliente para um cliente existente que você forneceu anteriormente usando o procedimento abaixo.</span><span class="sxs-lookup"><span data-stu-id="1701e-167">You can retrieve confirmation of customer acceptance for an existing customer that you have provided previously using the procedure below.</span></span> <span data-ttu-id="1701e-168">Você deve ser um Agente administrativo ou Agente de vendas para fazer isso.</span><span class="sxs-lookup"><span data-stu-id="1701e-168">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="1701e-169">Selecione **Clientes** e então localize e selecione o cliente que você deseja ver.</span><span class="sxs-lookup"><span data-stu-id="1701e-169">Select **Customers** , and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="1701e-170">Selecione **Informações da Conta** .</span><span class="sxs-lookup"><span data-stu-id="1701e-170">Select **Account info** .</span></span>

3. <span data-ttu-id="1701e-171">Em **Contrato de cliente da Microsoft** , você verá se a confirmação foi fornecida ou não para este cliente.</span><span class="sxs-lookup"><span data-stu-id="1701e-171">Under **Microsoft customer agreement** , you'll see whether or not confirmation has been provided for this customer.</span></span>

## <a name="next-steps"></a><span data-ttu-id="1701e-172">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="1701e-172">Next steps</span></span>

- [<span data-ttu-id="1701e-173">Confirmar a aceitação do Contrato de Cliente da Microsoft pelo cliente no programa de parceiro CSP</span><span class="sxs-lookup"><span data-stu-id="1701e-173">Confirm customer acceptance of the Microsoft Customer Agreement in the CSP partner program</span></span>](confirm-customer-agreement.md)

- [<span data-ttu-id="1701e-174">Atestar a aceitação do Contrato de Cliente da Microsoft em nome do seu cliente</span><span class="sxs-lookup"><span data-stu-id="1701e-174">Attest acceptance of the Microsoft Customer Agreement on behalf of your customer</span></span>](attest-acceptance-customer-agreement.md)