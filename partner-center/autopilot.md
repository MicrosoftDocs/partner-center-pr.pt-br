---
title: Personalizar a experiência de out-of-box do dispositivo com perfis do Windows Autopilot | Partner Center
description: Pré-configure experiência de out-of-box do dispositivo com perfis Autopilot.
ms.topic: article
ms.date: 02/06/19
author: maggiepuccievans
ms.author: evansma
keywords: piloto automático, o windows autopilot, piloto automático da microsoft, implantação zero touch, oobe, telas de logon, out-of-box
ms.localizationpriority: medium
ms.openlocfilehash: 46b8a74383585c630864079efa42b6e34412b91e
ms.sourcegitcommit: 80f3eb81f2e7605e77d19856827472f7830db419
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/22/2019
ms.locfileid: "9098823"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a><span data-ttu-id="21985-104">Personalizar a experiência de out-of-box do dispositivo com perfis do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="21985-104">Customize a device's out-of-box experience with Windows Autopilot profiles</span></span>

**<span data-ttu-id="21985-105">Aplica-se ao</span><span class="sxs-lookup"><span data-stu-id="21985-105">Applies to</span></span>**

- <span data-ttu-id="21985-106">Parceiros de cobrança direta CSP, provedores indiretos e revendedores indiretos</span><span class="sxs-lookup"><span data-stu-id="21985-106">CSP direct-bill partners, indirect providers, and indirect resellers</span></span>

<span data-ttu-id="21985-107">Se você gerencia dispositivos cliente, talvez seja necessário personalizar a experiência de out-of-box (OOBE) para usuários do cliente.</span><span class="sxs-lookup"><span data-stu-id="21985-107">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="21985-108">Você pode pré-configurar novos dispositivos com perfis do Windows Autopilot antes de entregar os dispositivos para os clientes e aplicar perfis de novos dispositivos clientes já tem comprado.</span><span class="sxs-lookup"><span data-stu-id="21985-108">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> <span data-ttu-id="21985-109">Este artigo explica como criar e aplicar perfis Autopilot para dispositivos no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="21985-109">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="21985-110">Se você já não estiver familiarizado com o Autopilot, examine as informações neste artigo:</span><span class="sxs-lookup"><span data-stu-id="21985-110">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="21985-111">Visão geral do Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="21985-111">Overview of Windows Autopilot</span></span>](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="21985-112">Guia de referência de implantação do AutoPilot</span><span class="sxs-lookup"><span data-stu-id="21985-112">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="21985-113">Visão geral</span><span class="sxs-lookup"><span data-stu-id="21985-113">Overview</span></span>

<span data-ttu-id="21985-114">Com o recurso Windows Autopilot no Partner Center, você pode criar perfis personalizados para aplicar aos dispositivos de cliente.</span><span class="sxs-lookup"><span data-stu-id="21985-114">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="21985-115">As seguintes configurações de perfil estavam disponíveis no momento em que este artigo foi publicado:</span><span class="sxs-lookup"><span data-stu-id="21985-115">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="21985-116">Ignorar configurações de privacidade.</span><span class="sxs-lookup"><span data-stu-id="21985-116">Skip privacy settings.</span></span> <span data-ttu-id="21985-117">Essa configuração de perfil do Autopilot opcional permite que as organizações não pergunte sobre configurações de privacidade durante o processo de configuração inicial pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="21985-117">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="21985-118">Desabilite a criação de conta de administrador local no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="21985-118">Disable local admin account creation on the device.</span></span> <span data-ttu-id="21985-119">As organizações podem decidir se o usuário de configuração do dispositivo deve ter acesso de administrador quando o processo for concluído.</span><span class="sxs-lookup"><span data-stu-id="21985-119">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="21985-120">Configure automaticamente o dispositivo para trabalho ou escola.</span><span class="sxs-lookup"><span data-stu-id="21985-120">Automatically set up device for work or school.</span></span> <span data-ttu-id="21985-121">Todos os dispositivos registrados com o Autopilot automaticamente serão considerados trabalho ou escola dispositivos, portanto, essa pergunta não será solicitada durante o processo de configuração inicial pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="21985-121">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="21985-122">Ignorar a Cortana, OneDrive e OEM páginas de configuração do registro.</span><span class="sxs-lookup"><span data-stu-id="21985-122">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="21985-123">Todos os dispositivos registrados com o Autopilot ignorará automaticamente essas páginas durante o processo de experiência de out-of-box (OOBE).</span><span class="sxs-lookup"><span data-stu-id="21985-123">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="21985-124">Ignorar o contrato de licença de usuário final (EULA).</span><span class="sxs-lookup"><span data-stu-id="21985-124">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="21985-125">A partir do Windows 10 versão 1709, as organizações podem optar por ignorar a página de EULA apresentada durante o processo de configuração inicial pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="21985-125">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="21985-126">Consulte o [descarte de EULA do Windows Autopilot](#windows-autopilot-eula-dismissal) abaixo para obter informações importantes a serem consideradas sobre ignorar a página do EULA durante a instalação do Windows.</span><span class="sxs-lookup"><span data-stu-id="21985-126">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="21985-127">Os seguintes permissões de gerenciamento de dispositivo e de perfil e limitações se aplicam:</span><span class="sxs-lookup"><span data-stu-id="21985-127">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="21985-128">Os parceiros CSP podem continuar a gerenciar perfis Autopilot para clientes existentes com quem eles têm relações de revendedor, mesmo que os clientes tenham removido privilégios de administração delegada do parceiro.</span><span class="sxs-lookup"><span data-stu-id="21985-128">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="21985-129">Você pode gerenciar dispositivos existentes para seus clientes que foram adicionados por você ou por outro parceiro CSP.</span><span class="sxs-lookup"><span data-stu-id="21985-129">You can manage existing devices for your customers that have been added either by you or by another CSP partner.</span></span>

- <span data-ttu-id="21985-130">Você não pode gerenciar dispositivos que seu cliente carregou a Microsoft Store para empresas ou Portal do Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="21985-130">You can’t manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="21985-131">Criar e gerenciar perfis Autopilot no Partner Center</span><span class="sxs-lookup"><span data-stu-id="21985-131">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="21985-132">No Partner Center, você pode criar perfis de implantação do Windows Autopilot e aplicá-los aos dispositivos.</span><span class="sxs-lookup"><span data-stu-id="21985-132">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="21985-133">Somente agentes de administrador podem criar e aplicar perfis.</span><span class="sxs-lookup"><span data-stu-id="21985-133">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="21985-134">Criar um novo perfil do Autopilot</span><span class="sxs-lookup"><span data-stu-id="21985-134">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="21985-135">Selecione **os clientes** no menu Partner Center e, em seguida, selecione o cliente que você estiver criando o perfil Autopilot.</span><span class="sxs-lookup"><span data-stu-id="21985-135">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="21985-136">Na página de detalhes do cliente, selecione **dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="21985-136">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="21985-137">Em **perfis do Windows Autopilot** selecione **Adicionar novo perfil**.</span><span class="sxs-lookup"><span data-stu-id="21985-137">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="21985-138">Insira o nome e a descrição do perfil e, em seguida, defina as configurações de OOBE.</span><span class="sxs-lookup"><span data-stu-id="21985-138">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="21985-139">Escolha:</span><span class="sxs-lookup"><span data-stu-id="21985-139">Choose from:</span></span>  

   - <span data-ttu-id="21985-140">Ignorar configurações de privacidade na instalação</span><span class="sxs-lookup"><span data-stu-id="21985-140">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="21985-141">Desabilitar a conta de administrador local na instalação</span><span class="sxs-lookup"><span data-stu-id="21985-141">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="21985-142">Ignorar automaticamente as páginas na instalação</span><span class="sxs-lookup"><span data-stu-id="21985-142">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="21985-143">(Inclui *Selecionar automaticamente a configuração para trabalho ou escola* e *Ignorar Cortana, OneDrive e OEM páginas de configuração de registro*)</span><span class="sxs-lookup"><span data-stu-id="21985-143">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="21985-144">Ignorar contrato de licença de usuário final (EULA)</span><span class="sxs-lookup"><span data-stu-id="21985-144">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="21985-145">Consulte o [descarte de EULA do Windows Autopilot](#windows-autopilot-eula-dismissal) abaixo para obter informações importantes a serem consideradas sobre ignorar a página do EULA durante a instalação do Windows.</span><span class="sxs-lookup"><span data-stu-id="21985-145">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="21985-146">Selecione **Enviar** quando terminado.</span><span class="sxs-lookup"><span data-stu-id="21985-146">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="21985-147">Aplicar um perfil Autopilot para dispositivos cliente</span><span class="sxs-lookup"><span data-stu-id="21985-147">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="21985-148">As instruções a seguir pressupõem que você já tiver adicionado os dispositivos do cliente para o Partner Center e que você possa acessar sua lista de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="21985-148">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="21985-149">Se você ainda não tiver adicionado dispositivos do cliente, siga as instruções em [Adicionar dispositivos para uma conta do cliente](#add-devices-to-a-customers-account) e, em seguida, siga as etapas abaixo.</span><span class="sxs-lookup"><span data-stu-id="21985-149">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="21985-150">Depois de criar um perfil Autopilot para um cliente, você pode aplicá-lo a dispositivos do cliente.</span><span class="sxs-lookup"><span data-stu-id="21985-150">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="21985-151">Selecione **os clientes** no menu Partner Center e, em seguida, selecione o cliente que você criou o perfil Autopilot para.</span><span class="sxs-lookup"><span data-stu-id="21985-151">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="21985-152">Na página de detalhes do cliente, selecione **dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="21985-152">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="21985-153">Em **aplicar perfis aos dispositivos** , selecione os dispositivos ou grupos de dispositivos que você deseja adicionar perfis a e, em seguida, selecione o **perfil de aplicar**.</span><span class="sxs-lookup"><span data-stu-id="21985-153">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="21985-154">O perfil que você acabou de aplicar aparece na coluna **perfil** .</span><span class="sxs-lookup"><span data-stu-id="21985-154">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="21985-155">Siga as etapas abaixo para verificar que o perfil será aplicado com êxito no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="21985-155">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="21985-156">a.</span><span class="sxs-lookup"><span data-stu-id="21985-156">a.</span></span>  <span data-ttu-id="21985-157">Conecte um dispositivo à rede e ativá-lo.</span><span class="sxs-lookup"><span data-stu-id="21985-157">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="21985-158">b.</span><span class="sxs-lookup"><span data-stu-id="21985-158">b.</span></span>  <span data-ttu-id="21985-159">Verifique se aparecem as telas OOBE apropriadas (se existirem).</span><span class="sxs-lookup"><span data-stu-id="21985-159">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="21985-160">c.</span><span class="sxs-lookup"><span data-stu-id="21985-160">c.</span></span>  <span data-ttu-id="21985-161">Quando o processo de OOBE parar, redefina o dispositivo para as configurações padrão de fábrica para prepará-lo para um novo usuário.</span><span class="sxs-lookup"><span data-stu-id="21985-161">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="21985-162">Remover um perfil Autopilot do dispositivo do cliente</span><span class="sxs-lookup"><span data-stu-id="21985-162">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="21985-163">Selecione **os clientes** no menu Partner Center e, em seguida, selecione o cliente que você criou o perfil Autopilot para.</span><span class="sxs-lookup"><span data-stu-id="21985-163">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="21985-164">Na página de detalhes do cliente, selecione **dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="21985-164">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="21985-165">Em **aplicar perfis aos dispositivos** selecione os dispositivos que você deseja remover o perfil e, em seguida, selecione **Remover perfil**.</span><span class="sxs-lookup"><span data-stu-id="21985-165">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="21985-166">Remover um perfil de um dispositivo não exclui o perfil de sua lista.</span><span class="sxs-lookup"><span data-stu-id="21985-166">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="21985-167">Se você deseja excluir um perfil, siga as instruções na [atualização ou excluir um perfil Autopilot](#update-or-delete-an-autopilot-profile).</span><span class="sxs-lookup"><span data-stu-id="21985-167">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="21985-168">Atualizar ou excluir um perfil Autopilot</span><span class="sxs-lookup"><span data-stu-id="21985-168">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="21985-169">Se um cliente quiser alterar a experiência de out-of-box depois que você tiver recebido os dispositivos para eles, você pode alterar o perfil no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="21985-169">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="21985-170">Quando o dispositivo do cliente se conecta à internet, ele vai baixar a versão mais recente do perfil durante o processo de configuração inicial pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="21985-170">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="21985-171">Além disso, sempre que um cliente restaura um dispositivo para as configurações padrão de fábrica, o dispositivo baixará novamente a versão mais recente do perfil durante o processo de configuração inicial pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="21985-171">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="21985-172">Selecione **os clientes** no menu Partner Center e, em seguida, selecione o cliente que deseja alterar um perfil Autopilot.</span><span class="sxs-lookup"><span data-stu-id="21985-172">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="21985-173">Na página de detalhes do cliente, selecione **dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="21985-173">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="21985-174">Em **perfis do Windows Autopilot** , selecione o perfil que você precisa atualizar.</span><span class="sxs-lookup"><span data-stu-id="21985-174">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="21985-175">Faça as alterações necessárias e, em seguida, selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="21985-175">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="21985-176">Para excluir esse perfil, selecione **Excluir perfil** no canto superior direito da página.</span><span class="sxs-lookup"><span data-stu-id="21985-176">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="21985-177">Adicionar dispositivos a uma conta do cliente</span><span class="sxs-lookup"><span data-stu-id="21985-177">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="21985-178">Agentes de vendas e agentes de administrador podem adicionar dispositivos para uma conta do cliente.</span><span class="sxs-lookup"><span data-stu-id="21985-178">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="21985-179">Antes de aplicar perfis Autopilot personalizados em dispositivos cliente, você deve ser capaz de acessar a lista de dispositivos do cliente.</span><span class="sxs-lookup"><span data-stu-id="21985-179">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="21985-180">Se você pretende usar o nome do OEM, o número de série e combinação de modelo, lembre-se dessas limitações:</span><span class="sxs-lookup"><span data-stu-id="21985-180">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="21985-181">Isso funciona tupla apenas para dispositivos mais recentes (4 hashes de k, por exemplo) e não há suporte para 128b hashes (RS2 e dispositivos anteriores).</span><span class="sxs-lookup"><span data-stu-id="21985-181">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="21985-182">O registro de tupla diferencia maiusculas de minúsculas, portanto, os dados no arquivo devem coincidir com o modelo e fabricante nomes ***exatamente*** conforme fornecido pelo provedor de OEM (fornecedor de hardware).</span><span class="sxs-lookup"><span data-stu-id="21985-182">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="21985-183">Siga as instruções para adicionar dispositivos a uma conta do cliente no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="21985-183">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="21985-184">Selecione **os clientes** no menu Partner Center e, em seguida, selecione o cliente cujos dispositivos que você deseja gerenciar.</span><span class="sxs-lookup"><span data-stu-id="21985-184">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="21985-185">Na página de detalhes do cliente, selecione **dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="21985-185">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="21985-186">Em **aplicar perfis aos dispositivos** selecione **Adicionar dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="21985-186">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="21985-187">Insira um nome para a lista de dispositivos e, em seguida, selecione **Procurar** para carregar a lista do cliente (no formato de arquivo. csv) para o Partner Center.</span><span class="sxs-lookup"><span data-stu-id="21985-187">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="21985-188">Você deve ter recebido esse arquivo. csv com sua compra de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="21985-188">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="21985-189">Se você não receber um arquivo. csv, você pode criar uma por conta própria, seguindo as etapas em [adicionando dispositivos Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span><span class="sxs-lookup"><span data-stu-id="21985-189">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="21985-190">Carregue o arquivo. csv e, em seguida, selecione **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="21985-190">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="21985-191">Se você receber uma mensagem de erro ao tentar carregar o arquivo. csv, verifique o formato do arquivo.</span><span class="sxs-lookup"><span data-stu-id="21985-191">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="21985-192">Você pode usar somente o hash de hardware ou o nome do OEM, o número de série e modelo (nessa ordem coluna) ou a ID do produto do Windows.</span><span class="sxs-lookup"><span data-stu-id="21985-192">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="21985-193">Você também pode usar o arquivo. csv de exemplo fornecido no link ao lado de **Adicionar dispositivos** para criar uma lista de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="21985-193">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="21985-194">Descarte de EULA do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="21985-194">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="21985-195">INFORMAÇÕES IMPORTANTES</span><span class="sxs-lookup"><span data-stu-id="21985-195">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="21985-196">O Windows Autopilot permite que você configure instalações personalizadas do Windows em dispositivos que você gerencia para seus clientes.</span><span class="sxs-lookup"><span data-stu-id="21985-196">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="21985-197">Se tiver autorização para fazê-lo pelo cliente, você pode suprimir ou ocultar determinadas telas de instalação que normalmente são apresentadas aos usuários ao configurar o Windows, incluindo a tela de aceitação do EULA (contrato de licença de usuário final).</span><span class="sxs-lookup"><span data-stu-id="21985-197">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="21985-198">Ao usar essa função, você concorda que suprimir ou ocultar quaisquer telas projetadas para fornecer aos usuários aviso ou aceitação dos termos significa que você obteve o consentimento suficiente e autorização de seu cliente para ocultar termos e que você, em nome de seu cliente (se uma organização ou um usuário individual como o caso pode ser), concorda com quaisquer avisos e aceitar qualquer termos que são aplicáveis ao cliente.</span><span class="sxs-lookup"><span data-stu-id="21985-198">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="21985-199">Isso inclui o acordo com os termos e condições da licença ou o aviso que seria apresentado ao usuário caso você não o tenha suprimido ou ocultado usando essa ferramenta.</span><span class="sxs-lookup"><span data-stu-id="21985-199">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="21985-200">Seu cliente não pode usar o software do Windows nesses dispositivos se o cliente não tiver adquirido de forma válida uma licença para o software da Microsoft ou de seus distribuidores licenciados.</span><span class="sxs-lookup"><span data-stu-id="21985-200">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>