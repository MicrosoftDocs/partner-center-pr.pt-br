---
title: Criar vários usuários para uma conta de cliente | Partner Center
description: Você pode adicionar vários usuários a uma conta do cliente de uma vez, carregando um arquivo de dados em formato de arquivo de valores separados por vírgula (.csv) no Partner Center.
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: MaggiePucciEvans
keywords: upload em massa, adicionar vários usuários a uma conta do cliente, adicionar usuários do cliente, upload em massa de usuários do cliente, conta do cliente, usuários do cliente, usuários
ms.localizationpriority: medium
ms.openlocfilehash: 123c2c7b80398a860aa894449052502d41409c85
ms.sourcegitcommit: 123a7f53d633c27eb5f982926d856de47afb1042
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/09/2018
ms.locfileid: "4488812"
---
# <a name="add-multiple-users-to-a-customer-account"></a><span data-ttu-id="f95e4-104">Adicionar vários usuários a uma conta do cliente</span><span class="sxs-lookup"><span data-stu-id="f95e4-104">Add multiple users to a customer account</span></span>

**<span data-ttu-id="f95e4-105">Aplicável a</span><span class="sxs-lookup"><span data-stu-id="f95e4-105">Applies to</span></span>**

-  <span data-ttu-id="f95e4-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="f95e4-106">Partner Center</span></span>

<span data-ttu-id="f95e4-107">Você pode adicionar vários usuários a uma conta do cliente uma vez, carregando um arquivo de dados no formato de arquivo de valores separados por vírgula (. csv) no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="f95e4-107">You can add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="f95e4-108">Você pode baixar um arquivo de dados de exemplo do Partner Center e editá-lo para seu uso, ou você pode criar um novo arquivo de dados usando o modelo de dados definido abaixo.</span><span class="sxs-lookup"><span data-stu-id="f95e4-108">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="f95e4-109">Requisitos de arquivo de dados:</span><span class="sxs-lookup"><span data-stu-id="f95e4-109">Data file requirements</span></span>


<span data-ttu-id="f95e4-110">Para adicionar vários usuários a uma conta de cliente usando o processo de upload em massa, você precisará atender aos seguintes requisitos:</span><span class="sxs-lookup"><span data-stu-id="f95e4-110">To add multiple users to a customer’s account using the bulk upload process, you’ll need to meet the following requirements:</span></span>

-   <span data-ttu-id="f95e4-111">Você deve ter permissões de administrador global para a conta de cliente;</span><span class="sxs-lookup"><span data-stu-id="f95e4-111">You must have global administrator permissions to the customer account;</span></span>
-   <span data-ttu-id="f95e4-112">Cada usuário deve ter um endereço de email exclusivo, adicionado ao(s) domínio(s) de email do cliente;</span><span class="sxs-lookup"><span data-stu-id="f95e4-112">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
-   <span data-ttu-id="f95e4-113">Você pode carregar até 100 registros por vez.</span><span class="sxs-lookup"><span data-stu-id="f95e4-113">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="f95e4-114">Se você precisar adicionar mais de 100 usuários, crie e carregue arquivos de dados adicionais.</span><span class="sxs-lookup"><span data-stu-id="f95e4-114">If you need to add more than 100 users, create and upload additional data files.</span></span>
-   <span data-ttu-id="f95e4-115">Todos os usuários devem estar na mesma **localização** geográfica.</span><span class="sxs-lookup"><span data-stu-id="f95e4-115">All users must be in the same geographic **Location**.</span></span>
-   <span data-ttu-id="f95e4-116">Insira apenas os dados descritos abaixo.</span><span class="sxs-lookup"><span data-stu-id="f95e4-116">Enter only the data described below.</span></span> <span data-ttu-id="f95e4-117">Dados irrelevantes causarão a falha do upload.</span><span class="sxs-lookup"><span data-stu-id="f95e4-117">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="f95e4-118">Insira os seguintes dados no arquivo de dados:</span><span class="sxs-lookup"><span data-stu-id="f95e4-118">Enter the following data in the data file:</span></span>

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| **<span data-ttu-id="f95e4-119">Nome da coluna</span><span class="sxs-lookup"><span data-stu-id="f95e4-119">Column name</span></span>** | **<span data-ttu-id="f95e4-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="f95e4-120">Description</span></span>**                                                              | **<span data-ttu-id="f95e4-121">Limitação</span><span class="sxs-lookup"><span data-stu-id="f95e4-121">Limitation</span></span>**                             |
| <span data-ttu-id="f95e4-122">Nome</span><span class="sxs-lookup"><span data-stu-id="f95e4-122">First name</span></span>      | <span data-ttu-id="f95e4-123">Nome do usuário (campo opcional)</span><span class="sxs-lookup"><span data-stu-id="f95e4-123">User’s first name (optional field)</span></span>                                           | <span data-ttu-id="f95e4-124">Limite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="f95e4-124">50-character limit</span></span>                         |
| <span data-ttu-id="f95e4-125">Sobrenome</span><span class="sxs-lookup"><span data-stu-id="f95e4-125">Last name</span></span>       | <span data-ttu-id="f95e4-126">Sobrenome do usuário (campo opcional)</span><span class="sxs-lookup"><span data-stu-id="f95e4-126">User's last name (optional field)</span></span>                                            | <span data-ttu-id="f95e4-127">Limite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="f95e4-127">50-character limit</span></span>                         |
| <span data-ttu-id="f95e4-128">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="f95e4-128">Display name</span></span>    | <span data-ttu-id="f95e4-129">Nome exibido no Partner Center (campo obrigatório)</span><span class="sxs-lookup"><span data-stu-id="f95e4-129">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="f95e4-130">Limite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="f95e4-130">50-character limit</span></span>                         |
| <span data-ttu-id="f95e4-131">Email</span><span class="sxs-lookup"><span data-stu-id="f95e4-131">Email</span></span>           | <span data-ttu-id="f95e4-132">Endereço de email comercial do usuário na empresa do cliente (campo obrigatório)</span><span class="sxs-lookup"><span data-stu-id="f95e4-132">User’s business email address at customer company (required field)</span></span>           | <span data-ttu-id="f95e4-133">Cada usuário deve ter um endereço de email exclusivo</span><span class="sxs-lookup"><span data-stu-id="f95e4-133">Each user must have a unique email address</span></span> |
| <span data-ttu-id="f95e4-134">Atualização de status</span><span class="sxs-lookup"><span data-stu-id="f95e4-134">Status update</span></span>   | <span data-ttu-id="f95e4-135">Usado para indicar se o novo registro de usuário foi ou não criado com êxito</span><span class="sxs-lookup"><span data-stu-id="f95e4-135">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="f95e4-136">\*\*Deixar em branco\* \ \*</span><span class="sxs-lookup"><span data-stu-id="f95e4-136">\*\*Leave empty\*\*</span></span>                        |

 

### <a href="" id="createmultipleuseraccounts"></a><span data-ttu-id="f95e4-137">Para criar várias contas de usuário</span><span class="sxs-lookup"><span data-stu-id="f95e4-137">To create multiple user accounts</span></span>

<a href="" id="creatingtheaccounts"></a>
1.  <span data-ttu-id="f95e4-138">Crie um arquivo de valores separados por vírgula (.csv) com os dados descritos acima.</span><span class="sxs-lookup"><span data-stu-id="f95e4-138">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="f95e4-139">Salve o arquivo para que você possa usá-lo em uma etapa posterior.</span><span class="sxs-lookup"><span data-stu-id="f95e4-139">Save the file so you can browse to it in a later step.</span></span>
2.  <span data-ttu-id="f95e4-140">No menu **Partner Center** , selecione **clientes**e, em seguida, escolha um cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="f95e4-140">From the **Partner Center** menu, select **Customers**, then choose a customer from the list.</span></span>
3.  <span data-ttu-id="f95e4-141">Selecione **Carregar usuários**.</span><span class="sxs-lookup"><span data-stu-id="f95e4-141">Select **Upload users**.</span></span>
4.  <span data-ttu-id="f95e4-142">Em **Carregar informações do usuário**, selecione **Procurar**.</span><span class="sxs-lookup"><span data-stu-id="f95e4-142">Under **Upload user info**, select **Browse**.</span></span>
5.  <span data-ttu-id="f95e4-143">No seletor de arquivo, selecione seu arquivo de dados e, em seguida, selecione **Abrir**.</span><span class="sxs-lookup"><span data-stu-id="f95e4-143">In the file selector, select your data file and then select **Open**.</span></span>
6.  <span data-ttu-id="f95e4-144">Selecione **Validar**.</span><span class="sxs-lookup"><span data-stu-id="f95e4-144">Select **Validate**.</span></span>

    <span data-ttu-id="f95e4-145">**Observação**  A maioria dos erros de criação de conta é causada por problemas no arquivo de dados, como falta de informações, endereços de email incorretos ou duplicados ou número excessivo de registros no arquivo.</span><span class="sxs-lookup"><span data-stu-id="f95e4-145">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

7.  <span data-ttu-id="f95e4-146">Depois que o Partner Center validar o arquivo, selecione a **localização** geográfica dos novos usuários.</span><span class="sxs-lookup"><span data-stu-id="f95e4-146">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
8.  <span data-ttu-id="f95e4-147">Selecione **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="f95e4-147">Select **Save**.</span></span>
9.  <span data-ttu-id="f95e4-148">Baixe as informações de senha temporária dos usuários.</span><span class="sxs-lookup"><span data-stu-id="f95e4-148">Download the temporary password information for the users.</span></span>

<span data-ttu-id="f95e4-149">**IMPORTANTE:** Certifique-se de baixar o arquivo com as senhas temporárias agora, pois não será possível fazer isso mais tarde.</span><span class="sxs-lookup"><span data-stu-id="f95e4-149">**IMPORTANT:** Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="f95e4-150">Os novos usuários devem fazer logon em suas novas contas usando a respectiva senha temporária.</span><span class="sxs-lookup"><span data-stu-id="f95e4-150">New users must log in to their new account using the temporary password for their new accounts.</span></span>

10. <span data-ttu-id="f95e4-151">Novos usuários recebem automaticamente permissões de **pode usar licenças e serviços** .</span><span class="sxs-lookup"><span data-stu-id="f95e4-151">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

 

 



