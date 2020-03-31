---
title: Criar vários usuários para uma conta de cliente | Partner Center
ms.topic: article
ms.date: 11/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como adicionar vários usuários à conta de um cliente de uma só vez, carregando um arquivo de dados no formato de arquivo de valores separados por vírgula (. csv) para o centro de parceiros.
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: jasonwhowell
ms.author: jasonh
keywords: upload em massa, adicionar vários usuários a uma conta do cliente, adicionar usuários do cliente, upload em massa de usuários do cliente, conta do cliente, usuários do cliente, usuários
ms.localizationpriority: medium
ms.openlocfilehash: 499aff67d18b0d8f9fbaf098fecbab2d888d9ac7
ms.sourcegitcommit: 5dcf8cefd2c4731c6a80e57c65b43521d7c37b6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/30/2020
ms.locfileid: "80390365"
---
# <a name="add-multiple-users-to-a-customer-account"></a><span data-ttu-id="47854-104">Adicionar vários usuários a uma conta de cliente</span><span class="sxs-lookup"><span data-stu-id="47854-104">Add multiple users to a customer account</span></span>

<span data-ttu-id="47854-105">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="47854-105">**Applies to**</span></span>

- <span data-ttu-id="47854-106">Centro de Parceiros</span><span class="sxs-lookup"><span data-stu-id="47854-106">Partner Center</span></span>

<span data-ttu-id="47854-107">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="47854-107">**Appropriate roles**</span></span>

- <span data-ttu-id="47854-108">Administração global</span><span class="sxs-lookup"><span data-stu-id="47854-108">Global admin</span></span>

<span data-ttu-id="47854-109">Você pode adicionar vários usuários à conta de um cliente de uma só vez, carregando um arquivo de dados no formato de arquivo de valores separados por vírgula (. csv) no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="47854-109">You can add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="47854-110">Você pode baixar um arquivo de dados de exemplo do centro de parceiros e, em seguida, editá-lo para seu uso ou pode criar um novo arquivo de dados usando o modelo de dados definido abaixo.</span><span class="sxs-lookup"><span data-stu-id="47854-110">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="47854-111">Requisitos de arquivo de dados</span><span class="sxs-lookup"><span data-stu-id="47854-111">Data file requirements</span></span>

<span data-ttu-id="47854-112">Para adicionar vários usuários à conta de um cliente usando o processo de carregamento em massa, você precisará atender aos seguintes requisitos:</span><span class="sxs-lookup"><span data-stu-id="47854-112">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="47854-113">Você deve ter permissões de administrador global para a conta de cliente;</span><span class="sxs-lookup"><span data-stu-id="47854-113">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="47854-114">Cada usuário deve ter um endereço de email exclusivo, adicionado ao(s) domínio(s) de email do cliente;</span><span class="sxs-lookup"><span data-stu-id="47854-114">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="47854-115">Você pode carregar até 100 registros por vez.</span><span class="sxs-lookup"><span data-stu-id="47854-115">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="47854-116">Se você precisar adicionar mais de 100 usuários, crie e carregue arquivos de dados adicionais.</span><span class="sxs-lookup"><span data-stu-id="47854-116">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="47854-117">Todos os usuários devem estar na mesma **localização** geográfica.</span><span class="sxs-lookup"><span data-stu-id="47854-117">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="47854-118">Insira apenas os dados descritos abaixo.</span><span class="sxs-lookup"><span data-stu-id="47854-118">Enter only the data described below.</span></span> <span data-ttu-id="47854-119">Dados irrelevantes causarão a falha do upload.</span><span class="sxs-lookup"><span data-stu-id="47854-119">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="47854-120">Insira os seguintes dados no arquivo de dados:</span><span class="sxs-lookup"><span data-stu-id="47854-120">Enter the following data in the data file:</span></span>

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| <span data-ttu-id="47854-121">**Nome da coluna**</span><span class="sxs-lookup"><span data-stu-id="47854-121">**Column name**</span></span> | <span data-ttu-id="47854-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="47854-122">**Description**</span></span>                                                              | <span data-ttu-id="47854-123">**Limitação**</span><span class="sxs-lookup"><span data-stu-id="47854-123">**Limitation**</span></span>                             |
| <span data-ttu-id="47854-124">Nome</span><span class="sxs-lookup"><span data-stu-id="47854-124">First name</span></span>      | <span data-ttu-id="47854-125">Nome do usuário (campo opcional)</span><span class="sxs-lookup"><span data-stu-id="47854-125">User's first name (optional field)</span></span>                                           | <span data-ttu-id="47854-126">Limite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="47854-126">50-character limit</span></span>                         |
| <span data-ttu-id="47854-127">Sobrenome</span><span class="sxs-lookup"><span data-stu-id="47854-127">Last name</span></span>       | <span data-ttu-id="47854-128">Sobrenome do usuário (campo opcional)</span><span class="sxs-lookup"><span data-stu-id="47854-128">User's last name (optional field)</span></span>                                            | <span data-ttu-id="47854-129">Limite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="47854-129">50-character limit</span></span>                         |
| <span data-ttu-id="47854-130">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="47854-130">Display name</span></span>    | <span data-ttu-id="47854-131">Nome exibido no Partner Center (campo obrigatório)</span><span class="sxs-lookup"><span data-stu-id="47854-131">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="47854-132">Limite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="47854-132">50-character limit</span></span>                         |
| <span data-ttu-id="47854-133">Email</span><span class="sxs-lookup"><span data-stu-id="47854-133">Email</span></span>           | <span data-ttu-id="47854-134">Endereço de email comercial do usuário na empresa do cliente (campo obrigatório)</span><span class="sxs-lookup"><span data-stu-id="47854-134">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="47854-135">Cada usuário deve ter um endereço de email exclusivo</span><span class="sxs-lookup"><span data-stu-id="47854-135">Each user must have a unique email address</span></span> |
| <span data-ttu-id="47854-136">Atualização de status</span><span class="sxs-lookup"><span data-stu-id="47854-136">Status update</span></span>   | <span data-ttu-id="47854-137">Usado para indicar se o novo registro de usuário foi ou não criado com êxito</span><span class="sxs-lookup"><span data-stu-id="47854-137">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="47854-138">\*\*deixar vazio\*\*</span><span class="sxs-lookup"><span data-stu-id="47854-138">\*\*Leave empty\*\*</span></span>                        |

### <a name="to-create-multiple-user-accounts"></a><a href="" id="createmultipleuseraccounts"></a><span data-ttu-id="47854-139">Para criar várias contas de usuário</span><span class="sxs-lookup"><span data-stu-id="47854-139">To create multiple user accounts</span></span>

<a href="" id="creatingtheaccounts"></a>

1. <span data-ttu-id="47854-140">Crie um arquivo de valores separados por vírgula (.csv) com os dados descritos acima.</span><span class="sxs-lookup"><span data-stu-id="47854-140">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="47854-141">Salve o arquivo para que você possa usá-lo em uma etapa posterior.</span><span class="sxs-lookup"><span data-stu-id="47854-141">Save the file so you can browse to it in a later step.</span></span>

2. <span data-ttu-id="47854-142">Entre no [painel](https://partner.microsoft.com/dashboard) do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="47854-142">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="47854-143">No menu do centro de parceiros, **selecione**clientes e, em seguida, escolha um cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="47854-143">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="47854-144">Selecione a guia **usuários e licenças** do cliente e, em seguida, selecione **carregar usuários**.</span><span class="sxs-lookup"><span data-stu-id="47854-144">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="47854-145">Em **Carregar informações do usuário**, selecione **Procurar**.</span><span class="sxs-lookup"><span data-stu-id="47854-145">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="47854-146">No seletor de arquivo, selecione seu arquivo de dados e, em seguida, selecione **Abrir**.</span><span class="sxs-lookup"><span data-stu-id="47854-146">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="47854-147">Selecione **Validar**.</span><span class="sxs-lookup"><span data-stu-id="47854-147">Select **Validate**.</span></span>

    <span data-ttu-id="47854-148">**Observe**  a maioria dos erros de criação de conta são causadas por problemas de arquivo de dados, incluindo informações ausentes, endereços de email malformados ou duplicados ou muitos registros no arquivo.</span><span class="sxs-lookup"><span data-stu-id="47854-148">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="47854-149">Depois que o Partner Center validar o arquivo, selecione o **local** geográfico para os novos usuários.</span><span class="sxs-lookup"><span data-stu-id="47854-149">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="47854-150">Selecione **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="47854-150">Select **Save**.</span></span>
10. <span data-ttu-id="47854-151">Baixe as informações de senha temporária dos usuários.</span><span class="sxs-lookup"><span data-stu-id="47854-151">Download the temporary password information for the users.</span></span>

<span data-ttu-id="47854-152">**IMPORTANTE:** Certifique-se de baixar o arquivo com as senhas temporárias agora, pois não será possível fazer isso mais tarde.</span><span class="sxs-lookup"><span data-stu-id="47854-152">**IMPORTANT:** Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="47854-153">Os novos usuários devem fazer logon em suas novas contas usando a respectiva senha temporária.</span><span class="sxs-lookup"><span data-stu-id="47854-153">New users must log in to their new account using the temporary password for their new accounts.</span></span>

10. <span data-ttu-id="47854-154">Os novos usuários recebem automaticamente permissões de **Pode usar licenças e serviços**.</span><span class="sxs-lookup"><span data-stu-id="47854-154">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

 

 



