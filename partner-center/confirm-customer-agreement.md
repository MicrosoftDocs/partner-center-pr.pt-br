---
title: Como confirmar se o cliente aceitou o Contrato de Cliente da Microsoft para o programa CSP
description: Os parceiros do CSP (Provedor de Soluções na Nuvem) precisam confirmar a aceitação do Contrato de Cliente da Microsoft pelo cliente antes de solicitar os serviços Microsoft para os clientes.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: ebb52a3a8223d3b1101e3a8e78728fcc167e25e3
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633770"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a><span data-ttu-id="766e2-103">Como confirmar se o cliente aceitou o Contrato de Cliente da Microsoft para o programa CSP</span><span class="sxs-lookup"><span data-stu-id="766e2-103">How to confirm that your customer has accepted the Microsoft Customer Agreement to the CSP program</span></span>

<span data-ttu-id="766e2-104">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="766e2-104">**Appropriate roles**</span></span>

- <span data-ttu-id="766e2-105">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="766e2-105">Admin agent</span></span>
- <span data-ttu-id="766e2-106">Agente de vendas</span><span class="sxs-lookup"><span data-stu-id="766e2-106">Sales agent</span></span>


<span data-ttu-id="766e2-107">Os clientes têm duas opções para aceitar o Contrato de Cliente da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="766e2-107">Customers have two options for how they accept the Microsoft Customer Agreement.</span></span>

<span data-ttu-id="766e2-108">**Opção 1**: Atestado do parceiro da aceitação do cliente – o parceiro pode confirmar a aceitação do cliente usando o SDK/a API do Partner Center ou pelo painel do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="766e2-108">**Option 1**: Partner attestation of customer acceptance - Partner can confirm customer acceptance using Partner Center API/SDK or through the Partner Center dashboard.</span></span>

<span data-ttu-id="766e2-109">**Opção 2**: Aceitação direta do cliente – o parceiro pode convidar o cliente por uma URL para examinar e aceitar o contrato no Centro de administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="766e2-109">**Option 2**: Customer direct acceptance - Partner can invite the customer via a URL to review and accept the agreement in the Microsoft 365 Admin Center.</span></span>

## <a name="access-microsoft-customer-agreement-template"></a><span data-ttu-id="766e2-110">Acessar o modelo do Contrato de Cliente da Microsoft</span><span class="sxs-lookup"><span data-stu-id="766e2-110">Access Microsoft Customer Agreement template</span></span>

<span data-ttu-id="766e2-111">Você pode baixar manualmente a última versão do modelo do Contrato de Cliente da Microsoft [aqui](https://aka.ms/customeragreement).</span><span class="sxs-lookup"><span data-stu-id="766e2-111">You can manually download the latest version of the Microsoft Customer Agreement template from [here](https://aka.ms/customeragreement).</span></span> <span data-ttu-id="766e2-112">O Contrato de Cliente da Microsoft é específico para cada país.</span><span class="sxs-lookup"><span data-stu-id="766e2-112">The Microsoft Customer Agreement is country-specific.</span></span> <span data-ttu-id="766e2-113">Ao solicitar o modelo do Contrato de Cliente da Microsoft, selecione o país correto com base no local do cliente.</span><span class="sxs-lookup"><span data-stu-id="766e2-113">When requesting the Microsoft Customer Agreement template, be sure to select the correct country based on the customer's location.</span></span>

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a><span data-ttu-id="766e2-114">Opção 1: Confirmar a aceitação do cliente no Partner Center</span><span class="sxs-lookup"><span data-stu-id="766e2-114">Option 1: Confirm customer acceptance in Partner Center</span></span>

<span data-ttu-id="766e2-115">Os parceiros de fatura direta podem confirmar a aceitação do Contrato de Cliente da Microsoft pelo cliente no Partner Center para clientes novos e existentes.</span><span class="sxs-lookup"><span data-stu-id="766e2-115">Direct bill partners can confirm customer acceptance of the Microsoft Customer Agreement in Partner Center for new and existing customers.</span></span> <span data-ttu-id="766e2-116">Os revendedores indiretos não podem atestar em nome de seus clientes e precisam trabalhar com seu Provedor Indireto para que o atestado seja concluído.</span><span class="sxs-lookup"><span data-stu-id="766e2-116">Indirect resellers cannot attest on behalf of their customers and need to work with their Indirect Provider to get attestation completed.</span></span>

### <a name="confirm-customer-acceptance-for-new-customers"></a><span data-ttu-id="766e2-117">Confirmar a aceitação do cliente para novos clientes</span><span class="sxs-lookup"><span data-stu-id="766e2-117">Confirm customer acceptance for new customers</span></span>

<span data-ttu-id="766e2-118">Ao criar um novo locatário do cliente no Partner Center, use as etapas a seguir para confirmar a aceitação do cliente do contrato do cliente da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="766e2-118">When you create a new customer tenant in Partner Center, use the following steps to confirm the customer's acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="766e2-119">Você deve ser um agente de administração ou um agente de vendas para executar essas etapas.</span><span class="sxs-lookup"><span data-stu-id="766e2-119">You must be an Admin agent or Sales agent to perform these steps.</span></span>

1. <span data-ttu-id="766e2-120">Selecione **Clientes** e então **Novo cliente**.</span><span class="sxs-lookup"><span data-stu-id="766e2-120">Select **Customers**, and then **New customer**.</span></span>

2. <span data-ttu-id="766e2-121">Em **informações da conta**, insira informações para a empresa e seu contato principal.</span><span class="sxs-lookup"><span data-stu-id="766e2-121">Under **Account info**, enter information for the company and its primary contact.</span></span>

3. <span data-ttu-id="766e2-122">Em **Contrato da Microsoft**, marque a caixa para atestar que o cliente aceitou o Contrato de Cliente da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="766e2-122">Under **Microsoft agreement**, select the box to attest that the customer has accepted the Microsoft Customer Agreement.</span></span>

4. <span data-ttu-id="766e2-123">Em **Data de aceitação do contrato**, insira a data apropriada.</span><span class="sxs-lookup"><span data-stu-id="766e2-123">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="766e2-124">Você não pode definir isso como uma data futura.</span><span class="sxs-lookup"><span data-stu-id="766e2-124">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="766e2-125">Verifique se as informações de contato do usuário primário exibidas estão corretas.</span><span class="sxs-lookup"><span data-stu-id="766e2-125">Make sure that the primary user contact information displayed is correct.</span></span> <span data-ttu-id="766e2-126">Se estiver incorreto, selecione **Atualizar** e insira as informações corretas da pessoa que aceitou o contrato.</span><span class="sxs-lookup"><span data-stu-id="766e2-126">If it's incorrect, select **Update** and enter the accurate information for the person who accepted the agreement.</span></span>

6. <span data-ttu-id="766e2-127">Selecione **Avançar** para continuar criando o locatário do cliente.</span><span class="sxs-lookup"><span data-stu-id="766e2-127">Select **Next** to continue creating the customer tenant.</span></span>

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Novo cliente":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a><span data-ttu-id="766e2-129">Confirmar a aceitação do cliente para clientes existentes</span><span class="sxs-lookup"><span data-stu-id="766e2-129">Confirm customer acceptance for existing customers</span></span>

<span data-ttu-id="766e2-130">Você deve ser um Agente administrativo ou Agente de vendas para fazer isto:</span><span class="sxs-lookup"><span data-stu-id="766e2-130">You must be an Admin agent or Sales agent to do this:</span></span>

1. <span data-ttu-id="766e2-131">Selecione **Clientes**.</span><span class="sxs-lookup"><span data-stu-id="766e2-131">Select **Customers**.</span></span> <span data-ttu-id="766e2-132">Localize e selecione o cliente.</span><span class="sxs-lookup"><span data-stu-id="766e2-132">Find and select the customer.</span></span>

2. <span data-ttu-id="766e2-133">Selecione **Informações da Conta**.</span><span class="sxs-lookup"><span data-stu-id="766e2-133">Select **Account info**.</span></span>

3. <span data-ttu-id="766e2-134">Em **Contrato de Cliente da Microsoft**, selecione **Atualizar**.</span><span class="sxs-lookup"><span data-stu-id="766e2-134">Under **Microsoft Customer Agreement**, select **Update**.</span></span>

4. <span data-ttu-id="766e2-135">Insira o **Nome**, **Sobrenome**, **E-mail** e **Número de telefone** (opcional) do usuário que aceitou o contrato.</span><span class="sxs-lookup"><span data-stu-id="766e2-135">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the person who accepted the agreement.</span></span> <span data-ttu-id="766e2-136">Em **Data de aceitação do contrato**, insira a data apropriada.</span><span class="sxs-lookup"><span data-stu-id="766e2-136">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="766e2-137">Você não pode definir isso como uma data futura.</span><span class="sxs-lookup"><span data-stu-id="766e2-137">You cannot set this to a future date.</span></span>

5. <span data-ttu-id="766e2-138">Selecione **Salvar** e continue.</span><span class="sxs-lookup"><span data-stu-id="766e2-138">Select **Save** and continue.</span></span>

   :::image type="content" source="images/mcua2-update2.png" alt-text="Cliente existente":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a><span data-ttu-id="766e2-140">Recuperar confirmação de aceitação do cliente</span><span class="sxs-lookup"><span data-stu-id="766e2-140">Retrieve confirmation of customer acceptance</span></span>

<span data-ttu-id="766e2-141">Para recuperar a confirmação de que um cliente existente aceitou o Contrato de Cliente da Microsoft, use as etapas a seguir.</span><span class="sxs-lookup"><span data-stu-id="766e2-141">To retrieve confirmation that an existing customer has accepted the Microsoft Customer Agreement, use the following steps.</span></span> <span data-ttu-id="766e2-142">Você deve ser um Agente administrativo ou Agente de vendas para fazer isso.</span><span class="sxs-lookup"><span data-stu-id="766e2-142">You must be an Admin agent or Sales agent to do this.</span></span>

1. <span data-ttu-id="766e2-143">Selecione **Clientes** e então localize e selecione o cliente que você deseja ver.</span><span class="sxs-lookup"><span data-stu-id="766e2-143">Select **Customers**, and then find and select the customer you want to see.</span></span>

2. <span data-ttu-id="766e2-144">Selecione **Informações da Conta**.</span><span class="sxs-lookup"><span data-stu-id="766e2-144">Select **Account info**.</span></span>

3. <span data-ttu-id="766e2-145">Em **contrato de cliente da Microsoft**, veja se a confirmação tem ou não foi fornecida por este cliente.</span><span class="sxs-lookup"><span data-stu-id="766e2-145">Under **Microsoft customer agreement**, view if confirmation has or hasn't been provided by this customer.</span></span>

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a><span data-ttu-id="766e2-146">Confirmar a aceitação do cliente usando o SDK/a API do Partner Center</span><span class="sxs-lookup"><span data-stu-id="766e2-146">Confirm customer acceptance using Partner Center API/SDK</span></span>

<span data-ttu-id="766e2-147">Você pode usar o SDK/a API do Partner Center para confirmar a aceitação do cliente do Contrato de Cliente da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="766e2-147">You can use Partner Center API/SDK to confirm customer acceptance of the Microsoft Customer Agreement.</span></span> <span data-ttu-id="766e2-148">Para obter detalhes sobre a API ou o SDK, confira:</span><span class="sxs-lookup"><span data-stu-id="766e2-148">For details on the API/SDK, refer to:</span></span>

- [<span data-ttu-id="766e2-149">Obter metadados do Contrato de Cliente da Microsoft</span><span class="sxs-lookup"><span data-stu-id="766e2-149">Get agreement metadata for the Microsoft Customer Agreement</span></span>](/partner-center/develop/get-customer-agreement-metadata)

- [<span data-ttu-id="766e2-150">Confirmar a aceitação do cliente do Contrato de Cliente da Microsoft</span><span class="sxs-lookup"><span data-stu-id="766e2-150">Confirm customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [<span data-ttu-id="766e2-151">Obter a confirmação da aceitação do Contrato de Cliente da Microsoft pelo cliente</span><span class="sxs-lookup"><span data-stu-id="766e2-151">Get confirmation of customer acceptance of Microsoft Customer Agreement</span></span>](/partner-center/develop/get-confirmation-of-customer-agreement)

- [<span data-ttu-id="766e2-152">Obter um link de download para o modelo do Contrato de Cliente da Microsoft</span><span class="sxs-lookup"><span data-stu-id="766e2-152">Get a download link for the Microsoft Customer Agreement template</span></span>](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a><span data-ttu-id="766e2-153">Opção 2: Aceitação do cliente no Centro de administração do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="766e2-153">Option 2: Customer acceptance in Microsoft 365 Admin Center</span></span>

<span data-ttu-id="766e2-154">Os parceiros podem convidar clientes novos e existentes, por meio de uma URL, para revisar e aceitar o contrato dentro do Centro de administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="766e2-154">Partners can invite new and existing customers, via a URL, to review and accept the agreement within the Microsoft 365 Admin Center.</span></span> <span data-ttu-id="766e2-155">As próximas seções mostram como:</span><span class="sxs-lookup"><span data-stu-id="766e2-155">The next few sections show you how to:</span></span>

- <span data-ttu-id="766e2-156">Criar um cliente e convidá-lo a examinar e aceitar o contrato.</span><span class="sxs-lookup"><span data-stu-id="766e2-156">Create a new customer and invite the customer to review and accept the agreement.</span></span>

- <span data-ttu-id="766e2-157">Convidar um novo cliente para examinar e aceitar a relação e o contrato do revendedor.</span><span class="sxs-lookup"><span data-stu-id="766e2-157">Invite a new customer to review and accept the reseller relationship and agreement.</span></span>

- <span data-ttu-id="766e2-158">Convidar um cliente existente para examinar e aceitar o contrato.</span><span class="sxs-lookup"><span data-stu-id="766e2-158">Invite an existing customer to review and accept the agreement.</span></span>

>[!NOTE]
> <span data-ttu-id="766e2-159">Você pode usar [o SDK ou a API do Partner Center](/partner-center/develop/get-direct-sign-status-of-customer-agreement) para confirmar o status da aceitação direta do cliente do Contrato de Cliente da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="766e2-159">You can use [Partner Center API/SDK](/partner-center/develop/get-direct-sign-status-of-customer-agreement) to get the status of a customer's direct acceptance of the Microsoft Customer Agreement.</span></span>  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="766e2-160">Criar um cliente e convidá-lo a examinar e aceitar o contrato</span><span class="sxs-lookup"><span data-stu-id="766e2-160">Create a new customer and invite the customer to review and accept the agreement</span></span>

<span data-ttu-id="766e2-161">Use as etapas a seguir para criar um cliente no Partner Center e convidá-lo a revisar e aceitar o Contrato de Cliente da Microsoft dentro do Centro de administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="766e2-161">Use the following steps to create a new customer in Partner Center then invite them to review and accept the Microsoft Customer Agreement within Microsoft 365 Admin Center.</span></span>

1. <span data-ttu-id="766e2-162">Na guia **Clientes** no Partner Center, selecione **Adicionar cliente**.</span><span class="sxs-lookup"><span data-stu-id="766e2-162">From the **Customers** tab within Partner Center, select **Add customer**.</span></span>

2. <span data-ttu-id="766e2-163">Em **Informações sobre a conta**, insira as informações sobre o novo cliente em todos os campos obrigatórios, incluindo o nome da empresa e o contato principal do cliente.</span><span class="sxs-lookup"><span data-stu-id="766e2-163">Under **Account Info**, enter information about the new customer in all required fields, including the customer's company name and primary contact.</span></span>

3. <span data-ttu-id="766e2-164">Em **Contrato de Cliente**, selecione a opção **Será solicitado que o cliente aceite o Contrato de Cliente da Microsoft no Centro de Administração do Microsoft 365**.</span><span class="sxs-lookup"><span data-stu-id="766e2-164">Under **Customer Agreement**, select **Customer will be asked to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center**.</span></span> <span data-ttu-id="766e2-165">Preencha todos os outros campos obrigatórios na página.</span><span class="sxs-lookup"><span data-stu-id="766e2-165">Complete any other required fields on the page.</span></span>

4. <span data-ttu-id="766e2-166">Selecione **Avançar: Examinar**. Em seguida, prossiga com as etapas para criar o locatário do cliente.</span><span class="sxs-lookup"><span data-stu-id="766e2-166">Select **Next: Review** then continue the steps to create the customer tenant.</span></span> 

>[!NOTE] 
><span data-ttu-id="766e2-167">Novos clientes não podem fazer uma compra até aceitarem o Contrato de Cliente da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="766e2-167">New customers cannot make a purchase until they accept the Microsoft Customer Agreement.</span></span>  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Criar cliente":::

5. <span data-ttu-id="766e2-169">Ao acessar a tela de **Confirmação** no novo fluxo de trabalho do cliente, salve as credenciais dele.</span><span class="sxs-lookup"><span data-stu-id="766e2-169">When you reach the **Confirmation** screen in the new customer workflow, save the customer credentials.</span></span> <span data-ttu-id="766e2-170">Você precisará fornecer essas credenciais para o cliente mais tarde.</span><span class="sxs-lookup"><span data-stu-id="766e2-170">You will need to give these credentials to your customer later.</span></span>

6. <span data-ttu-id="766e2-171">Fora do Partner Center, crie e envie um email que convida o cliente a aceitar o Contrato de Cliente da Microsoft no Centro de administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="766e2-171">Outside of Partner Center, create and send an email that invites the customer to accept the Microsoft Customer Agreement in Microsoft 365 Admin Center.</span></span> <span data-ttu-id="766e2-172">Inclua estes itens no email:</span><span class="sxs-lookup"><span data-stu-id="766e2-172">Make sure to include these items in the email:</span></span>

   - <span data-ttu-id="766e2-173">Um link para esta [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (é necessário se conectar)</span><span class="sxs-lookup"><span data-stu-id="766e2-173">A link to this [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (Sign-in required)</span></span>

   - <span data-ttu-id="766e2-174">As credenciais do cliente que você salvou na Etapa 5.</span><span class="sxs-lookup"><span data-stu-id="766e2-174">The customer's credentials that you saved in Step 5.</span></span>

7. <span data-ttu-id="766e2-175">O cliente receberá o convite por email do parceiro e selecionará a [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span><span class="sxs-lookup"><span data-stu-id="766e2-175">The customer will then receive the email invite from the partner and select the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span>

8. <span data-ttu-id="766e2-176">O cliente entra no Centro de Administração do Microsoft 365 usando as credenciais do cliente que você forneceu.</span><span class="sxs-lookup"><span data-stu-id="766e2-176">The customer signs into Microsoft 365 Admin Center using the customer credentials you provided.</span></span>

9. <span data-ttu-id="766e2-177">O cliente marca a caixa para aceitar o Contrato de Cliente da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="766e2-177">The customer checks the box to accept the Microsoft Customer agreement.</span></span>

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a><span data-ttu-id="766e2-178">Convidar um novo cliente para revisar e aceitar a relação de revendedor e o Contrato de Cliente da Microsoft</span><span class="sxs-lookup"><span data-stu-id="766e2-178">Invite a new customer to review and accept the reseller relationship and Microsoft Customer Agreement</span></span> 

<span data-ttu-id="766e2-179">Use as etapas a seguir para convidar um novo cliente a revisar e aceitar a relação de revendedor e o Contrato de Cliente da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="766e2-179">Use the following steps to invite a new customer to review and accept the reseller relationship and the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="766e2-180">Na guia **Clientes** no Partner Center, selecione o link **Solicitar uma relação de revendedor**.</span><span class="sxs-lookup"><span data-stu-id="766e2-180">From the **Customers** tab within Partner Center, select **Request a reseller relationship** link.</span></span> 

2. <span data-ttu-id="766e2-181">Um modelo de email automático será gerado, incluindo um texto e uma URL parametrizada que direcionará o cliente para o Centro de Administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="766e2-181">An automatic email template will be generated, including text and a parameterized URL that directs the customer to the Microsoft 365 Admin Center.</span></span>

3. <span data-ttu-id="766e2-182">Você pode personalizar o modelo de email gerado automaticamente e, em seguida, selecionar **Copiar para a área de transferência** ou **Abrir no email**.</span><span class="sxs-lookup"><span data-stu-id="766e2-182">You can customize the automatically generated email template and then select **Copy to clipboard** or **Open in email**.</span></span>

4. <span data-ttu-id="766e2-183">Use este modelo de email para convidar o cliente a aceitar a solicitação de **relação de revendedor** e o **Contrato de Cliente da Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="766e2-183">Use this email template to invite the customer to accept **reseller relationship** request and the **Microsoft Customer Agreement**.</span></span> <span data-ttu-id="766e2-184">(Observação: no convite por email, verifique se o parceiro também inclui a URL fornecida automaticamente, assim como as credenciais do cliente criadas recentemente.)</span><span class="sxs-lookup"><span data-stu-id="766e2-184">(Note: In the email invite, make sure the partner also includes the URL that was automatically provided as well as the customer credentials that were recently created.)</span></span>

   :::image type="content" source="images/mca/createrelationship.png" alt-text="criar uma relação":::

5. <span data-ttu-id="766e2-186">O cliente recebe o convite por email e clica na URL parametrizada.</span><span class="sxs-lookup"><span data-stu-id="766e2-186">Customer receives invite via email and clicks on the parameterized URL.</span></span> 

6. <span data-ttu-id="766e2-187">O cliente usa as credenciais fornecidas por você no email para entrar no Centro de Administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="766e2-187">Customer uses credentials you provide within email to sign into Microsoft 365 Admin Center.</span></span>

7. <span data-ttu-id="766e2-188">O cliente marca a caixa para aceitar a **relação de revendedor** e o **Contrato de Cliente da Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="766e2-188">Customer checks the box to accept the **reseller relationship** and **Microsoft Customer Agreement**.</span></span> 

8. <span data-ttu-id="766e2-189">Na mesma URL, o cliente pode ver uma lista consolidada de diferentes parceiros com os quais ele está trabalhando.</span><span class="sxs-lookup"><span data-stu-id="766e2-189">Within the same URL, the customer is able to see a consolidated list of different partners they are working with.</span></span> <span data-ttu-id="766e2-190">Ele pode selecionar um parceiro para ver os detalhes.</span><span class="sxs-lookup"><span data-stu-id="766e2-190">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/accept.jpg" alt-text="Aceitar o contrato":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a><span data-ttu-id="766e2-192">Convidar um cliente existente para revisar e aceitar o contrato</span><span class="sxs-lookup"><span data-stu-id="766e2-192">Invite an existing customer to review and accept the agreement</span></span>

<span data-ttu-id="766e2-193">Use as etapas a seguir para convidar um cliente existente a revisar e aceitar o Contrato de Cliente da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="766e2-193">Use the following steps to invite an existing customer to review and accept the Microsoft Customer Agreement.</span></span> 

1. <span data-ttu-id="766e2-194">Crie o email do cliente com a URL inserida que convida seu cliente a aceitar o Contrato de Cliente da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="766e2-194">Create the customer email with the embedded URL inviting your customer to accept the Microsoft Customer Agreement.</span></span>

2. <span data-ttu-id="766e2-195">O cliente recebe o convite por email e clica na [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span><span class="sxs-lookup"><span data-stu-id="766e2-195">Your customer receives the invitation via email and clicks the [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).</span></span> 

3. <span data-ttu-id="766e2-196">O cliente insere as credenciais dele no Centro de administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="766e2-196">The customer enters their credentials into Microsoft 365 Admin Center.</span></span>

4. <span data-ttu-id="766e2-197">Seu cliente marca a caixa para aceitar o Contrato de Cliente da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="766e2-197">Your customer checks the box to accept the Microsoft Customer Agreement.</span></span> 

5. <span data-ttu-id="766e2-198">Na mesma URL, o cliente pode ver a lista consolidada de diferentes parceiros com os quais eles estão trabalhando.</span><span class="sxs-lookup"><span data-stu-id="766e2-198">Within the same URL, the customer can see the consolidated list of different partners they are working with.</span></span> <span data-ttu-id="766e2-199">Ele pode selecionar um parceiro para ver os detalhes.</span><span class="sxs-lookup"><span data-stu-id="766e2-199">They can select a partner to see details.</span></span>

   :::image type="content" source="images/mca/customeraccept.png" alt-text="cliente":::

>[!NOTE]
><span data-ttu-id="766e2-201">Em determinados cenários, os clientes talvez não possam aceitar diretamente o Contrato de Cliente da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="766e2-201">In certain scenarios, customers may not be able to directly accept the Microsoft Customer Agreement.</span></span> <span data-ttu-id="766e2-202">Para saber mais sobre essas situações, leia a próxima seção: Dois cenários em que você precisa atestar em nome do cliente.</span><span class="sxs-lookup"><span data-stu-id="766e2-202">To learn more about these situations, read Two scenarios where you need to attest on behalf of your customer, below.</span></span>

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a><span data-ttu-id="766e2-203">Dois cenários em que você precisa atestar em nome do seu cliente</span><span class="sxs-lookup"><span data-stu-id="766e2-203">Two scenarios where you need to attest on behalf of your customer</span></span>

<span data-ttu-id="766e2-204">Há dois cenários em que os clientes talvez não possam aceitar diretamente o Contrato de Cliente da Microsoft dentro do Centro de Administração do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="766e2-204">There are two scenarios where customers may not be able to directly accept the Microsoft Customer Agreement within the Microsoft 365 Admin Center.</span></span>

<span data-ttu-id="766e2-205">**Cenário 1**: um cliente existente comprou qualquer um dos seguintes itens por meio de um relacionamento com o parceiro existente: ofertas, software ou assinaturas de software, Instâncias Reservadas ou o Plano do Azure.</span><span class="sxs-lookup"><span data-stu-id="766e2-205">**Scenario 1**: An existing customer has purchased any of the following through an existing partner relationship: offers, software or software subscriptions, Reserved Instances, or Azure Plan.</span></span> <span data-ttu-id="766e2-206">Agora, o cliente está tentando fazer qualquer nova compra (excluindo a renovação automática).</span><span class="sxs-lookup"><span data-stu-id="766e2-206">The customer is now attempting to make any new purchase (excluding auto renewal).</span></span> <span data-ttu-id="766e2-207">Quando esse cliente clicar na URL, receberá a mensagem “Entre em contato com seu Parceiro para confirmar a aceitação do Contrato de Cliente da Microsoft”.</span><span class="sxs-lookup"><span data-stu-id="766e2-207">When that customer clicks the URL, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="766e2-208">**Para resolver**: você deve atestar em nome do cliente.</span><span class="sxs-lookup"><span data-stu-id="766e2-208">**To resolve**: You must attest on behalf of the customer.</span></span>

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Captura de tela da página do Centro de administração do Microsoft 365 solicitando que você entre em contato com seu parceiro para confirmar a aceitação do Contrato de Cliente da Microsoft.":::

<span data-ttu-id="766e2-210">**Cenário 2**: um cliente comprou uma das seguintes ofertas, softwares ou assinaturas de software, Instâncias Reservadas ou Plano do Azure.</span><span class="sxs-lookup"><span data-stu-id="766e2-210">**Scenario 2**: An existing customer has purchased any of the following offers, software and software subscriptions, Reserved Instances, and Azure Plan.</span></span> <span data-ttu-id="766e2-211">Agora, o cliente está tentando fazer qualquer nova compra com um novo parceiro.</span><span class="sxs-lookup"><span data-stu-id="766e2-211">The customer is now attempting to make any new purchase with a new partner.</span></span>

<span data-ttu-id="766e2-212">Quando o cliente clicar na URL para o Centro de administração do Microsoft 365 para aceitar o novo relacionamento com o parceiro e o contrato, ele receberá a mensagem “Entre em contato com seu Parceiro para confirmar sua aceitação do Contrato de Cliente da Microsoft”.</span><span class="sxs-lookup"><span data-stu-id="766e2-212">When the customer clicks the URL to Microsoft 365 Admin Center to accept the new partner relationship and the agreement, they will receive the message "Please reach out to your Partner to confirm your acceptance of the Microsoft Customer Agreement."</span></span>  

<span data-ttu-id="766e2-213">**Para resolver**: você deve atestar em nome do cliente.</span><span class="sxs-lookup"><span data-stu-id="766e2-213">**To resolve**: You must attest on behalf of the customer.</span></span>  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a><span data-ttu-id="766e2-214">Confirmar que um cliente aceitou o contrato</span><span class="sxs-lookup"><span data-stu-id="766e2-214">Confirm that a customer has accepted the agreement</span></span>

<span data-ttu-id="766e2-215">Se você tentar criar um pedido para um cliente existente que não fez a confirmação antes, receberá um aviso para concluir a confirmação.</span><span class="sxs-lookup"><span data-stu-id="766e2-215">If you try to create a new order for an existing customer who you have not confirmed before, you'll receive a prompt to complete the confirmation.</span></span> <span data-ttu-id="766e2-216">Use o procedimento a seguir para fazer isso.</span><span class="sxs-lookup"><span data-stu-id="766e2-216">Use the following procedure to do this.</span></span>

1. <span data-ttu-id="766e2-217">Insira o **Nome**, **Sobrenome**, **Endereço de email** e **Número de telefone** (opcional) do usuário que aceitou o contrato.</span><span class="sxs-lookup"><span data-stu-id="766e2-217">Enter the **First name**, **Last name**, **Email address**, and **Phone number** (optional) of the user who accepted the agreement.</span></span>

2. <span data-ttu-id="766e2-218">Em **Data de aceitação do contrato**, insira a data apropriada.</span><span class="sxs-lookup"><span data-stu-id="766e2-218">Under **Agreement acceptance date**, enter the appropriate date.</span></span> <span data-ttu-id="766e2-219">Você não pode definir isso como uma data futura.</span><span class="sxs-lookup"><span data-stu-id="766e2-219">You cannot set this to a future date.</span></span>

3. <span data-ttu-id="766e2-220">Selecione **Salvar e continuar**.</span><span class="sxs-lookup"><span data-stu-id="766e2-220">Select **Save and continue**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="766e2-221">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="766e2-221">Next steps</span></span>

- [<span data-ttu-id="766e2-222">Verificar ou atualizar as informações de perfil da sua empresa</span><span class="sxs-lookup"><span data-stu-id="766e2-222">Verify or update your company profile information</span></span>](update-your-partner-profile.md)
- [<span data-ttu-id="766e2-223">Contratos de Cliente da Microsoft (por região e idioma)</span><span class="sxs-lookup"><span data-stu-id="766e2-223">Microsoft Customer Agreements (by region, language)</span></span>](Agreements.md)
