---
title: Personalizar a experiência de out-of-box do dispositivo com perfis do Windows Autopilot | Partner Center
description: Pré-configure a experiência de out-of-box do dispositivo com perfis do Autopilot.
ms.topic: article
ms.date: 03/18/19
author: maggiepuccievans
ms.author: evansma
keywords: piloto automático, do windows autopilot, piloto automático da microsoft, implantação zero-touch, oobe, telas de logon, out-of-box
ms.localizationpriority: medium
ms.openlocfilehash: e940a7ccf79f6b43d3712a2f3ae2f9b150e1473e
ms.sourcegitcommit: f5dbd07185059aa5faddf1c5daa556f634ce97ee
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/19/2019
ms.locfileid: "58162216"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a><span data-ttu-id="2b4cd-104">Personalizar a experiência de out-of-box do dispositivo com perfis do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="2b4cd-104">Customize a device's out-of-box experience with Windows Autopilot profiles</span></span>

<span data-ttu-id="2b4cd-105">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="2b4cd-105">**Applies to**</span></span>

- <span data-ttu-id="2b4cd-106">Os parceiros CSP direto fatura, provedores indiretos e revendedores indiretos</span><span class="sxs-lookup"><span data-stu-id="2b4cd-106">CSP direct-bill partners, indirect providers, and indirect resellers</span></span>

<span data-ttu-id="2b4cd-107">Se você gerenciar dispositivos de cliente, você talvez precise personalizar a experiência de out-of-box (OOBE) para usuários do cliente.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-107">If you manage customer devices, you may need to customize the out-of-box experience (OOBE) for the customer's users.</span></span> <span data-ttu-id="2b4cd-108">Você pode pré-configurar novos dispositivos com perfis do Windows Autopilot antes de entregar os dispositivos para os clientes e aplicar novos perfis em dispositivos clientes já tem comprado.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-108">You can pre-configure new devices with Windows Autopilot profiles before delivering the devices to customers and apply new profiles to devices customers have already purchased.</span></span> <span data-ttu-id="2b4cd-109">Este artigo explica como criar e aplicar os perfis do Autopilot para dispositivos no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-109">This article explains how to create and apply Autopilot profiles to devices in Partner Center.</span></span>

<span data-ttu-id="2b4cd-110">Se você não ainda estiver familiarizado com o piloto automático, examine as informações nesses artigos:</span><span class="sxs-lookup"><span data-stu-id="2b4cd-110">If you're not already familiar with Autopilot, review the information in these articles:</span></span>

- [<span data-ttu-id="2b4cd-111">Visão geral do Windows Autopilot.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-111">Overview of Windows Autopilot</span></span>](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [<span data-ttu-id="2b4cd-112">Guia de referência de implantação do AutoPilot</span><span class="sxs-lookup"><span data-stu-id="2b4cd-112">Autopilot deployment reference guide</span></span>](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a><span data-ttu-id="2b4cd-113">Visão geral</span><span class="sxs-lookup"><span data-stu-id="2b4cd-113">Overview</span></span>

<span data-ttu-id="2b4cd-114">Com o recurso do Windows Autopilot no Partner Center, você pode criar perfis personalizados para se aplicam a dispositivos de cliente.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-114">With the Windows Autopilot feature in Partner Center, you can create custom profiles to apply to customer devices.</span></span> <span data-ttu-id="2b4cd-115">As seguintes configurações de perfil estavam disponíveis no momento em que este artigo foi publicado em:</span><span class="sxs-lookup"><span data-stu-id="2b4cd-115">The following profile settings were available at the time this article was published:</span></span>

- <span data-ttu-id="2b4cd-116">Ignorar configurações de privacidade.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-116">Skip privacy settings.</span></span> <span data-ttu-id="2b4cd-117">Essa configuração de perfil do Autopilot opcional permite que as organizações não pergunte sobre as configurações de privacidade durante o processo OOBE.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-117">This optional Autopilot profile setting enables organizations to not ask about privacy settings during the OOBE process.</span></span>

- <span data-ttu-id="2b4cd-118">Desabilite a criação da conta de administrador local no dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-118">Disable local admin account creation on the device.</span></span> <span data-ttu-id="2b4cd-119">As organizações podem decidir se a configuração do dispositivo de usuário deve ter acesso de administrador quando o processo for concluído.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-119">Organizations can decide whether the user setting up the device should have administrator access once the process is complete.</span></span>

- <span data-ttu-id="2b4cd-120">Configure automaticamente o dispositivo para o trabalho ou escola.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-120">Automatically set up device for work or school.</span></span> <span data-ttu-id="2b4cd-121">Todos os dispositivos registrados com o Autopilot serão automaticamente considerados trabalho ou escola de dispositivos, portanto, essa questão não será solicitado durante o processo OOBE.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-121">All devices registered with Autopilot will automatically be considered work or school devices, so this question will not be asked during the OOBE process.</span></span>

- <span data-ttu-id="2b4cd-122">Ignorar as páginas de configuração de registro de OEM, OneDrive e Cortana.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-122">Skip Cortana, OneDrive, and OEM registration setup pages.</span></span> <span data-ttu-id="2b4cd-123">Todos os dispositivos registrados com o Autopilot ignorará automaticamente essas páginas durante o processo de out-of-box experience (OOBE).</span><span class="sxs-lookup"><span data-stu-id="2b4cd-123">All devices registered with Autopilot will automatically skip these pages during the out-of-box experience (OOBE) process.</span></span>

- <span data-ttu-id="2b4cd-124">Ignore o contrato de licença de usuário final (EULA).</span><span class="sxs-lookup"><span data-stu-id="2b4cd-124">Skip End User License Agreement (EULA).</span></span> <span data-ttu-id="2b4cd-125">Começando no Windows 10 versão 1709, as organizações podem optar por ignorar a página de EULA apresentada durante o processo OOBE.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-125">Starting in Windows 10 version 1709, organizations can decide to skip the EULA page presented during the OOBE process.</span></span> <span data-ttu-id="2b4cd-126">Ver [exoneração do EULA do Windows Autopilot](#windows-autopilot-eula-dismissal) abaixo para obter informações importantes a considerar sobre como ignorar a página de EULA Windows durante a instalação.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-126">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

<span data-ttu-id="2b4cd-127">As seguintes permissões de gerenciamento de dispositivo e de perfil e limitações se aplicam:</span><span class="sxs-lookup"><span data-stu-id="2b4cd-127">The following profile and device management permissions and limitations apply:</span></span>

- <span data-ttu-id="2b4cd-128">Os parceiros CSP podem continuar a gerenciar os perfis do Autopilot para os clientes existentes com os quais eles têm relações de revendedor, mesmo se os clientes removeu os privilégios de administração delegada do parceiro.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-128">CSP partners can continue to manage Autopilot profiles for existing customers with whom they have reseller relationships, even if the customers have removed the partner's delegated administration privileges.</span></span>

- <span data-ttu-id="2b4cd-129">Você pode gerenciar os dispositivos existentes para os clientes que você adicionou.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-129">You can manage existing devices for your customers that you have added.</span></span>

- <span data-ttu-id="2b4cd-130">Você não pode gerenciar dispositivos de que seu cliente tiver carregado para a Microsoft Store for Business ou o Portal do Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-130">You can’t manage devices your customer has uploaded to Microsoft Store for Business or the Microsoft Intune Portal.</span></span>

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a><span data-ttu-id="2b4cd-131">Criar e gerenciar perfis do Autopilot no Partner Center</span><span class="sxs-lookup"><span data-stu-id="2b4cd-131">Create and manage Autopilot profiles in Partner Center</span></span>

<span data-ttu-id="2b4cd-132">No Partner Center, você pode criar perfis de implantação do Windows Autopilot e aplicá-las a dispositivos.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-132">In Partner Center, you can create Windows Autopilot deployment profiles and apply them to devices.</span></span>

>[!NOTE]
><span data-ttu-id="2b4cd-133">Somente os agentes administradores podem criar e aplicar perfis.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-133">Only admin agents can create and apply profiles.</span></span>

### <a name="create-a-new-autopilot-profile"></a><span data-ttu-id="2b4cd-134">Criar um novo perfil do Autopilot</span><span class="sxs-lookup"><span data-stu-id="2b4cd-134">Create a new Autopilot profile</span></span>

1. <span data-ttu-id="2b4cd-135">Selecione **clientes** no menu do Partner Center e em seguida, selecione o cliente você está criando o perfil do Autopilot.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-135">Select **Customers** from the Partner Center menu and then select the customer you're creating the Autopilot profile for.</span></span>

2. <span data-ttu-id="2b4cd-136">Na página de detalhes do cliente, selecione **dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-136">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="2b4cd-137">Sob **perfis do Windows Autopilot** selecionar **adicionar novo perfil**.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-137">Under **Windows Autopilot profiles** select **Add new profile**.</span></span>

4. <span data-ttu-id="2b4cd-138">Insira o nome e uma descrição do perfil e, em seguida, defina as configurações de OOBE.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-138">Enter the profile's name and description and then configure the OOBE settings.</span></span> <span data-ttu-id="2b4cd-139">Escolha entre:</span><span class="sxs-lookup"><span data-stu-id="2b4cd-139">Choose from:</span></span>  

   - <span data-ttu-id="2b4cd-140">Ignorar configurações de privacidade na instalação</span><span class="sxs-lookup"><span data-stu-id="2b4cd-140">Skip privacy settings in setup</span></span>

   - <span data-ttu-id="2b4cd-141">Desabilitar a conta de administrador local na instalação</span><span class="sxs-lookup"><span data-stu-id="2b4cd-141">Disable local admin account in setup</span></span>
  
   - <span data-ttu-id="2b4cd-142">Ignorar automaticamente as páginas na instalação</span><span class="sxs-lookup"><span data-stu-id="2b4cd-142">Automatically skip pages in setup</span></span><br>
        <span data-ttu-id="2b4cd-143">(Inclui *automaticamente Selecionar configuração de trabalho ou escola* e *páginas de configuração de registro de Skip Cortana, o OneDrive e o OEM*)</span><span class="sxs-lookup"><span data-stu-id="2b4cd-143">(Includes *Automatically select setup for work or school* and *Skip Cortana, OneDrive, and OEM registration setup pages*)</span></span>
  
   - <span data-ttu-id="2b4cd-144">Ignorar o contrato de licença de usuário final (EULA)</span><span class="sxs-lookup"><span data-stu-id="2b4cd-144">Skip end user license agreement (EULA)</span></span><br> 
       >[!IMPORTANT] 
       ><span data-ttu-id="2b4cd-145">Ver [exoneração do EULA do Windows Autopilot](#windows-autopilot-eula-dismissal) abaixo para obter informações importantes a considerar sobre como ignorar a página de EULA Windows durante a instalação.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-145">See [Windows Autopilot EULA dismissal](#windows-autopilot-eula-dismissal) below for important information to consider about skipping the EULA page during Windows setup.</span></span>

5. <span data-ttu-id="2b4cd-146">Selecione **Enviar** quando terminado.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-146">Select **Submit** when finished.</span></span>

### <a name="apply-an-autopilot-profile-to-customer-devices"></a><span data-ttu-id="2b4cd-147">Aplicar um perfil do Autopilot para dispositivos cliente</span><span class="sxs-lookup"><span data-stu-id="2b4cd-147">Apply an Autopilot profile to customer devices</span></span>

>[!NOTE]
><span data-ttu-id="2b4cd-148">As instruções abaixo pressupõem que você já adicionou os dispositivos do cliente ao Partner Center e que você pode acessar sua lista de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-148">The instructions below assume that you've already added the customer's devices to Partner Center and that you can access their device list.</span></span> <span data-ttu-id="2b4cd-149">Se você já não tiver adicionado os dispositivos do cliente, siga as instruções em [adicionar dispositivos para uma conta de cliente](#add-devices-to-a-customers-account) e, em seguida, siga as etapas abaixo.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-149">If you haven't already added the customer's devices, follow the instructions in [Add devices to a customer's account](#add-devices-to-a-customers-account) and then follow the steps below.</span></span>

<span data-ttu-id="2b4cd-150">Depois de criar um perfil do Autopilot para um cliente, você pode aplicá-lo a dispositivos do cliente.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-150">After you create an Autopilot profile for a customer, you can apply it to the customer's devices.</span></span>

1. <span data-ttu-id="2b4cd-151">Selecione **clientes** no menu do Partner Center e em seguida, selecione o cliente é criado para o perfil do Autopilot.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-151">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="2b4cd-152">Na página de detalhes do cliente, selecione **dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-152">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="2b4cd-153">Sob **aplicar perfis de dispositivos** selecione os dispositivos ou grupos de dispositivos que você deseja adicionar os perfis para e, em seguida, selecione **aplicar perfil**.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-153">Under **Apply profiles to devices** select the devices or device groups you want to add profiles to and then select **Apply profile**.</span></span> <span data-ttu-id="2b4cd-154">O perfil que você acabou de ser aplicado aparecerá na **perfil** coluna.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-154">The profile you just applied appears in the **Profile** column.</span></span>

4. <span data-ttu-id="2b4cd-155">Siga as etapas abaixo para verificar que o perfil será aplicado com êxito para o dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-155">Follow the steps below to verify that the profile will be applied successfully to the device.</span></span>

    <span data-ttu-id="2b4cd-156">a.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-156">a.</span></span>  <span data-ttu-id="2b4cd-157">Conectar um dispositivo à rede e ativá-lo.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-157">Connect a device to the network and turn it on.</span></span>

    <span data-ttu-id="2b4cd-158">b.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-158">b.</span></span>  <span data-ttu-id="2b4cd-159">Verifique se aparecem as telas OOBE apropriadas (se existirem).</span><span class="sxs-lookup"><span data-stu-id="2b4cd-159">Verify that the appropriate OOBE screens (if any) appear.</span></span>

    <span data-ttu-id="2b4cd-160">c.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-160">c.</span></span>  <span data-ttu-id="2b4cd-161">Quando o processo OOBE é interrompida, redefina o dispositivo para as configurações padrão de fábrica para prepará-lo para um novo usuário.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-161">When the OOBE process stops, reset the device to its factory default settings to prepare it for a new user.</span></span>

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a><span data-ttu-id="2b4cd-162">Remover um perfil do Autopilot de dispositivo do cliente</span><span class="sxs-lookup"><span data-stu-id="2b4cd-162">Remove an Autopilot profile from a customer's device</span></span>

1. <span data-ttu-id="2b4cd-163">Selecione **clientes** no menu do Partner Center e em seguida, selecione o cliente é criado para o perfil do Autopilot.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-163">Select **Customers** from the Partner Center menu and then select the customer you created the Autopilot profile for.</span></span>

2. <span data-ttu-id="2b4cd-164">Na página de detalhes do cliente, selecione **dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-164">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="2b4cd-165">Sob **aplicar perfis de dispositivos** selecione os dispositivos que você deseja remover o perfil do e, em seguida, selecione **remover perfil**.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-165">Under **Apply profiles to devices** select the devices you want to remove the profile from and then select **Remove profile**.</span></span>

   >[!NOTE]
   ><span data-ttu-id="2b4cd-166">A remoção de um perfil de um dispositivo não exclui o perfil da sua lista.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-166">Removing a profile from a device does not delete the profile from your list.</span></span> <span data-ttu-id="2b4cd-167">Se você quiser excluir um perfil, siga as instruções em [Update ou delete de um perfil do Autopilot](#update-or-delete-an-autopilot-profile).</span><span class="sxs-lookup"><span data-stu-id="2b4cd-167">If you want to delete a profile, follow the instructions in [Update or delete an Autopilot profile](#update-or-delete-an-autopilot-profile).</span></span>

### <a name="update-or-delete-an-autopilot-profile"></a><span data-ttu-id="2b4cd-168">Atualizar ou excluir um perfil do Autopilot</span><span class="sxs-lookup"><span data-stu-id="2b4cd-168">Update or delete an Autopilot profile</span></span>

<span data-ttu-id="2b4cd-169">Se um cliente deseja alterar a experiência de out-of-box depois que você enviou os dispositivos a eles, você pode alterar o perfil no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-169">If a customer wants to change the out-of-box experience after you've shipped the devices to them, you can change the profile in Partner Center.</span></span>

<span data-ttu-id="2b4cd-170">Quando o dispositivo do cliente se conecta à internet, ele baixará a última versão de perfil durante o processo OOBE.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-170">When the customer's device connects to the internet, it will download the latest profile version during the OOBE process.</span></span> <span data-ttu-id="2b4cd-171">Além disso, sempre que um cliente restaura um dispositivo para suas configurações padrão de fábrica, o dispositivo novamente baixará a última versão de perfil durante o processo OOBE.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-171">Also, any time a customer restores a device to its factory default settings, the device will again download the latest profile version during the OOBE process.</span></span>

1. <span data-ttu-id="2b4cd-172">Selecione **clientes** no menu do Partner Center e, em seguida, selecione o cliente que deseja alterar um perfil do Autopilot.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-172">Select **Customers** from the Partner Center menu and then select the customer who wants you to change an Autopilot profile.</span></span>

2. <span data-ttu-id="2b4cd-173">Na página de detalhes do cliente, selecione **dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-173">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="2b4cd-174">Sob **perfis do Windows Autopilot** selecione o perfil que você precisa atualizar.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-174">Under **Windows Autopilot profiles** select the profile you need to update.</span></span> <span data-ttu-id="2b4cd-175">Faça as alterações necessárias e, em seguida, selecione **enviar**.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-175">Make the required changes and then select **Submit**.</span></span>

<span data-ttu-id="2b4cd-176">Para excluir este perfil, selecione **excluir perfil** do canto superior direito da página.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-176">To delete this profile, select **Delete profile** from the upper right corner of the page.</span></span>

### <a name="add-devices-to-a-customers-account"></a><span data-ttu-id="2b4cd-177">Adicionar dispositivos para uma conta de cliente</span><span class="sxs-lookup"><span data-stu-id="2b4cd-177">Add devices to a customer's account</span></span>

>[!NOTE]
><span data-ttu-id="2b4cd-178">Agentes de vendas e agentes de administrador podem adicionar dispositivos para uma conta de cliente.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-178">Sales agents and admin agents can add devices to a customer's account.</span></span>

<span data-ttu-id="2b4cd-179">Antes de aplicar os perfis personalizados do Autopilot para dispositivos de cliente, você deve ser capaz de acessar a lista de dispositivos do cliente.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-179">Before you can apply custom Autopilot profiles to customer devices, you must be able to access the customer's device list.</span></span>

<span data-ttu-id="2b4cd-180">Se você planeja usar o nome, número de série e combinação de modelo do OEM, esteja ciente dessas limitações:</span><span class="sxs-lookup"><span data-stu-id="2b4cd-180">If you plan to use the OEM name, serial number, and model combination, be aware of these limitations:</span></span>

- <span data-ttu-id="2b4cd-181">Isso funciona de tupla somente para dispositivos mais recentes (4 hashes de k, por exemplo) e não há suporte para hashes 128b (dispositivos anteriores e RS2).</span><span class="sxs-lookup"><span data-stu-id="2b4cd-181">This tuple works only for newer devices (4k hashes, for example) and is not supported for 128b hashes (RS2 and prior devices).</span></span>

- <span data-ttu-id="2b4cd-182">O registro de tupla é diferencia maiusculas de minúsculas, portanto, os dados no arquivo devem corresponder aos nomes de modelo e fabricante ***exatamente*** conforme fornecido pelo provedor de OEM (provedor de hardware).</span><span class="sxs-lookup"><span data-stu-id="2b4cd-182">The tuple registration is case sensitive, so the data in the file must match the model and manufacturer names ***exactly*** as provided by the OEM provider (hardware provider).</span></span>

<span data-ttu-id="2b4cd-183">Siga as instruções abaixo para adicionar dispositivos de uma conta de cliente no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-183">Follow the instructions below to add devices to a customer's account in Partner Center.</span></span>

1. <span data-ttu-id="2b4cd-184">Selecione **clientes** no menu do Partner Center e, em seguida, selecione o cliente cujos dispositivos você deseja gerenciar.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-184">Select **Customers** from the Partner Center menu and then select the customer whose devices you want to manage.</span></span>

2. <span data-ttu-id="2b4cd-185">Na página de detalhes do cliente, selecione **dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-185">On the customer's detail page, select **Devices**.</span></span>

3. <span data-ttu-id="2b4cd-186">Sob **aplicar perfis de dispositivos** selecionar **adicionar dispositivos**.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-186">Under **Apply profiles to devices** select **Add devices**.</span></span>

4. <span data-ttu-id="2b4cd-187">Insira um nome para a lista de dispositivos e, em seguida, selecione **procurar** para carregar a lista do cliente (no formato de arquivo. csv) no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-187">Enter a name for the device list and then select **Browse** to upload the customer's list (in .csv file format) to Partner Center.</span></span>

    >[!NOTE]
    ><span data-ttu-id="2b4cd-188">Você deve ter recebido esse arquivo. csv com a compra de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-188">You should have received this .csv file with your device purchase.</span></span> <span data-ttu-id="2b4cd-189">Se você não recebeu um arquivo. csv, você pode criar um por conta própria, seguindo as etapas em [adição de dispositivos Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span><span class="sxs-lookup"><span data-stu-id="2b4cd-189">If you didn't receive a .csv file, you can create one yourself by following the steps in [Adding devices to Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).</span></span>  

5. <span data-ttu-id="2b4cd-190">Carregue o arquivo. csv e, em seguida, selecione **salvar**.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-190">Upload the .csv file and then select **Save**.</span></span>

<span data-ttu-id="2b4cd-191">Se você receber uma mensagem de erro ao tentar carregar o arquivo. csv, verifique o formato do arquivo.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-191">If you get an error message while trying to upload the .csv file, check the format of the file.</span></span> <span data-ttu-id="2b4cd-192">Você pode usar somente, o hash de hardware ou o nome do OEM, número de série e modelo (nessa ordem coluna) ou a ID do produto do Windows.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-192">You can use the hardware hash only, or the OEM name, serial number, and model (in that column order), or the Windows Product ID.</span></span> <span data-ttu-id="2b4cd-193">Você também pode usar o arquivo. csv de exemplo fornecido, próximo a partir do link **adicionar dispositivos** para criar uma lista de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-193">You can also use the sample .csv file provided from the link next to **Add devices** to create a device list.</span></span>

## <a name="windows-autopilot-eula-dismissal"></a><span data-ttu-id="2b4cd-194">Exoneração do EULA do Windows Autopilot</span><span class="sxs-lookup"><span data-stu-id="2b4cd-194">Windows Autopilot EULA dismissal</span></span>

### <a name="important-information"></a><span data-ttu-id="2b4cd-195">INFORMAÇÕES IMPORTANTES</span><span class="sxs-lookup"><span data-stu-id="2b4cd-195">IMPORTANT INFORMATION</span></span>

<span data-ttu-id="2b4cd-196">Windows Autopilot permite que você configure instalações personalizadas do Windows nos dispositivos gerenciados para seus clientes.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-196">Windows Autopilot allows you to configure customized installations of Windows on devices you manage for your customers.</span></span> <span data-ttu-id="2b4cd-197">Se autorizado a fazê-lo pelo cliente, você pode suprimir ou ocultar determinadas telas de configuração que normalmente são apresentadas aos usuários durante a configuração do Windows, incluindo a tela de aceitação do EULA (contrato de licença de usuário final).</span><span class="sxs-lookup"><span data-stu-id="2b4cd-197">If authorized to do so by the customer, you can suppress or hide certain set-up screens that are normally presented to users when setting up Windows, including the EULA (End User License Agreement) acceptance screen.</span></span>

<span data-ttu-id="2b4cd-198">Usando essa função, você concorda que, suprimindo ou ocultando as telas que são projetadas para fornecer aos usuários Observe ou a aceitação dos meios de termos que você obteve suficiente consentimento e autorização do cliente para ocultar os termos e que você, em nome de seu cliente (se uma organização ou um usuário individual, como o caso pode estar), concordar com quaisquer avisos e aceitar qualquer termos que são aplicáveis ao seu cliente.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-198">By using this function, you agree that suppressing or hiding any screens that are designed to provide users with notice or acceptance of terms means that you have obtained sufficient consent and authorization from your customer to hide terms, and that you, on behalf of your customer (whether an organization or an individual user as the case may be), consent to any notices and accept any terms that are applicable to your customer.</span></span> <span data-ttu-id="2b4cd-199">Isso inclui o acordo com os termos e condições da licença ou o aviso que seria apresentado ao usuário caso você não o tenha suprimido ou ocultado usando essa ferramenta.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-199">This includes agreement to the terms and conditions of the license or notice that would be presented to the user if you did not suppress or hide it using this tool.</span></span> <span data-ttu-id="2b4cd-200">Seu cliente não pode usar o software do Windows nesses dispositivos se o cliente não tiver adquirido de forma válida uma licença para o software da Microsoft ou de seus distribuidores licenciados.</span><span class="sxs-lookup"><span data-stu-id="2b4cd-200">Your customer may not use the Windows software on those devices if the customer has not validly acquired a license for the software from Microsoft or its licensed distributors.</span></span>