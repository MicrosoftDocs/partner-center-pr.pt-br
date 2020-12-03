---
title: Personalizar a experiência de uso inicial do dispositivo
ms.topic: how-to
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Antes de entregar um novo dispositivo do cliente, você pode usar os perfis do Windows AutoPilot para personalizar ou pré-configurar a OOBE (configuração inicial do usuário) do dispositivo.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: 12057d50e4456dd2450ff497e00c89a9afa5dc4d
ms.sourcegitcommit: 2d9aab15ddc20cb3d9537e68ace33d36f7d8a250
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/02/2020
ms.locfileid: "96534975"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a><span data-ttu-id="5e7d0-103">Usar perfis do Windows Autopilot em novos dispositivos para personalizar a experiência imediata do cliente</span><span class="sxs-lookup"><span data-stu-id="5e7d0-103">Use Windows Autopilot profiles on new devices to customize a customer's out-of-box experience</span></span>

<span data-ttu-id="5e7d0-104">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="5e7d0-104">**Appropriate roles**</span></span>

- <span data-ttu-id="5e7d0-105">Agente administrativo</span><span class="sxs-lookup"><span data-stu-id="5e7d0-105">Admin agent</span></span>
- <span data-ttu-id="5e7d0-106">Administrador global</span><span class="sxs-lookup"><span data-stu-id="5e7d0-106">Global admin</span></span>
- <span data-ttu-id="5e7d0-107">Agente de vendas</span><span class="sxs-lookup"><span data-stu-id="5e7d0-107">Sales agent</span></span>
- <span data-ttu-id="5e7d0-108">Administrador de gerenciamento de usuário</span><span class="sxs-lookup"><span data-stu-id="5e7d0-108">User management admin</span></span>

<span data-ttu-id="5e7d0-109">Se você gerenciar dispositivos de clientes, talvez seja necessário personalizar a OOBE (experiência inicial do usuário) para os usuários do cliente.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-109">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="5e7d0-110">Você pode pré-configurar novos dispositivos com os perfis do Windows AutoPilot antes de entregar os dispositivos aos clientes e aplicar novos perfis a dispositivos que os clientes já adquiriram.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-110">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> 

<span data-ttu-id="5e7d0-111">Observe que os OEMs começaram a incluir um rótulo de remessa no fora da caixa de dispositivo do piloto automático que mostra a **ID de chave do produto (PKID)** do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-111">Note that OEMs have started including a shipping label on the outside of the Autopilot device box that shows the device's **Product Key ID (PKID)**.</span></span>  <span data-ttu-id="5e7d0-112">Este código de barras legível e unidimensional fornece aos parceiros downstream uma maneira de registrar dispositivos para o AutoPilot sem precisar unboxr os dispositivos e coletar a ID do dispositivo por meios alternativos.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-112">This 1-dimensional, readable barcode provides downstream partners with a way to register devices for Autopilot without having to unbox the device(s) and harvest the device ID by alternative means.</span></span>

<span data-ttu-id="5e7d0-113">Este artigo explica como criar e aplicar perfis do AutoPilot a dispositivos no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-113">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="5e7d0-114">Se você ainda não estiver familiarizado com o piloto automático, revise as informações nestes artigos:</span><span class="sxs-lookup"><span data-stu-id="5e7d0-114">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="5e7d0-115">Visão geral do Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-115">Overview of Windows Autopilot</span></span>](/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="5e7d0-116">Guia de referência de implantação do AutoPilot</span><span class="sxs-lookup"><span data-stu-id="5e7d0-116">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="5e7d0-117">Visão geral</span><span class="sxs-lookup"><span data-stu-id="5e7d0-117">Overview</span></span>

<span data-ttu-id="5e7d0-118">Com o recurso de piloto automático do Windows no Partner Center, você pode criar perfis personalizados para aplicar aos dispositivos do cliente.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-118">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="5e7d0-119">As seguintes configurações de perfil estavam disponíveis no momento em que este artigo foi publicado:</span><span class="sxs-lookup"><span data-stu-id="5e7d0-119">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="5e7d0-120">Ignore as configurações de privacidade.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-120">Skip privacy settings.</span></span> <span data-ttu-id="5e7d0-121">Essa configuração opcional do perfil de piloto automático permite que as organizações não perguntem sobre as configurações de privacidade durante o processo OOBE.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-121">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="5e7d0-122">Desabilite a criação da conta de administrador local no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-122">Disable local admin account creation on the device.</span></span> <span data-ttu-id="5e7d0-123">As organizações podem decidir se o usuário que está configurando o dispositivo deve ter acesso de administrador quando o processo for concluído.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-123">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="5e7d0-124">Configurar automaticamente o dispositivo para trabalho ou escola.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-124">Automatically set up device for work or school.</span></span> <span data-ttu-id="5e7d0-125">Todos os dispositivos registrados com o piloto automático serão considerados dispositivos corporativos ou de estudante automaticamente, portanto, essa pergunta não será feita durante o processo OOBE.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-125">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="5e7d0-126">Ignore as páginas de configuração de registro do Cortana, do OneDrive e do OEM.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-126">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="5e7d0-127">Todos os dispositivos registrados com o AutoPilot irão ignorar automaticamente essas páginas durante o processo de OOBE (experiência inicial do uso).</span><span class="sxs-lookup"><span data-stu-id="5e7d0-127">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="5e7d0-128">Ignorar contrato de licença de usuário final (EULA).</span><span class="sxs-lookup"><span data-stu-id="5e7d0-128">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="5e7d0-129">A partir do Windows 10 versão 1709, as organizações podem decidir ignorar a página de EULA apresentada durante o processo OOBE.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-129">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="5e7d0-130">Consulte o [contrato de EULA do Windows AutoPilot](#windows-autopilot-eula-dismissal) abaixo para obter informações importantes a serem consideradas para ignorar a página de EULA durante a instalação do Windows.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-130">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="5e7d0-131">As permissões e limitações de gerenciamento de perfil e dispositivo a seguir se aplicam:</span><span class="sxs-lookup"><span data-stu-id="5e7d0-131">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="5e7d0-132">Os parceiros CSP podem continuar a gerenciar perfis do Autopilot para clientes existentes com os quais têm relacionamentos com revendedores, mesmo que os clientes tenham removido os privilégios de administração delegados do parceiro.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-132">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="5e7d0-133">Você pode gerenciar os dispositivos existentes dos clientes que você adicionou.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-133">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="5e7d0-134">Você não pode gerenciar os dispositivos que o cliente carregou na Microsoft Store for Business ou no Portal do Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-134">You can't manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="5e7d0-135">Criar e gerenciar perfis do AutoPilot no Partner Center</span><span class="sxs-lookup"><span data-stu-id="5e7d0-135">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="5e7d0-136">No Partner Center, você pode criar perfis de implantação do Windows AutoPilot e aplicá-los a dispositivos.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-136">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="5e7d0-137">Somente agentes admin podem criar e aplicar perfis.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-137">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="5e7d0-138">Criar um novo perfil do AutoPilot</span><span class="sxs-lookup"><span data-stu-id="5e7d0-138">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="5e7d0-139">Selecione **clientes** no menu do centro de parceiros e, em seguida, selecione o cliente para o qual você está criando o perfil do AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-139">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="5e7d0-140">Na página de detalhes do cliente, selecione **dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-140">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="5e7d0-141">Em **perfis do Windows AutoPilot** , selecione **Adicionar novo perfil**.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-141">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="5e7d0-142">Insira o nome e a descrição do perfil e defina as configurações do OOBE.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-142">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="5e7d0-143">Escolha:</span><span class="sxs-lookup"><span data-stu-id="5e7d0-143">Choose from:</span></span>  

   - <span data-ttu-id="5e7d0-144">Ignorar as configurações de privacidade na instalação</span><span class="sxs-lookup"><span data-stu-id="5e7d0-144">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="5e7d0-145">Desabilitar a conta de administrador local na instalação</span><span class="sxs-lookup"><span data-stu-id="5e7d0-145">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="5e7d0-146">Ignorar automaticamente as páginas na instalação</span><span class="sxs-lookup"><span data-stu-id="5e7d0-146">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="5e7d0-147">(Inclui *selecionar automaticamente a instalação para trabalho ou escola* e *ignorar as páginas de configuração de registro do Cortana, onedrive e OEM*)</span><span class="sxs-lookup"><span data-stu-id="5e7d0-147">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="5e7d0-148">Ignorar contrato de licença de usuário final (EULA)</span><span class="sxs-lookup"><span data-stu-id="5e7d0-148">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="5e7d0-149">Consulte o [contrato de EULA do Windows AutoPilot](#windows-autopilot-eula-dismissal) abaixo para obter informações importantes a serem consideradas para ignorar a página de EULA durante a instalação do Windows.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-149">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="5e7d0-150">Selecione **Enviar** quando terminado.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-150">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="5e7d0-151">Aplicar um perfil do AutoPilot aos dispositivos do cliente</span><span class="sxs-lookup"><span data-stu-id="5e7d0-151">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="5e7d0-152">As instruções a seguir pressupõem que você já adicionou os dispositivos do cliente ao Partner Center e que pode acessar sua lista de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-152">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="5e7d0-153">Se você ainda não tiver adicionado os dispositivos do cliente, siga as instruções em [Adicionar dispositivos à conta de um cliente](#add-devices-to-a-customers-account) e siga as etapas abaixo.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-153">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="5e7d0-154">Depois de criar um perfil de AutoPilot para um cliente, você pode aplicá-lo aos dispositivos do cliente.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-154">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="5e7d0-155">Selecione **clientes** no menu do centro de parceiros e, em seguida, selecione o cliente para o qual você criou o perfil do AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-155">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="5e7d0-156">Na página de detalhes do cliente, selecione **dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-156">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="5e7d0-157">Em **aplicar perfis a dispositivos** , selecione os dispositivos ou grupos de dispositivos aos quais você deseja adicionar perfis e, em seguida, selecione **aplicar perfil**.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-157">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="5e7d0-158">O perfil que você acabou de aplicar aparece na coluna **perfil** .</span><span class="sxs-lookup"><span data-stu-id="5e7d0-158">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="5e7d0-159">Siga as etapas abaixo para verificar se o perfil será aplicado com êxito ao dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-159">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="5e7d0-160">a.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-160">a.</span></span>  <span data-ttu-id="5e7d0-161">Conecte um dispositivo à rede e ligue-o.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-161">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="5e7d0-162">b.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-162">b.</span></span>  <span data-ttu-id="5e7d0-163">Verifique se aparecem as telas OOBE apropriadas (se existirem).</span><span class="sxs-lookup"><span data-stu-id="5e7d0-163">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="5e7d0-164">c.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-164">c.</span></span>  <span data-ttu-id="5e7d0-165">Quando o processo OOBE for interrompido, redefina o dispositivo para as configurações padrão de fábrica para prepará-lo para um novo usuário.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-165">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="5e7d0-166">Remover um perfil do AutoPilot do dispositivo de um cliente</span><span class="sxs-lookup"><span data-stu-id="5e7d0-166">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="5e7d0-167">Selecione **clientes** no menu do centro de parceiros e, em seguida, selecione o cliente para o qual você criou o perfil do AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-167">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="5e7d0-168">Na página de detalhes do cliente, selecione **dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-168">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="5e7d0-169">Em **aplicar perfis a dispositivos** , selecione os dispositivos dos quais você deseja remover o perfil e, em seguida, selecione **remover Perfil**.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-169">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="5e7d0-170">A remoção de um perfil de um dispositivo não exclui o perfil da sua lista.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-170">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="5e7d0-171">Se você quiser excluir um perfil, siga as instruções em [atualizar ou excluir um perfil do AutoPilot](#update-or-delete-an-autopilot-profile).</span><span class="sxs-lookup"><span data-stu-id="5e7d0-171">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="5e7d0-172">Atualizar ou excluir um perfil do AutoPilot</span><span class="sxs-lookup"><span data-stu-id="5e7d0-172">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="5e7d0-173">Se um cliente quiser alterar a experiência inicial do usuário depois que você enviou os dispositivos para eles, você poderá alterar o perfil no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-173">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="5e7d0-174">Quando o dispositivo do cliente se conecta à Internet, ele baixa a versão mais recente do perfil durante o processo OOBE.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-174">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="5e7d0-175">Além disso, sempre que um cliente restaurar um dispositivo para suas configurações padrão de fábrica, o dispositivo baixará novamente a versão mais recente do perfil durante o processo OOBE.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-175">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="5e7d0-176">Selecione **clientes** no menu do Partner Center e, em seguida, selecione o cliente que deseja alterar um perfil do AutoPilot.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-176">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="5e7d0-177">Na página de detalhes do cliente, selecione **dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-177">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="5e7d0-178">Em **perfis do Windows AutoPilot** , selecione o perfil que você precisa atualizar.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-178">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="5e7d0-179">Faça as alterações necessárias e, em seguida, selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-179">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="5e7d0-180">Para excluir esse perfil, selecione **excluir perfil** no canto superior direito da página.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-180">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="5e7d0-181">Adicionar dispositivos à conta de um cliente</span><span class="sxs-lookup"><span data-stu-id="5e7d0-181">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="5e7d0-182">Agentes de vendas e agentes de Administração podem adicionar dispositivos à conta de um cliente.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-182">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="5e7d0-183">Antes de aplicar perfis de AutoPilot personalizados a dispositivos de cliente, você deve ser capaz de acessar a lista de dispositivos do cliente.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-183">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="5e7d0-184">Se você planeja usar o nome do OEM, o número de série e a combinação de modelos, esteja atento a essas limitações:</span><span class="sxs-lookup"><span data-stu-id="5e7d0-184">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="5e7d0-185">Essa tupla funciona apenas para dispositivos mais recentes (hashes de 4K, por exemplo) e não tem suporte para hashes 128B (RS2 e dispositivos anteriores).</span><span class="sxs-lookup"><span data-stu-id="5e7d0-185">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="5e7d0-186">O registro de tupla diferencia maiúsculas de minúsculas e, portanto, os dados no arquivo devem corresponder ao modelo e nomes de fabricantes \**_exatamente_* _, conforme fornecido pelo provedor OEM (provedor de hardware).</span><span class="sxs-lookup"><span data-stu-id="5e7d0-186">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names \**_exactly_* _ as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="5e7d0-187">Siga as instruções abaixo para adicionar dispositivos à conta de um cliente no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-187">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="5e7d0-188">Selecione _ *Customers*\* no menu do Partner Center e, em seguida, selecione o cliente cujos dispositivos você deseja gerenciar.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-188">Select _ *Customers*\* from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="5e7d0-189">Na página de detalhes do cliente, selecione **dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-189">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="5e7d0-190">Em **aplicar perfis a dispositivos** , selecione **Adicionar dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-190">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="5e7d0-191">Insira um nome para a lista de dispositivos e, em seguida, selecione **procurar** para carregar a lista do cliente (no formato de arquivo. csv) para o centro de parceiros.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-191">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="5e7d0-192">Você deve ter recebido esse arquivo. csv com a compra do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-192">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="5e7d0-193">Se você não recebeu um arquivo. csv, você pode criar um por conta própria seguindo as etapas em [adicionando dispositivos ao Windows AutoPilot](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span><span class="sxs-lookup"><span data-stu-id="5e7d0-193">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="5e7d0-194">Carregue o arquivo. csv e, em seguida, selecione **salvar**.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-194">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="5e7d0-195">Se você receber uma mensagem de erro ao tentar carregar o arquivo .csv, verifique o formato do arquivo.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-195">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="5e7d0-196">Você pode usar somente o hash de hardware ou o nome do OEM, o número de série e o modelo (na ordem da coluna) ou a ID de Produto do Windows.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-196">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="5e7d0-197">Você também pode usar o arquivo. csv de exemplo fornecido no link ao lado de **Adicionar dispositivos** para criar uma lista de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-197">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

<span data-ttu-id="5e7d0-198">Seu arquivo. csv deve ser semelhante a este:</span><span class="sxs-lookup"><span data-stu-id="5e7d0-198">Your .csv file should look something like this:</span></span>

> <span data-ttu-id="5e7d0-199">**Número de série do dispositivo, ID do produto do Windows, hash de hardware, nome do fabricante, modelo do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="5e7d0-199">**Device Serial Number,Windows Product ID,Hardware Hash,Manufacturer name,Device model**</span></span>

> <span data-ttu-id="5e7d0-200">**{serialNumber},,, Microsoft Corporation, laptop Surface**</span><span class="sxs-lookup"><span data-stu-id="5e7d0-200">**{serialNumber},,,Microsoft Corporation,Surface Laptop**</span></span>

>[!NOTE]
> <span data-ttu-id="5e7d0-201">"Nome do fabricante" e "modelo do dispositivo" diferenciam maiúsculas de minúsculas.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-201">"Manufacturer name" and "Device model" are case-sensitive.</span></span>

<span data-ttu-id="5e7d0-202">Se você não souber qual valor deve ser colocado para o nome do fabricante e o modelo do dispositivo, poderá executá-lo no dispositivo para reunir os valores corretos:</span><span class="sxs-lookup"><span data-stu-id="5e7d0-202">If you don't know what value to put for Manufacturer name and Device Model, you can run this on the device to gather the correct values:</span></span>

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="5e7d0-203">Descartar EULA do Windows AutoPilot</span><span class="sxs-lookup"><span data-stu-id="5e7d0-203">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="5e7d0-204">INFORMAÇÕES IMPORTANTES</span><span class="sxs-lookup"><span data-stu-id="5e7d0-204">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="5e7d0-205">O Windows Autopilot permite configurar instalações personalizadas do Windows em dispositivos que você gerencia para seus clientes.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-205">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="5e7d0-206">Se autorizado a fazer isso pelo cliente, você poderá suprimir ou ocultar determinadas telas de configuração que normalmente são apresentadas aos usuários durante a configuração do Windows, incluindo a tela de aceitação do EULA (contrato de licença de usuário final).</span><span class="sxs-lookup"><span data-stu-id="5e7d0-206">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="5e7d0-207">Usando essa função, você concorda que suprimir ou ocultar as telas que foram projetadas para fornecer aos usuários aviso ou aceitação de termos significa que você obteve consentimento e autorização suficientes de seu cliente para ocultar os termos e que, em nome de seu cliente (seja uma organização ou um usuário individual como o caso), tenha consentimento para quaisquer avisos e aceite quaisquer termos que sejam aplicáveis ao cliente.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-207">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="5e7d0-208">Isso inclui o acordo com os termos e condições da licença ou o aviso que seria apresentado ao usuário caso você não o tenha suprimido ou ocultado usando essa ferramenta.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-208">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="5e7d0-209">Seu cliente não pode usar o software do Windows nesses dispositivos se o cliente não tiver adquirido de forma válida uma licença para o software da Microsoft ou de seus distribuidores licenciados.</span><span class="sxs-lookup"><span data-stu-id="5e7d0-209">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>