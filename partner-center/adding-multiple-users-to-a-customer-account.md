---
title: Adicionar vários usuários para uma conta de cliente
ms.topic: how-to
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Para adicionar vários usuários à conta de um cliente, carregue um arquivo de dados no Partner Center usando o formato de arquivo. csv (valores separados por vírgulas).
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9f1d6e2a59bd892b7b79a1e3aa532242cdd0e302
ms.sourcegitcommit: 4043c791402f0acebee6ede160a135e87fe92493
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "96474182"
---
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a><span data-ttu-id="63041-103">Carregar um arquivo. csv de usuários para a conta de um cliente</span><span class="sxs-lookup"><span data-stu-id="63041-103">Upload a .csv file of users to a customer's account</span></span>


<span data-ttu-id="63041-104">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="63041-104">**Appropriate roles**</span></span>

- <span data-ttu-id="63041-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="63041-105">Global admin</span></span>

<span data-ttu-id="63041-106">Adicione vários usuários à conta de um cliente de uma só vez, carregando um arquivo de dados no formato de arquivo de valores separados por vírgula (. csv) no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="63041-106">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a><span data-ttu-id="63041-107">Criar o arquivo de usuários do cliente e carregar na conta do cliente</span><span class="sxs-lookup"><span data-stu-id="63041-107">Create the file of customer users and upload to customer account</span></span>

1. <span data-ttu-id="63041-108">Crie um arquivo de valores separados por vírgula (.csv) com os dados descritos acima.</span><span class="sxs-lookup"><span data-stu-id="63041-108">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="63041-109">Salve o arquivo para que você possa usá-lo em uma etapa posterior.</span><span class="sxs-lookup"><span data-stu-id="63041-109">Save the file so you can browse to it in a later step.</span></span> <span data-ttu-id="63041-110">Consulte [os campos do arquivo. csv para importar vários usuários para uma conta de cliente](file-customer-users.md).</span><span class="sxs-lookup"><span data-stu-id="63041-110">See [Fields for .csv file to import multiple users for a customer account](file-customer-users.md).</span></span> 

2. <span data-ttu-id="63041-111">Entre no [painel](https://partner.microsoft.com/dashboard) do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="63041-111">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="63041-112">No menu do centro de parceiros, **selecione** clientes e, em seguida, escolha um cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="63041-112">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="63041-113">Selecione a guia **usuários e licenças** do cliente e, em seguida, selecione **carregar usuários**.</span><span class="sxs-lookup"><span data-stu-id="63041-113">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="63041-114">Em **Carregar informações do usuário**, selecione **Procurar**.</span><span class="sxs-lookup"><span data-stu-id="63041-114">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="63041-115">No seletor de arquivo, selecione seu arquivo de dados e, em seguida, selecione **Abrir**.</span><span class="sxs-lookup"><span data-stu-id="63041-115">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="63041-116">Selecione **Validar**.</span><span class="sxs-lookup"><span data-stu-id="63041-116">Select **Validate**.</span></span>

    <span data-ttu-id="63041-117">**Observação**  A maioria dos erros de criação de conta é causada por problemas no arquivo de dados, como falta de informações, endereços de email incorretos ou duplicados ou número excessivo de registros no arquivo.</span><span class="sxs-lookup"><span data-stu-id="63041-117">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="63041-118">Depois que o Partner Center validar o arquivo, selecione o **local** geográfico para os novos usuários.</span><span class="sxs-lookup"><span data-stu-id="63041-118">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="63041-119">Clique em **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="63041-119">Select **Save**.</span></span>
10. <span data-ttu-id="63041-120">Baixe as informações de senha temporária para os usuários.</span><span class="sxs-lookup"><span data-stu-id="63041-120">Download the temporary password information for the users.</span></span>

    >[!IMPORTANT]
    > <span data-ttu-id="63041-121">Certifique-se de baixar o arquivo com as senhas temporárias agora, pois você não poderá fazer isso mais tarde.</span><span class="sxs-lookup"><span data-stu-id="63041-121">Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="63041-122">Os novos usuários devem fazer logon em suas novas contas usando a respectiva senha temporária.</span><span class="sxs-lookup"><span data-stu-id="63041-122">New users must log in to their new account using the temporary password for their new accounts.</span></span>

11. <span data-ttu-id="63041-123">Os novos usuários recebem automaticamente permissões de **Pode usar licenças e serviços**.</span><span class="sxs-lookup"><span data-stu-id="63041-123">New users are automatically assigned permissions of **Can use licenses and services** .</span></span> 

## <a name="next-steps"></a><span data-ttu-id="63041-124">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="63041-124">Next steps</span></span>

- [<span data-ttu-id="63041-125">Dê permissão aos clientes no Partner Center para comprar seus próprios produtos ou serviços</span><span class="sxs-lookup"><span data-stu-id="63041-125">Give customers permission in Partner Center to buy their own products or services</span></span>](give-customers-permission.md)
