---
title: Adicionar vários usuários para uma conta de cliente
ms.topic: how-to
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Para adicionar vários usuários à conta de um cliente, carregue um arquivo de dados no Partner Center usando o formato de arquivo de valor separado por vírgula (.csv).
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 268cc9cb42bc72a444da6aec99425c2b29b71cb4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150464"
---
# <a name="upload-a-csv-file-of-users-to-a-customers-account"></a><span data-ttu-id="caf98-103">Carregar um arquivo .csv de usuários na conta de um cliente</span><span class="sxs-lookup"><span data-stu-id="caf98-103">Upload a .csv file of users to a customer's account</span></span>


<span data-ttu-id="caf98-104">**Funções apropriadas**: administrador global</span><span class="sxs-lookup"><span data-stu-id="caf98-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="caf98-105">Adicione vários usuários à conta de um cliente de uma só vez carregando um arquivo de dados no formato de arquivo de valor separado por vírgula (.csv) para o Partner Center.</span><span class="sxs-lookup"><span data-stu-id="caf98-105">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> 

## <a name="create-the-file-of-customer-users-and-upload-to-customer-account"></a><span data-ttu-id="caf98-106">Criar o arquivo de usuários do cliente e carregar na conta do cliente</span><span class="sxs-lookup"><span data-stu-id="caf98-106">Create the file of customer users and upload to customer account</span></span>

1. <span data-ttu-id="caf98-107">Crie um arquivo de valores separados por vírgula (.csv) com os dados descritos acima.</span><span class="sxs-lookup"><span data-stu-id="caf98-107">Create a comma-separated value (.csv) data file with the data described above.</span></span> <span data-ttu-id="caf98-108">Salve o arquivo para que você possa usá-lo em uma etapa posterior.</span><span class="sxs-lookup"><span data-stu-id="caf98-108">Save the file so you can browse to it in a later step.</span></span> <span data-ttu-id="caf98-109">Consulte [Campos para o arquivo .csv para importar vários usuários para uma conta de cliente](file-customer-users.md).</span><span class="sxs-lookup"><span data-stu-id="caf98-109">See [Fields for .csv file to import multiple users for a customer account](file-customer-users.md).</span></span> 

2. <span data-ttu-id="caf98-110">Entre no [painel](https://partner.microsoft.com/dashboard) do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="caf98-110">Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).</span></span>

3. <span data-ttu-id="caf98-111">No menu do centro de parceiros, **selecione** clientes e, em seguida, escolha um cliente na lista.</span><span class="sxs-lookup"><span data-stu-id="caf98-111">From the Partner Center menu, select **Customers**, then choose a customer from the list.</span></span>

4. <span data-ttu-id="caf98-112">Selecione a guia Usuários **e Licenças do** cliente e, em seguida, **selecione Carregar usuários**.</span><span class="sxs-lookup"><span data-stu-id="caf98-112">Select the customer's **Users and Licenses** tab, then select **Upload users**.</span></span>

5. <span data-ttu-id="caf98-113">Em **Carregar informações do usuário**, selecione **Procurar**.</span><span class="sxs-lookup"><span data-stu-id="caf98-113">Under **Upload user info**, select **Browse**.</span></span>

6. <span data-ttu-id="caf98-114">No seletor de arquivo, selecione seu arquivo de dados e, em seguida, selecione **Abrir**.</span><span class="sxs-lookup"><span data-stu-id="caf98-114">In the file selector, select your data file and then select **Open**.</span></span>

7. <span data-ttu-id="caf98-115">Selecione **Validar**.</span><span class="sxs-lookup"><span data-stu-id="caf98-115">Select **Validate**.</span></span>

    <span data-ttu-id="caf98-116">**Observação**  A maioria dos erros de criação de conta é causada por problemas no arquivo de dados, como falta de informações, endereços de email incorretos ou duplicados ou número excessivo de registros no arquivo.</span><span class="sxs-lookup"><span data-stu-id="caf98-116">**Note**  Most account creation errors are caused by data file issues, including missing information, malformed or duplicated email addresses, or too many records in the file.</span></span>

8. <span data-ttu-id="caf98-117">Depois que Partner Center validar o arquivo, selecione a **Localização geográfica** para os novos usuários.</span><span class="sxs-lookup"><span data-stu-id="caf98-117">After the Partner Center validates the file, select the geographic **Location** for the new users.</span></span>
9. <span data-ttu-id="caf98-118">Selecione **Salvar**.</span><span class="sxs-lookup"><span data-stu-id="caf98-118">Select **Save**.</span></span>
10. <span data-ttu-id="caf98-119">Baixe as informações de senha temporária para os usuários.</span><span class="sxs-lookup"><span data-stu-id="caf98-119">Download the temporary password information for the users.</span></span>

    >[!IMPORTANT]
    > <span data-ttu-id="caf98-120">Certifique-se de baixar o arquivo com as senhas temporárias agora, pois você não poderá fazer isso mais tarde.</span><span class="sxs-lookup"><span data-stu-id="caf98-120">Be sure to download the file with the temporary passwords now as you won't be able to do this later.</span></span> <span data-ttu-id="caf98-121">Os novos usuários devem fazer logon em suas novas contas usando a respectiva senha temporária.</span><span class="sxs-lookup"><span data-stu-id="caf98-121">New users must log in to their new account using the temporary password for their new accounts.</span></span>

11. <span data-ttu-id="caf98-122">Novos usuários são atribuídos automaticamente a permissões de **Pode usar licenças e serviços**.</span><span class="sxs-lookup"><span data-stu-id="caf98-122">New users are automatically assigned permissions of **Can use licenses and services**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="caf98-123">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="caf98-123">Next steps</span></span>

- [<span data-ttu-id="caf98-124">Dar aos clientes permissão Partner Center para comprar seus próprios produtos ou serviços</span><span class="sxs-lookup"><span data-stu-id="caf98-124">Give customers permission in Partner Center to buy their own products or services</span></span>](give-customers-permission.md)
