---
title: Criar vários usuários para uma conta de cliente | Partner Center
ms.topic: article
ms.date: 11/13/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como adicionar vários usuários à conta de um cliente de uma só vez, carregando um arquivo de dados no formato de arquivo de valores separados por vírgula (. csv) para o centro de parceiros.
ms.assetid: c6fca2c0-2e6c-41b1-9be8-b363b139f15b
author: MaggiePucciEvans
ms.author: evansma
keywords: upload em massa, adicionar vários usuários a uma conta do cliente, adicionar usuários do cliente, upload em massa de usuários do cliente, conta do cliente, usuários do cliente, usuários
ms.localizationpriority: medium
ms.openlocfilehash: 5c9de7ed78a0494790b447d1755d5eef70a89cca
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253176"
---
# <a name="add-multiple-users-to-a-customer-account"></a><span data-ttu-id="3bbc3-104">Adicionar vários usuários a uma conta do cliente</span><span class="sxs-lookup"><span data-stu-id="3bbc3-104">Add multiple users to a customer account</span></span>

<span data-ttu-id="3bbc3-105">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="3bbc3-105">**Applies to**</span></span>

-  <span data-ttu-id="3bbc3-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="3bbc3-106">Partner Center</span></span>

<span data-ttu-id="3bbc3-107">Você pode adicionar vários usuários à conta de um cliente de uma só vez, carregando um arquivo de dados no formato de arquivo de valores separados por vírgula (. csv) no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="3bbc3-107">You can add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="3bbc3-108">Você pode baixar um arquivo de dados de exemplo do centro de parceiros e, em seguida, editá-lo para seu uso ou pode criar um novo arquivo de dados usando o modelo de dados definido abaixo.</span><span class="sxs-lookup"><span data-stu-id="3bbc3-108">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="3bbc3-109">Requisitos de arquivo de dados</span><span class="sxs-lookup"><span data-stu-id="3bbc3-109">Data file requirements</span></span>


<span data-ttu-id="3bbc3-110">Para adicionar vários usuários à conta de um cliente usando o processo de carregamento em massa, você precisará atender aos seguintes requisitos:</span><span class="sxs-lookup"><span data-stu-id="3bbc3-110">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

-   <span data-ttu-id="3bbc3-111">Você deve ter permissões de administrador global para a conta de cliente;</span><span class="sxs-lookup"><span data-stu-id="3bbc3-111">You must have global administrator permissions to the customer account;</span></span>
-   <span data-ttu-id="3bbc3-112">Cada usuário deve ter um endereço de email exclusivo, adicionado ao(s) domínio(s) de email do cliente;</span><span class="sxs-lookup"><span data-stu-id="3bbc3-112">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
-   <span data-ttu-id="3bbc3-113">Você pode carregar até 100 registros por vez.</span><span class="sxs-lookup"><span data-stu-id="3bbc3-113">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="3bbc3-114">Se você precisar adicionar mais de 100 usuários, crie e carregue arquivos de dados adicionais.</span><span class="sxs-lookup"><span data-stu-id="3bbc3-114">If you need to add more than 100 users, create and upload additional data files.</span></span>
-   <span data-ttu-id="3bbc3-115">Todos os usuários devem estar na mesma **localização** geográfica.</span><span class="sxs-lookup"><span data-stu-id="3bbc3-115">All users must be in the same geographic **Location**.</span></span>
-   <span data-ttu-id="3bbc3-116">Insira apenas os dados descritos abaixo.</span><span class="sxs-lookup"><span data-stu-id="3bbc3-116">Enter only the data described below.</span></span> <span data-ttu-id="3bbc3-117">Dados irrelevantes causarão a falha do upload.</span><span class="sxs-lookup"><span data-stu-id="3bbc3-117">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="3bbc3-118">Insira os seguintes dados no arquivo de dados:</span><span class="sxs-lookup"><span data-stu-id="3bbc3-118">Enter the following data in the data file:</span></span>

|                 |                                                                              |                                            |
|-----------------|------------------------------------------------------------------------------|--------------------------------------------|
| <span data-ttu-id="3bbc3-119">**Nome da coluna**</span><span class="sxs-lookup"><span data-stu-id="3bbc3-119">**Column name**</span></span> | <span data-ttu-id="3bbc3-120">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="3bbc3-120">**Description**</span></span>                                                              | <span data-ttu-id="3bbc3-121">**Limitação**</span><span class="sxs-lookup"><span data-stu-id="3bbc3-121">**Limitation**</span></span>                             |
| <span data-ttu-id="3bbc3-122">Nome</span><span class="sxs-lookup"><span data-stu-id="3bbc3-122">First name</span></span>      | <span data-ttu-id="3bbc3-123">Nome do usuário (campo opcional)</span><span class="sxs-lookup"><span data-stu-id="3bbc3-123">User's first name (optional field)</span></span>                                           | <span data-ttu-id="3bbc3-124">Limite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="3bbc3-124">50-character limit</span></span>                         |
| <span data-ttu-id="3bbc3-125">Sobrenome</span><span class="sxs-lookup"><span data-stu-id="3bbc3-125">Last name</span></span>       | <span data-ttu-id="3bbc3-126">Sobrenome do usuário (campo opcional)</span><span class="sxs-lookup"><span data-stu-id="3bbc3-126">User's last name (optional field)</span></span>                                            | <span data-ttu-id="3bbc3-127">Limite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="3bbc3-127">50-character limit</span></span>                         |
| <span data-ttu-id="3bbc3-128">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="3bbc3-128">Display name</span></span>    | <span data-ttu-id="3bbc3-129">Nome exibido no Partner Center (campo obrigatório)</span><span class="sxs-lookup"><span data-stu-id="3bbc3-129">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="3bbc3-130">Limite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="3bbc3-130">50-character limit</span></span>                         |
| <span data-ttu-id="3bbc3-131">Email</span><span class="sxs-lookup"><span data-stu-id="3bbc3-131">Email</span></span>           | <span data-ttu-id="3bbc3-132">Endereço de email comercial do usuário na empresa do cliente (campo obrigatório)</span><span class="sxs-lookup"><span data-stu-id="3bbc3-132">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="3bbc3-133">Cada usuário deve ter um endereço de email exclusivo</span><span class="sxs-lookup"><span data-stu-id="3bbc3-133">Each user must have a unique email address</span></span> |
| <span data-ttu-id="3bbc3-134">Atualização de status</span><span class="sxs-lookup"><span data-stu-id="3bbc3-134">Status update</span></span>   | <span data-ttu-id="3bbc3-135">Usado para indicar se o novo registro de usuário foi ou não criado com êxito</span><span class="sxs-lookup"><span data-stu-id="3bbc3-135">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="3bbc3-136">\*\*deixar vazio\*\*</span><span class="sxs-lookup"><span data-stu-id="3bbc3-136">\*\*Leave empty\*\*</span></span>                        |

 

### <a href="" id="createmultipleuseraccounts"></a><span data-ttu-id="3bbc3-137">Para criar várias contas de usuário</span><span class="sxs-lookup"><span data-stu-id="3bbc3-137">To create multiple user accounts</span></span>

<a href="" id="creatingtheaccounts"></a>
1.  <span data-ttu-id="3bbc3-138">Crie um arquivo de valores separados por vírgula (.csv) com os dados descritos acima.</span><span class="sxs-lookup"><span data-stu-id="3bbc3-138">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="3bbc3-139">Salve o arquivo para que você possa usá-lo em uma etapa posterior.</span><span class="sxs-lookup"><span data-stu-id="3bbc3-139">Save the file so you can browse to it in a later step.</span></span>
2.  <span data-ttu-id="3bbc3-140">No menu do **centro de parceiros** , selecione **clientes**e, em seguida, escolha um cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="3bbc3-140">From the **Partner Center** menu, select **Customers**, then choose a customer from the list.</span></span>
3.  <span data-ttu-id="3bbc3-141">Selecione **Carregar usuários**.</span><span class="sxs-lookup"><span data-stu-id="3bbc3-141">Select **Upload users**.</span></span>
4.  <span data-ttu-id="3bbc3-142">Em **Carregar informações do usuário**, selecione **Procurar**.</span><span class="sxs-lookup"><span data-stu-id="3bbc3-142">Under **Upload user info**, select **Browse**.</span></span>
5.  <span data-ttu-id="3bbc3-143">No seletor de arquivo, selecione seu arquivo de dados e, em seguida, selecione **Abrir**.</span><span class="sxs-lookup"><span data-stu-id="3bbc3-143">In the file selector, select your data file and then select **Open**.</span></span>
6.  <span data-ttu-id="3bbc3-144">Selecione **Validar**.</span><span class="sxs-lookup"><span data-stu-id="3bbc3-144">Select **Validate**.</span></span>

    <span data-ttu-id="3bbc3-145">**Observe**  a maioria dos erros de criação de conta são causadas por problemas de arquivo de dados, incluindo informações ausentes, endereços de email malformados ou duplicados ou muitos registros no arquivo.</span><span class="sxs-lookup"><span data-stu-id="3bbc3-145">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

7.  <span data-ttu-id="3bbc3-146">Depois que o Partner Center validar o arquivo, selecione o **local** geográfico para os novos usuários.</span><span class="sxs-lookup"><span data-stu-id="3bbc3-146">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
8.  <span data-ttu-id="3bbc3-147">Selecione **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="3bbc3-147">Select **Save**.</span></span>
9.  <span data-ttu-id="3bbc3-148">Baixe as informações de senha temporária dos usuários.</span><span class="sxs-lookup"><span data-stu-id="3bbc3-148">Download the temporary password information for the users.</span></span>

<span data-ttu-id="3bbc3-149">**IMPORTANTE:** Certifique-se de baixar o arquivo com as senhas temporárias agora, pois não será possível fazer isso mais tarde.</span><span class="sxs-lookup"><span data-stu-id="3bbc3-149">**IMPORTANT:** Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="3bbc3-150">Os novos usuários devem fazer logon em suas novas contas usando a respectiva senha temporária.</span><span class="sxs-lookup"><span data-stu-id="3bbc3-150">New users must log in to their new account using the temporary password for their new accounts.</span></span>

10. <span data-ttu-id="3bbc3-151">Os novos usuários recebem automaticamente permissões de **Pode usar licenças e serviços**.</span><span class="sxs-lookup"><span data-stu-id="3bbc3-151">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

 

 



