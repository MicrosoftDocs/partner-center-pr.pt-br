---
title: Restabelecer privilégios de administrador para o CSP do Azure
ms.topic: how-to
ms.date: 05/27/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como ajudar os clientes a restabelecer os privilégios de administrador de um parceiro para que ele possa ajudar a gerenciar as assinaturas de CSP (Provedor de Soluções de Nuvem) do Azure de um cliente.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 196b38d30942278beb00096529f5965db7dfb96c
ms.sourcegitcommit: b55f63a029d88c73cd5190bbac2df1b5990e6e44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2021
ms.locfileid: "113510169"
---
# <a name="reinstate-admin-privileges-for-a-customers-azure-csp-subscriptions"></a><span data-ttu-id="dfb42-103">Restabelecer privilégios de administrador para assinaturas de CSP do Azure de um cliente</span><span class="sxs-lookup"><span data-stu-id="dfb42-103">Reinstate admin privileges for a customer's Azure CSP subscriptions</span></span>  

<span data-ttu-id="dfb42-104">**Funções apropriadas**: Administração global | Agente de administração</span><span class="sxs-lookup"><span data-stu-id="dfb42-104">**Appropriate roles**: Global admin | Admin agent</span></span>

<span data-ttu-id="dfb42-105">Na condição de um parceiro CSP (Provedor de Soluções na Nuvem), muitas vezes os clientes esperam que você gerencie para eles o uso que eles fazem do Azure e os sistemas deles.</span><span class="sxs-lookup"><span data-stu-id="dfb42-105">As a Cloud Solution Provider (CSP) partner, your customers often expect that you'll manage their Azure usage and their systems for them.</span></span> <span data-ttu-id="dfb42-106">Você precisa ter privilégios de administrador para fazer isso.</span><span class="sxs-lookup"><span data-stu-id="dfb42-106">You must have admin privileges to do so.</span></span> <span data-ttu-id="dfb42-107">Alguns privilégios são concedidos quando seu relacionamento de revendedor com o cliente é estabelecido.</span><span class="sxs-lookup"><span data-stu-id="dfb42-107">Some privileges are granted when your reseller relationship with the customer is established.</span></span> <span data-ttu-id="dfb42-108">Outros são concedidos a você pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="dfb42-108">Others are granted to you by your customer.</span></span>

## <a name="admin-privileges-for-azure-in-csp"></a><span data-ttu-id="dfb42-109">Privilégios de administrador para o Azure no CSP</span><span class="sxs-lookup"><span data-stu-id="dfb42-109">Admin privileges for Azure in CSP</span></span>

<span data-ttu-id="dfb42-110">Há dois níveis de privilégios de administrador para o Azure no CSP.</span><span class="sxs-lookup"><span data-stu-id="dfb42-110">There are two levels of admin privileges for Azure in CSP.</span></span>

- <span data-ttu-id="dfb42-111">**Privilégios de administrador de nível de locatário (privilégios de administrador delegado)** : os parceiros CSP obtêm esses privilégios ao estabelecerem o relacionamento de revendedor CSP com os clientes.</span><span class="sxs-lookup"><span data-stu-id="dfb42-111">**Tenant level admin privileges (Delegated admin privileges)**:  CSP partners get these privileges while establishing CSP reseller relationship with customers.</span></span> <span data-ttu-id="dfb42-112">Os privilégios de administrador delegado fornecem aos parceiros CSP acesso aos locatários dos clientes deles.</span><span class="sxs-lookup"><span data-stu-id="dfb42-112">Delegated admin privileges give CSP partners access to their customers' tenants.</span></span> <span data-ttu-id="dfb42-113">Esse acesso permite que eles desempenhem funções administrativas, como adicionar/gerenciar usuários, redefinir senhas e gerenciar licenças dos usuários.</span><span class="sxs-lookup"><span data-stu-id="dfb42-113">This access allows them to do administrative functions such as add/manage users, reset passwords and manage user licenses.</span></span>
- <span data-ttu-id="dfb42-114">**Privilégios de administrador de nível de assinatura**: os parceiros CSP obtêm esses privilégios ao criar assinaturas do CSP do Azure para os clientes deles.</span><span class="sxs-lookup"><span data-stu-id="dfb42-114">**Subscription level admin privileges**: CSP partners get these privileges while creating Azure CSP subscriptions for their customers.</span></span> <span data-ttu-id="dfb42-115">A posse desses privilégios fornece aos parceiros do CSP acesso completo a essas assinaturas, o que lhes permite provisionar e gerenciar recursos do Azure.</span><span class="sxs-lookup"><span data-stu-id="dfb42-115">Having these privileges gives CSP partners complete access to these subscriptions, which allows them to provision and manage Azure resources.</span></span>

## <a name="reinstate-csp-a-partners-admin-privileges"></a><span data-ttu-id="dfb42-116">Reaplicar ao CSP os privilégios de administrador de um parceiro</span><span class="sxs-lookup"><span data-stu-id="dfb42-116">Reinstate CSP a partner's admin privileges</span></span>

<span data-ttu-id="dfb42-117">O cliente poderá recriar a atribuição de função do CSP se você fornecer o `object ID` do grupo AdminAgents ao seu cliente.</span><span class="sxs-lookup"><span data-stu-id="dfb42-117">Your customer can re-create the CSP role assignment if you provide the `object ID` of the AdminAgents group to your customer.</span></span> <span data-ttu-id="dfb42-118">Para restabelecer os privilégios de administrador delegado, você precisa trabalhar com o cliente por meio das etapas a seguir.</span><span class="sxs-lookup"><span data-stu-id="dfb42-118">To regain delegated admin privileges, you need to work with your customer through the following steps.</span></span>

1. <span data-ttu-id="dfb42-119">Entre no painel do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="dfb42-119">Sign into the Partner Center dashboard.</span></span>

2. <span data-ttu-id="dfb42-120">No menu do Partner Center, selecione **Clientes**.</span><span class="sxs-lookup"><span data-stu-id="dfb42-120">On the Partner Center menu, select **Customers**.</span></span>

3. <span data-ttu-id="dfb42-121">Selecione o cliente com o qual você está trabalhando e **solicite um relacionamento de revendedor**.</span><span class="sxs-lookup"><span data-stu-id="dfb42-121">Select the customer you are working with and **request a reseller relationship**.</span></span> <span data-ttu-id="dfb42-122">Essa ação gera um link para o cliente que tem direitos de administrador de locatários.</span><span class="sxs-lookup"><span data-stu-id="dfb42-122">This action generates a link to the customer who has tenant admin rights.</span></span>

4. <span data-ttu-id="dfb42-123">Seu cliente precisa selecionar o link e aprovar a solicitação de relacionamento do revendedor.</span><span class="sxs-lookup"><span data-stu-id="dfb42-123">Your customer needs to select the link and approve the reseller relationship request.</span></span>

   :::image type="content" source="images/azure/revoke4.png" alt-text="Exemplo de email para criar relacionamento com o revendedor":::.

5. <span data-ttu-id="dfb42-125">Você, o parceiro, precisa se conectar ao locatário do parceiro para obter a ID de objeto do grupo AdminAgents.</span><span class="sxs-lookup"><span data-stu-id="dfb42-125">You, the partner, need to connect to partner tenant to get the Object ID of the AdminAgents group.</span></span>
  
   ```powershell
   Connect-AzAccount -Tenant "Partner tenant"
   # Get Object ID of AdminAgents group
   Get-AzADGroup -DisplayName AdminAgents
   ```

6. <span data-ttu-id="dfb42-126">O cliente precisa executar as etapas a seguir usando o PowerShell ou a CLI do Azure.</span><span class="sxs-lookup"><span data-stu-id="dfb42-126">Your customer must then do the following steps using either PowerShell or Azure CLI.</span></span> <span data-ttu-id="dfb42-127">O cliente precisa ter:</span><span class="sxs-lookup"><span data-stu-id="dfb42-127">Your customer must have:</span></span>

- <span data-ttu-id="dfb42-128">A função de **proprietário** ou **administrador de acesso do usuário**</span><span class="sxs-lookup"><span data-stu-id="dfb42-128">The role of **owner** or **user access administrator**</span></span> 
- <span data-ttu-id="dfb42-129">Permissões para criar atribuições de função no nível da assinatura</span><span class="sxs-lookup"><span data-stu-id="dfb42-129">Permissions to create role assignments at the subscription level</span></span>

   <span data-ttu-id="dfb42-130">a.</span><span class="sxs-lookup"><span data-stu-id="dfb42-130">a.</span></span> <span data-ttu-id="dfb42-131">Somente para o PowerShell, o cliente precisa atualizar o módulo `Az.Resources`.</span><span class="sxs-lookup"><span data-stu-id="dfb42-131">For PowerShell only, the customer must update the `Az.Resources` module.</span></span>
   ```powershell
   Update-Module Az.Resources
   ```

   <span data-ttu-id="dfb42-132">b.</span><span class="sxs-lookup"><span data-stu-id="dfb42-132">b.</span></span> <span data-ttu-id="dfb42-133">O cliente se conecta ao locatário em que a assinatura do CSP existe.</span><span class="sxs-lookup"><span data-stu-id="dfb42-133">The customer connects to the tenant where the CSP subscription exists.</span></span>
   ```powershell
   Connect-AzAccount -TenantID "<Customer tenant>"
   ```
   ```azurecli
   az login --tenant <Customer tenant>
   ```

   <span data-ttu-id="dfb42-134">c.</span><span class="sxs-lookup"><span data-stu-id="dfb42-134">c.</span></span> <span data-ttu-id="dfb42-135">O cliente se conecta à assinatura.</span><span class="sxs-lookup"><span data-stu-id="dfb42-135">The customer connects to the subscription.</span></span> <span data-ttu-id="dfb42-136">Isso será aplicável *somente* se o usuário tiver permissões de atribuição de função em várias assinaturas no locatário.</span><span class="sxs-lookup"><span data-stu-id="dfb42-136">This is *only* applicable if the user has role assignment permissions over multiple subscriptions in the tenant.</span></span>

   ```powershell
   Set-AzContext -SubscriptionID <"CSP Subscription ID">
   ```
   ```azurecli
   az account set --subscription <CSP Subscription ID>
   ```

   <span data-ttu-id="dfb42-137">d.</span><span class="sxs-lookup"><span data-stu-id="dfb42-137">d.</span></span> <span data-ttu-id="dfb42-138">O cliente criará a atribuição de função.</span><span class="sxs-lookup"><span data-stu-id="dfb42-138">The customer then creates the role assignment.</span></span>
    
   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID of the Admin Agents group provided by partner>" -RoleDefinitionName "Owner" -Scope "/subscriptions/'<CSP subscription ID>'"
   ```
   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>"
   ```

<span data-ttu-id="dfb42-139">Em vez de conceder permissões de proprietário no escopo da assinatura, você pode conceder no nível de recurso ou grupo de recursos.</span><span class="sxs-lookup"><span data-stu-id="dfb42-139">Instead of granting owner permissions at the subscription scope, you can grant at the resource group or resource level.</span></span> 

- <span data-ttu-id="dfb42-140">No nível do grupo de recursos</span><span class="sxs-lookup"><span data-stu-id="dfb42-140">At the resource group level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "/subscriptions/'SubscriptionID of CSP subscription'/resourceGroups/'Resource group name'"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "/subscriptions/<CSP Subscription Id>//resourceGroups/<Resource group name>"
   ```

- <span data-ttu-id="dfb42-141">No nível do recurso</span><span class="sxs-lookup"><span data-stu-id="dfb42-141">At the resource level</span></span>

   ```powershell
   New-AzRoleAssignment -ObjectID "<Object ID from step 3>" -RoleDefinitionName Owner -Scope "<Resource URI>"
   ```

   ```azurecli
   az role assignment create --role "Owner" --assignee-object-id <Object Id of the Admin Agents group provided by partner> --scope "<Resource URI>"
   ```

<span data-ttu-id="dfb42-142">Se as etapas acima não funcionarem ou se você receber erros ao tentar segui-las, experimente o procedimento "catch-all" a seguir para restabelecer os direitos de administrador para o cliente.</span><span class="sxs-lookup"><span data-stu-id="dfb42-142">If the above steps don't work or you get errors when attempting them, try the following "catch-all" procedure to reinstate admin rights for your customer.</span></span>

```powershell
Install-Module -Name Az.Resources -Force -Verbose
Import-Module -Name Az.Resources -Verbose -MinimumVersion 4.1.1
Connect-AzAccount -Tenant <customer tenant>
Set-AzContext -SubscriptionId <customer subscriptions>
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<customer subscription>" -ObjectType "ForeignGroup"
```

### <a name="troubleshooting"></a><span data-ttu-id="dfb42-143">Solução de problemas</span><span class="sxs-lookup"><span data-stu-id="dfb42-143">Troubleshooting</span></span>

<span data-ttu-id="dfb42-144">Se o cliente não conseguir concluir a etapa 6 acima, faça com que ele experimente o seguinte comando:</span><span class="sxs-lookup"><span data-stu-id="dfb42-144">If the customer is unable to complete step 6 above, have the customer try the following command:</span></span>

```powershell
New-AzRoleAssignment -ObjectId <principal ID> -RoleDefinitionName "Owner" -Scope "/subscriptions/<costumer subscription>" -ObjectType "ForeignGroup" -Debug > newRoleAssignment.log
```

<span data-ttu-id="dfb42-145">Forneça o arquivo `newRoleAssignment.log` resultante à Microsoft para análise posterior.</span><span class="sxs-lookup"><span data-stu-id="dfb42-145">Provide the resulting `newRoleAssignment.log` file to Microsoft for further analysis.</span></span>

<span data-ttu-id="dfb42-146">Se o procedimento "catch-all" falhar durante o `Import-Module`, experimente as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="dfb42-146">If the "catch-all" procedure fails during the `Import-Module`, try the following steps:</span></span>
- <span data-ttu-id="dfb42-147">Se a importação falhar porque o módulo está em uso, reinicie a sessão do PowerShell fechando e reabrindo todas as janelas.</span><span class="sxs-lookup"><span data-stu-id="dfb42-147">If the import fails because the module is in use, restart the PowerShell session by closing and reopening all windows.</span></span>
- <span data-ttu-id="dfb42-148">Verifique a versão do `Az.Resources` com `Get-Module Az.Resources -ListAvailable`.</span><span class="sxs-lookup"><span data-stu-id="dfb42-148">Check version of `Az.Resources` with `Get-Module Az.Resources -ListAvailable`.</span></span>
- <span data-ttu-id="dfb42-149">Se a versão 4.1.1 não estiver na lista disponível, você precisará usar `Update-Module Az.Resources -Force`.</span><span class="sxs-lookup"><span data-stu-id="dfb42-149">If version 4.1.1 is not within the available list, you must use `Update-Module Az.Resources -Force`.</span></span>
- <span data-ttu-id="dfb42-150">Se o erro informar que `Az.Accounts` precisa ser uma versão específica, atualize esse módulo também, substituindo `Az.Resources` por `Az.Accounts`.</span><span class="sxs-lookup"><span data-stu-id="dfb42-150">If the error states that `Az.Accounts` needs to be a specific version, update that module as well, replacing `Az.Resources` with `Az.Accounts`.</span></span> <span data-ttu-id="dfb42-151">Em seguida, você precisa reiniciar a sessão do PowerShell.</span><span class="sxs-lookup"><span data-stu-id="dfb42-151">You must then restart the PowerShell session.</span></span>


## <a name="next-steps"></a><span data-ttu-id="dfb42-152">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="dfb42-152">Next steps</span></span>

- [<span data-ttu-id="dfb42-153">Gerenciar assinaturas e recursos no âmbito do plano do Azure</span><span class="sxs-lookup"><span data-stu-id="dfb42-153">Manage subscriptions and resources under the Azure plan</span></span>](azure-plan-manage.md)
