---
title: Adicionar vários usuários para uma conta de cliente
ms.topic: article
ms.date: 06/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como adicionar vários usuários à conta de um cliente de uma só vez. Carregue um arquivo de dados no Partner Center usando o formato de arquivo. csv (valores separados por vírgulas).
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a9a94ac9d9022b33c7f909a258b66daa4312ad13
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2020
ms.locfileid: "86436305"
---
# <a name="add-multiple-users-to-a-customer-account---upload-a-data-file-to-partner-center"></a><span data-ttu-id="353c6-104">Adicionar vários usuários a uma conta de cliente – carregar um arquivo de dados no Partner Center</span><span class="sxs-lookup"><span data-stu-id="353c6-104">Add multiple users to a customer account - upload a data file to Partner Center</span></span>

<span data-ttu-id="353c6-105">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="353c6-105">**Applies to**</span></span>

- <span data-ttu-id="353c6-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="353c6-106">Partner Center</span></span>

<span data-ttu-id="353c6-107">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="353c6-107">**Appropriate roles**</span></span>

- <span data-ttu-id="353c6-108">Administrador global</span><span class="sxs-lookup"><span data-stu-id="353c6-108">Global admin</span></span>

<span data-ttu-id="353c6-109">Você pode adicionar vários usuários à conta de um cliente de uma só vez, carregando um arquivo de dados no formato de arquivo de valores separados por vírgula (. csv) no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="353c6-109">You can add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="353c6-110">Você pode baixar um arquivo de dados de exemplo do centro de parceiros e, em seguida, editá-lo para seu uso ou pode criar um novo arquivo de dados usando o modelo de dados definido abaixo.</span><span class="sxs-lookup"><span data-stu-id="353c6-110">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="353c6-111">Requisitos de arquivo de dados:</span><span class="sxs-lookup"><span data-stu-id="353c6-111">Data file requirements</span></span>

<span data-ttu-id="353c6-112">Para adicionar vários usuários à conta de um cliente usando o processo de carregamento em massa, você precisará atender aos seguintes requisitos:</span><span class="sxs-lookup"><span data-stu-id="353c6-112">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="353c6-113">Você deve ter permissões de administrador global para a conta de cliente;</span><span class="sxs-lookup"><span data-stu-id="353c6-113">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="353c6-114">Cada usuário deve ter um endereço de email exclusivo, adicionado ao(s) domínio(s) de email do cliente;</span><span class="sxs-lookup"><span data-stu-id="353c6-114">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="353c6-115">Você pode carregar até 100 registros por vez.</span><span class="sxs-lookup"><span data-stu-id="353c6-115">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="353c6-116">Se você precisar adicionar mais de 100 usuários, crie e carregue arquivos de dados adicionais.</span><span class="sxs-lookup"><span data-stu-id="353c6-116">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="353c6-117">Todos os usuários devem estar na mesma **localização** geográfica.</span><span class="sxs-lookup"><span data-stu-id="353c6-117">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="353c6-118">Insira apenas os dados descritos abaixo.</span><span class="sxs-lookup"><span data-stu-id="353c6-118">Enter only the data described below.</span></span> <span data-ttu-id="353c6-119">Dados irrelevantes causarão a falha do upload.</span><span class="sxs-lookup"><span data-stu-id="353c6-119">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="353c6-120">Insira os seguintes dados no arquivo de dados:</span><span class="sxs-lookup"><span data-stu-id="353c6-120">Enter the following data in the data file:</span></span>

| <span data-ttu-id="353c6-121">**Nome da coluna**</span><span class="sxs-lookup"><span data-stu-id="353c6-121">**Column name**</span></span> | <span data-ttu-id="353c6-122">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="353c6-122">**Description**</span></span>  | <span data-ttu-id="353c6-123">**Limitação**</span><span class="sxs-lookup"><span data-stu-id="353c6-123">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="353c6-124">Nome</span><span class="sxs-lookup"><span data-stu-id="353c6-124">First name</span></span>  | <span data-ttu-id="353c6-125">Nome do usuário (campo opcional)</span><span class="sxs-lookup"><span data-stu-id="353c6-125">User's first name (optional field)</span></span>  | <span data-ttu-id="353c6-126">limite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="353c6-126">50-character limit</span></span>  |
| <span data-ttu-id="353c6-127">Sobrenome</span><span class="sxs-lookup"><span data-stu-id="353c6-127">Last name</span></span>  | <span data-ttu-id="353c6-128">Sobrenome do usuário (campo opcional)</span><span class="sxs-lookup"><span data-stu-id="353c6-128">User's last name (optional field)</span></span>  | <span data-ttu-id="353c6-129">limite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="353c6-129">50-character limit</span></span>  |
| <span data-ttu-id="353c6-130">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="353c6-130">Display name</span></span>    | <span data-ttu-id="353c6-131">Nome exibido no Partner Center (campo obrigatório)</span><span class="sxs-lookup"><span data-stu-id="353c6-131">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="353c6-132">limite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="353c6-132">50-character limit</span></span>                         |
| <span data-ttu-id="353c6-133">Email</span><span class="sxs-lookup"><span data-stu-id="353c6-133">Email</span></span>   | <span data-ttu-id="353c6-134">Endereço de email comercial do usuário na empresa do cliente (campo obrigatório)</span><span class="sxs-lookup"><span data-stu-id="353c6-134">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="353c6-135">Cada usuário deve ter um endereço de e-mail exclusivo</span><span class="sxs-lookup"><span data-stu-id="353c6-135">Each user must have a unique email address</span></span> |
| <span data-ttu-id="353c6-136">Atualização de status</span><span class="sxs-lookup"><span data-stu-id="353c6-136">Status update</span></span>   | <span data-ttu-id="353c6-137">Usado para indicar se o novo registro de usuário foi ou não criado com êxito</span><span class="sxs-lookup"><span data-stu-id="353c6-137">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="353c6-138">\*\*Deixar vazio\*\*</span><span class="sxs-lookup"><span data-stu-id="353c6-138">\*\*Leave empty\*\*</span></span>                        |

### <a name="to-create-multiple-user-accounts"></a><a href="" id="createmultipleuseraccounts"></a><span data-ttu-id="353c6-139">Para criar várias contas de usuário</span><span class="sxs-lookup"><span data-stu-id="353c6-139">To create multiple user accounts</span></span>

<a href="" id="creatingtheaccounts"></a>

1. <span data-ttu-id="353c6-140">Crie um arquivo de valores separados por vírgula (.csv) com os dados descritos acima.</span><span class="sxs-lookup"><span data-stu-id="353c6-140">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="353c6-141">Salve o arquivo para que você possa usá-lo em uma etapa posterior.</span><span class="sxs-lookup"><span data-stu-id="353c6-141">Save the file so you can browse to it in a later step.</span></span>

2. <span data-ttu-id="353c6-142">Entre no [painel](https://partner.microsoft.com/dashboard) do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="353c6-142">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="353c6-143">No menu do centro de parceiros, **selecione**clientes e, em seguida, escolha um cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="353c6-143">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="353c6-144">Selecione a guia **usuários e licenças** do cliente e, em seguida, selecione **carregar usuários**.</span><span class="sxs-lookup"><span data-stu-id="353c6-144">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="353c6-145">Em **Carregar informações do usuário**, selecione **Procurar**.</span><span class="sxs-lookup"><span data-stu-id="353c6-145">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="353c6-146">No seletor de arquivo, selecione seu arquivo de dados e, em seguida, selecione **Abrir**.</span><span class="sxs-lookup"><span data-stu-id="353c6-146">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="353c6-147">Selecione **Validar**.</span><span class="sxs-lookup"><span data-stu-id="353c6-147">Select **Validate**.</span></span>

    <span data-ttu-id="353c6-148">**Observação**    A maioria dos erros de criação de conta é causada por problemas de arquivo de dados, incluindo informações ausentes, endereços de email malformados ou duplicados ou muitos registros no arquivo.</span><span class="sxs-lookup"><span data-stu-id="353c6-148">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="353c6-149">Depois que o Partner Center validar o arquivo, selecione o **local** geográfico para os novos usuários.</span><span class="sxs-lookup"><span data-stu-id="353c6-149">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="353c6-150">Clique em **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="353c6-150">Select **Save**.</span></span>
10. <span data-ttu-id="353c6-151">Baixe as informações de senha temporária para os usuários.</span><span class="sxs-lookup"><span data-stu-id="353c6-151">Download the temporary password information for the users.</span></span>

<span data-ttu-id="353c6-152">**IMPORTANTE:** Certifique-se de baixar o arquivo com as senhas temporárias agora, pois não será possível fazer isso mais tarde.</span><span class="sxs-lookup"><span data-stu-id="353c6-152">**IMPORTANT:** Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="353c6-153">Os novos usuários devem fazer logon em suas novas contas usando a respectiva senha temporária.</span><span class="sxs-lookup"><span data-stu-id="353c6-153">New users must log in to their new account using the temporary password for their new accounts.</span></span>

10. <span data-ttu-id="353c6-154">Os novos usuários recebem automaticamente permissões de **Pode usar licenças e serviços**.</span><span class="sxs-lookup"><span data-stu-id="353c6-154">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

 

 



