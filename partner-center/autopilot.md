---
title: Personalizar a experiência de uso inicial do dispositivo
ms.topic: article
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Antes de entregar um novo dispositivo do cliente, você pode usar os perfis do Windows AutoPilot para personalizar ou pré-configurar a OOBE (configuração inicial do usuário) do dispositivo.
author: BillLinzbach
ms.author: BillLi
keywords: piloto automático, piloto automático do Windows, Microsoft AutoPilot, implantação Zero Touch, OOBE, telas de logon, pronto para uso
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 85750e58efb7f79612a666f556cddff27db28d76
ms.sourcegitcommit: 9d0f5e6cfcaf191f95d153ae3a53fef1ab3d6f77
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2020
ms.locfileid: "86377660"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a><span data-ttu-id="9041d-104">Usar perfis do Windows AutoPilot em novos dispositivos para personalizar a experiência de uso inicial do cliente</span><span class="sxs-lookup"><span data-stu-id="9041d-104">Use Windows Autopilot profiles on new devices to customize a customer's out-of-box experience</span></span>

<span data-ttu-id="9041d-105">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="9041d-105">**Applies to**</span></span>

- <span data-ttu-id="9041d-106">CSP direto-parceiros de cobrança, provedores indiretos e revendedores indiretos</span><span class="sxs-lookup"><span data-stu-id="9041d-106">CSP direct-bill partners, indirect providers, and indirect resellers</span></span>

<span data-ttu-id="9041d-107">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="9041d-107">**Appropriate roles**</span></span>

- <span data-ttu-id="9041d-108">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="9041d-108">Admin agent</span></span>
- <span data-ttu-id="9041d-109">Administrador global</span><span class="sxs-lookup"><span data-stu-id="9041d-109">Global admin</span></span>
- <span data-ttu-id="9041d-110">Agente de vendas</span><span class="sxs-lookup"><span data-stu-id="9041d-110">Sales agent</span></span>
- <span data-ttu-id="9041d-111">Administrador de gerenciamento de usuário</span><span class="sxs-lookup"><span data-stu-id="9041d-111">User management admin</span></span>

<span data-ttu-id="9041d-112">Se você gerenciar dispositivos de clientes, talvez seja necessário personalizar a OOBE (experiência inicial do usuário) para os usuários do cliente.</span><span class="sxs-lookup"><span data-stu-id="9041d-112">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="9041d-113">Você pode pré-configurar novos dispositivos com os perfis do Windows AutoPilot antes de entregar os dispositivos aos clientes e aplicar novos perfis a dispositivos que os clientes já adquiriram.</span><span class="sxs-lookup"><span data-stu-id="9041d-113">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> 

<span data-ttu-id="9041d-114">Observe que os OEMs começaram a incluir um rótulo de remessa no fora da caixa de dispositivo do piloto automático que mostra a **ID de chave do produto (PKID)** do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9041d-114">Note that OEMs have started including a shipping label on the outside of the Autopilot device box that shows the device's **Product Key ID (PKID)**.</span></span>  <span data-ttu-id="9041d-115">Este código de barras legível e unidimensional fornece aos parceiros downstream uma maneira de registrar dispositivos para o AutoPilot sem precisar unboxr os dispositivos e coletar a ID do dispositivo por meios alternativos.</span><span class="sxs-lookup"><span data-stu-id="9041d-115">This 1-dimensional, readable barcode provides downstream partners with a way to register devices for Autopilot without having to unbox the device(s) and harvest the device ID by alternative means.</span></span>

<span data-ttu-id="9041d-116">Este artigo explica como criar e aplicar perfis do AutoPilot a dispositivos no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="9041d-116">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="9041d-117">Se você ainda não estiver familiarizado com o piloto automático, revise as informações nestes artigos:</span><span class="sxs-lookup"><span data-stu-id="9041d-117">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="9041d-118">Visão geral do Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="9041d-118">Overview of Windows Autopilot</span></span>](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="9041d-119">Guia de referência de implantação do AutoPilot</span><span class="sxs-lookup"><span data-stu-id="9041d-119">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="9041d-120">Visão geral</span><span class="sxs-lookup"><span data-stu-id="9041d-120">Overview</span></span>

<span data-ttu-id="9041d-121">Com o recurso de piloto automático do Windows no Partner Center, você pode criar perfis personalizados para aplicar aos dispositivos do cliente.</span><span class="sxs-lookup"><span data-stu-id="9041d-121">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="9041d-122">As seguintes configurações de perfil estavam disponíveis no momento em que este artigo foi publicado:</span><span class="sxs-lookup"><span data-stu-id="9041d-122">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="9041d-123">Ignore as configurações de privacidade.</span><span class="sxs-lookup"><span data-stu-id="9041d-123">Skip privacy settings.</span></span> <span data-ttu-id="9041d-124">Essa configuração opcional do perfil de piloto automático permite que as organizações não perguntem sobre as configurações de privacidade durante o processo OOBE.</span><span class="sxs-lookup"><span data-stu-id="9041d-124">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="9041d-125">Desabilite a criação da conta de administrador local no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9041d-125">Disable local admin account creation on the device.</span></span> <span data-ttu-id="9041d-126">As organizações podem decidir se o usuário que está configurando o dispositivo deve ter acesso de administrador quando o processo for concluído.</span><span class="sxs-lookup"><span data-stu-id="9041d-126">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="9041d-127">Configurar automaticamente o dispositivo para trabalho ou escola.</span><span class="sxs-lookup"><span data-stu-id="9041d-127">Automatically set up device for work or school.</span></span> <span data-ttu-id="9041d-128">Todos os dispositivos registrados com o piloto automático serão considerados dispositivos corporativos ou de estudante automaticamente, portanto, essa pergunta não será feita durante o processo OOBE.</span><span class="sxs-lookup"><span data-stu-id="9041d-128">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="9041d-129">Ignore as páginas de configuração de registro do Cortana, do OneDrive e do OEM.</span><span class="sxs-lookup"><span data-stu-id="9041d-129">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="9041d-130">Todos os dispositivos registrados com o AutoPilot irão ignorar automaticamente essas páginas durante o processo de OOBE (experiência inicial do uso).</span><span class="sxs-lookup"><span data-stu-id="9041d-130">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="9041d-131">Ignorar contrato de licença de usuário final (EULA).</span><span class="sxs-lookup"><span data-stu-id="9041d-131">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="9041d-132">A partir do Windows 10 versão 1709, as organizações podem decidir ignorar a página de EULA apresentada durante o processo OOBE.</span><span class="sxs-lookup"><span data-stu-id="9041d-132">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="9041d-133">Consulte o [contrato de EULA do Windows AutoPilot](#windows-autopilot-eula-dismissal) abaixo para obter informações importantes a serem consideradas para ignorar a página de EULA durante a instalação do Windows.</span><span class="sxs-lookup"><span data-stu-id="9041d-133">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="9041d-134">As seguintes permissões e limitações de gerenciamento de perfil e dispositivo se aplicam:</span><span class="sxs-lookup"><span data-stu-id="9041d-134">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="9041d-135">Os parceiros CSP podem continuar a gerenciar perfis de AutoPilot para clientes existentes com os quais têm relações de revendedores, mesmo que os clientes tenham removido os privilégios de administração delegada do parceiro.</span><span class="sxs-lookup"><span data-stu-id="9041d-135">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="9041d-136">Você pode gerenciar dispositivos existentes para seus clientes que você adicionou.</span><span class="sxs-lookup"><span data-stu-id="9041d-136">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="9041d-137">Você não pode gerenciar dispositivos que seu cliente carregou para Microsoft Store para empresas ou para o portal de Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="9041d-137">You can't manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="9041d-138">Criar e gerenciar perfis do AutoPilot no Partner Center</span><span class="sxs-lookup"><span data-stu-id="9041d-138">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="9041d-139">No Partner Center, você pode criar perfis de implantação do Windows AutoPilot e aplicá-los a dispositivos.</span><span class="sxs-lookup"><span data-stu-id="9041d-139">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="9041d-140">Somente agentes admin podem criar e aplicar perfis.</span><span class="sxs-lookup"><span data-stu-id="9041d-140">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="9041d-141">Criar um novo perfil do AutoPilot</span><span class="sxs-lookup"><span data-stu-id="9041d-141">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="9041d-142">Selecione **clientes** no menu do centro de parceiros e, em seguida, selecione o cliente para o qual você está criando o perfil do AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="9041d-142">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="9041d-143">Na página de detalhes do cliente, selecione **dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="9041d-143">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="9041d-144">Em **perfis do Windows AutoPilot** , selecione **Adicionar novo perfil**.</span><span class="sxs-lookup"><span data-stu-id="9041d-144">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="9041d-145">Insira o nome e a descrição do perfil e defina as configurações do OOBE.</span><span class="sxs-lookup"><span data-stu-id="9041d-145">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="9041d-146">Escolha:</span><span class="sxs-lookup"><span data-stu-id="9041d-146">Choose from:</span></span>  

   - <span data-ttu-id="9041d-147">Ignorar as configurações de privacidade na instalação</span><span class="sxs-lookup"><span data-stu-id="9041d-147">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="9041d-148">Desabilitar a conta de administrador local na instalação</span><span class="sxs-lookup"><span data-stu-id="9041d-148">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="9041d-149">Ignorar automaticamente as páginas na instalação</span><span class="sxs-lookup"><span data-stu-id="9041d-149">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="9041d-150">(Inclui *selecionar automaticamente a instalação para trabalho ou escola* e *ignorar as páginas de configuração de registro do Cortana, onedrive e OEM*)</span><span class="sxs-lookup"><span data-stu-id="9041d-150">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="9041d-151">Ignorar contrato de licença de usuário final (EULA)</span><span class="sxs-lookup"><span data-stu-id="9041d-151">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="9041d-152">Consulte o [contrato de EULA do Windows AutoPilot](#windows-autopilot-eula-dismissal) abaixo para obter informações importantes a serem consideradas para ignorar a página de EULA durante a instalação do Windows.</span><span class="sxs-lookup"><span data-stu-id="9041d-152">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="9041d-153">Selecione **Enviar** quando terminado.</span><span class="sxs-lookup"><span data-stu-id="9041d-153">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="9041d-154">Aplicar um perfil do AutoPilot aos dispositivos do cliente</span><span class="sxs-lookup"><span data-stu-id="9041d-154">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="9041d-155">As instruções a seguir pressupõem que você já adicionou os dispositivos do cliente ao Partner Center e que pode acessar sua lista de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="9041d-155">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="9041d-156">Se você ainda não tiver adicionado os dispositivos do cliente, siga as instruções em [Adicionar dispositivos à conta de um cliente](#add-devices-to-a-customers-account) e siga as etapas abaixo.</span><span class="sxs-lookup"><span data-stu-id="9041d-156">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="9041d-157">Depois de criar um perfil de AutoPilot para um cliente, você pode aplicá-lo aos dispositivos do cliente.</span><span class="sxs-lookup"><span data-stu-id="9041d-157">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="9041d-158">Selecione **clientes** no menu do centro de parceiros e, em seguida, selecione o cliente para o qual você criou o perfil do AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="9041d-158">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="9041d-159">Na página de detalhes do cliente, selecione **dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="9041d-159">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="9041d-160">Em **aplicar perfis a dispositivos** , selecione os dispositivos ou grupos de dispositivos aos quais você deseja adicionar perfis e, em seguida, selecione **aplicar perfil**.</span><span class="sxs-lookup"><span data-stu-id="9041d-160">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="9041d-161">O perfil que você acabou de aplicar aparece na coluna **perfil** .</span><span class="sxs-lookup"><span data-stu-id="9041d-161">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="9041d-162">Siga as etapas abaixo para verificar se o perfil será aplicado com êxito ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9041d-162">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="9041d-163">a.</span><span class="sxs-lookup"><span data-stu-id="9041d-163">a.</span></span>  <span data-ttu-id="9041d-164">Conecte um dispositivo à rede e ligue-o.</span><span class="sxs-lookup"><span data-stu-id="9041d-164">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="9041d-165">b.</span><span class="sxs-lookup"><span data-stu-id="9041d-165">b.</span></span>  <span data-ttu-id="9041d-166">Verifique se aparecem as telas OOBE apropriadas (se existirem).</span><span class="sxs-lookup"><span data-stu-id="9041d-166">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="9041d-167">c.</span><span class="sxs-lookup"><span data-stu-id="9041d-167">c.</span></span>  <span data-ttu-id="9041d-168">Quando o processo OOBE for interrompido, redefina o dispositivo para as configurações padrão de fábrica para prepará-lo para um novo usuário.</span><span class="sxs-lookup"><span data-stu-id="9041d-168">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="9041d-169">Remover um perfil do AutoPilot do dispositivo de um cliente</span><span class="sxs-lookup"><span data-stu-id="9041d-169">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="9041d-170">Selecione **clientes** no menu do centro de parceiros e, em seguida, selecione o cliente para o qual você criou o perfil do AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="9041d-170">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="9041d-171">Na página de detalhes do cliente, selecione **dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="9041d-171">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="9041d-172">Em **aplicar perfis a dispositivos** , selecione os dispositivos dos quais você deseja remover o perfil e, em seguida, selecione **remover Perfil**.</span><span class="sxs-lookup"><span data-stu-id="9041d-172">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="9041d-173">A remoção de um perfil de um dispositivo não exclui o perfil da sua lista.</span><span class="sxs-lookup"><span data-stu-id="9041d-173">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="9041d-174">Se você quiser excluir um perfil, siga as instruções em [atualizar ou excluir um perfil do AutoPilot](#update-or-delete-an-autopilot-profile).</span><span class="sxs-lookup"><span data-stu-id="9041d-174">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="9041d-175">Atualizar ou excluir um perfil do AutoPilot</span><span class="sxs-lookup"><span data-stu-id="9041d-175">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="9041d-176">Se um cliente quiser alterar a experiência inicial do usuário depois que você enviou os dispositivos para eles, você poderá alterar o perfil no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="9041d-176">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="9041d-177">Quando o dispositivo do cliente se conecta à Internet, ele baixa a versão mais recente do perfil durante o processo OOBE.</span><span class="sxs-lookup"><span data-stu-id="9041d-177">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="9041d-178">Além disso, sempre que um cliente restaurar um dispositivo para suas configurações padrão de fábrica, o dispositivo baixará novamente a versão mais recente do perfil durante o processo OOBE.</span><span class="sxs-lookup"><span data-stu-id="9041d-178">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="9041d-179">Selecione **clientes** no menu do Partner Center e, em seguida, selecione o cliente que deseja alterar um perfil do AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="9041d-179">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="9041d-180">Na página de detalhes do cliente, selecione **dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="9041d-180">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="9041d-181">Em **perfis do Windows AutoPilot** , selecione o perfil que você precisa atualizar.</span><span class="sxs-lookup"><span data-stu-id="9041d-181">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="9041d-182">Faça as alterações necessárias e, em seguida, selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="9041d-182">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="9041d-183">Para excluir esse perfil, selecione **excluir perfil** no canto superior direito da página.</span><span class="sxs-lookup"><span data-stu-id="9041d-183">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="9041d-184">Adicionar dispositivos à conta de um cliente</span><span class="sxs-lookup"><span data-stu-id="9041d-184">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="9041d-185">Agentes de vendas e agentes de Administração podem adicionar dispositivos à conta de um cliente.</span><span class="sxs-lookup"><span data-stu-id="9041d-185">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="9041d-186">Antes de aplicar perfis de AutoPilot personalizados a dispositivos de cliente, você deve ser capaz de acessar a lista de dispositivos do cliente.</span><span class="sxs-lookup"><span data-stu-id="9041d-186">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="9041d-187">Se você planeja usar o nome do OEM, o número de série e a combinação de modelos, esteja atento a essas limitações:</span><span class="sxs-lookup"><span data-stu-id="9041d-187">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="9041d-188">Essa tupla funciona apenas para dispositivos mais recentes (hashes de 4K, por exemplo) e não tem suporte para hashes 128B (RS2 e dispositivos anteriores).</span><span class="sxs-lookup"><span data-stu-id="9041d-188">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="9041d-189">O registro de tupla diferencia maiúsculas de minúsculas e, portanto, os dados no arquivo devem corresponder ao modelo e aos nomes dos fabricantes ***exatamente*** como fornecidos pelo provedor OEM (provedor de hardware).</span><span class="sxs-lookup"><span data-stu-id="9041d-189">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="9041d-190">Siga as instruções abaixo para adicionar dispositivos à conta de um cliente no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="9041d-190">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="9041d-191">Selecione **clientes** no menu do centro de parceiros e, em seguida, selecione o cliente cujos dispositivos você deseja gerenciar.</span><span class="sxs-lookup"><span data-stu-id="9041d-191">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="9041d-192">Na página de detalhes do cliente, selecione **dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="9041d-192">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="9041d-193">Em **aplicar perfis a dispositivos** , selecione **Adicionar dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="9041d-193">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="9041d-194">Insira um nome para a lista de dispositivos e, em seguida, selecione **procurar** para carregar a lista do cliente (no formato de arquivo. csv) para o centro de parceiros.</span><span class="sxs-lookup"><span data-stu-id="9041d-194">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="9041d-195">Você deve ter recebido esse arquivo. csv com a compra do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="9041d-195">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="9041d-196">Se você não recebeu um arquivo. csv, você pode criar um por conta própria seguindo as etapas em [adicionando dispositivos ao Windows AutoPilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span><span class="sxs-lookup"><span data-stu-id="9041d-196">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="9041d-197">Carregue o arquivo. csv e, em seguida, selecione **salvar**.</span><span class="sxs-lookup"><span data-stu-id="9041d-197">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="9041d-198">Se você receber uma mensagem de erro ao tentar carregar o arquivo. csv, verifique o formato do arquivo.</span><span class="sxs-lookup"><span data-stu-id="9041d-198">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="9041d-199">Você pode usar somente o hash de hardware ou o nome do OEM, o número de série e o modelo (na ordem da coluna) ou a ID do produto do Windows.</span><span class="sxs-lookup"><span data-stu-id="9041d-199">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="9041d-200">Você também pode usar o arquivo. csv de exemplo fornecido no link ao lado de **Adicionar dispositivos** para criar uma lista de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="9041d-200">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

<span data-ttu-id="9041d-201">Seu arquivo. csv deve ser semelhante a este:</span><span class="sxs-lookup"><span data-stu-id="9041d-201">Your .csv file should look something like this:</span></span>

> <span data-ttu-id="9041d-202">**Número de série do dispositivo, ID do produto do Windows, hash de hardware, nome do fabricante, modelo do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="9041d-202">**Device Serial Number,Windows Product ID,Hardware Hash,Manufacturer name,Device model**</span></span>

> <span data-ttu-id="9041d-203">**{serialNumber},,, Microsoft Corporation, laptop Surface**</span><span class="sxs-lookup"><span data-stu-id="9041d-203">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span></span>

>[!NOTE]
> <span data-ttu-id="9041d-204">"Nome do fabricante" e "modelo do dispositivo" diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="9041d-204">"Manufacturer name" and "Device model" are case-sensitive.</span></span>

<span data-ttu-id="9041d-205">Se você não souber qual valor deve ser colocado para o nome do fabricante e o modelo do dispositivo, poderá executá-lo no dispositivo para reunir os valores corretos:</span><span class="sxs-lookup"><span data-stu-id="9041d-205">If you don't know what value to put for Manufacturer name and Device Model, you can run this on the device to gather the correct values:</span></span>

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="9041d-206">Descartar EULA do Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="9041d-206">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="9041d-207">INFORMAÇÕES IMPORTANTES</span><span class="sxs-lookup"><span data-stu-id="9041d-207">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="9041d-208">O Windows Autopilot permite configurar instalações personalizadas do Windows em dispositivos que você gerencia para seus clientes.</span><span class="sxs-lookup"><span data-stu-id="9041d-208">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="9041d-209">Se autorizado a fazer isso pelo cliente, você poderá suprimir ou ocultar determinadas telas de configuração que normalmente são apresentadas aos usuários durante a configuração do Windows, incluindo a tela de aceitação do EULA (contrato de licença de usuário final).</span><span class="sxs-lookup"><span data-stu-id="9041d-209">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="9041d-210">Usando essa função, você concorda que suprimir ou ocultar as telas que foram projetadas para fornecer aos usuários aviso ou aceitação de termos significa que você obteve consentimento e autorização suficientes de seu cliente para ocultar os termos e que, em nome de seu cliente (seja uma organização ou um usuário individual como o caso), tenha consentimento para quaisquer avisos e aceite quaisquer termos que sejam aplicáveis ao cliente.</span><span class="sxs-lookup"><span data-stu-id="9041d-210">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="9041d-211">Isso inclui o acordo com os termos e condições da licença ou o aviso que seria apresentado ao usuário caso você não o tenha suprimido ou ocultado usando essa ferramenta.</span><span class="sxs-lookup"><span data-stu-id="9041d-211">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="9041d-212">Seu cliente não pode usar o software do Windows nesses dispositivos se o cliente não tiver adquirido de forma válida uma licença para o software da Microsoft ou de seus distribuidores licenciados.</span><span class="sxs-lookup"><span data-stu-id="9041d-212">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>
