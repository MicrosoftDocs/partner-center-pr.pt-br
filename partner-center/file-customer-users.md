---
title: Campos para o arquivo .csv para importar vários usuários para uma conta de cliente
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Para adicionar vários usuários a uma conta de cliente, crie um arquivo de valor separado por vírgula (.csv) com campos apropriados.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 152daadde25a9325937797f7a3daa90dfb59a9b4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110150974"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="769b0-103">Adicionar vários usuários a uma conta de cliente criando um arquivo .csv</span><span class="sxs-lookup"><span data-stu-id="769b0-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="769b0-104">**Funções apropriadas**: administrador global</span><span class="sxs-lookup"><span data-stu-id="769b0-104">**Appropriate roles**: Global admin</span></span>

<span data-ttu-id="769b0-105">Adicione vários usuários à conta de um cliente de uma só vez carregando um arquivo de dados no formato de arquivo de valor separado por vírgula (.csv) para o Partner Center.</span><span class="sxs-lookup"><span data-stu-id="769b0-105">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="769b0-106">Você pode baixar um arquivo de dados de exemplo do Partner Center e editá-lo para seu uso ou criar um novo arquivo de dados usando o modelo de dados definido abaixo.</span><span class="sxs-lookup"><span data-stu-id="769b0-106">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="769b0-107">Requisitos de arquivo de dados:</span><span class="sxs-lookup"><span data-stu-id="769b0-107">Data file requirements</span></span>

<span data-ttu-id="769b0-108">Para adicionar vários usuários à conta de um cliente usando o processo de carregamento em massa, você precisará atender aos seguintes requisitos:</span><span class="sxs-lookup"><span data-stu-id="769b0-108">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="769b0-109">Você deve ter permissões de administrador global para a conta de cliente;</span><span class="sxs-lookup"><span data-stu-id="769b0-109">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="769b0-110">Cada usuário deve ter um endereço de email exclusivo, adicionado ao(s) domínio(s) de email do cliente;</span><span class="sxs-lookup"><span data-stu-id="769b0-110">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="769b0-111">Você pode carregar até 100 registros por vez.</span><span class="sxs-lookup"><span data-stu-id="769b0-111">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="769b0-112">Se você precisar adicionar mais de 100 usuários, crie e carregue arquivos de dados adicionais.</span><span class="sxs-lookup"><span data-stu-id="769b0-112">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="769b0-113">Todos os usuários devem estar na mesma **localização** geográfica.</span><span class="sxs-lookup"><span data-stu-id="769b0-113">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="769b0-114">Insira apenas os dados descritos abaixo.</span><span class="sxs-lookup"><span data-stu-id="769b0-114">Enter only the data described below.</span></span> <span data-ttu-id="769b0-115">Dados irrelevantes causarão a falha do upload.</span><span class="sxs-lookup"><span data-stu-id="769b0-115">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="769b0-116">Insira os seguintes dados no arquivo de dados:</span><span class="sxs-lookup"><span data-stu-id="769b0-116">Enter the following data in the data file:</span></span>

| <span data-ttu-id="769b0-117">**Nome da coluna**</span><span class="sxs-lookup"><span data-stu-id="769b0-117">**Column name**</span></span> | <span data-ttu-id="769b0-118">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="769b0-118">**Description**</span></span>  | <span data-ttu-id="769b0-119">**Limitação**</span><span class="sxs-lookup"><span data-stu-id="769b0-119">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="769b0-120">Nome</span><span class="sxs-lookup"><span data-stu-id="769b0-120">First name</span></span>  | <span data-ttu-id="769b0-121">Nome do usuário (campo opcional)</span><span class="sxs-lookup"><span data-stu-id="769b0-121">User's first name (optional field)</span></span>  | <span data-ttu-id="769b0-122">limite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="769b0-122">50-character limit</span></span>  |
| <span data-ttu-id="769b0-123">Sobrenome</span><span class="sxs-lookup"><span data-stu-id="769b0-123">Last name</span></span>  | <span data-ttu-id="769b0-124">Sobrenome do usuário (campo opcional)</span><span class="sxs-lookup"><span data-stu-id="769b0-124">User's last name (optional field)</span></span>  | <span data-ttu-id="769b0-125">limite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="769b0-125">50-character limit</span></span>  |
| <span data-ttu-id="769b0-126">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="769b0-126">Display name</span></span>    | <span data-ttu-id="769b0-127">Nome exibido na Partner Center (campo obrigatório)</span><span class="sxs-lookup"><span data-stu-id="769b0-127">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="769b0-128">limite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="769b0-128">50-character limit</span></span>                         |
| <span data-ttu-id="769b0-129">Email</span><span class="sxs-lookup"><span data-stu-id="769b0-129">Email</span></span>   | <span data-ttu-id="769b0-130">Endereço de email comercial do usuário na empresa do cliente (campo obrigatório)</span><span class="sxs-lookup"><span data-stu-id="769b0-130">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="769b0-131">Cada usuário deve ter um endereço de e-mail exclusivo</span><span class="sxs-lookup"><span data-stu-id="769b0-131">Each user must have a unique email address</span></span> |
| <span data-ttu-id="769b0-132">Atualização de status</span><span class="sxs-lookup"><span data-stu-id="769b0-132">Status update</span></span>   | <span data-ttu-id="769b0-133">Usado para indicar se o novo registro de usuário foi criado com êxito</span><span class="sxs-lookup"><span data-stu-id="769b0-133">Used to indicate whether the new user record was successfully created</span></span> | <span data-ttu-id="769b0-134">\*\*Deixe em branco\*\*</span><span class="sxs-lookup"><span data-stu-id="769b0-134">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="769b0-135">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="769b0-135">Next steps</span></span>

- [<span data-ttu-id="769b0-136">Como adicionar vários usuários para um cliente</span><span class="sxs-lookup"><span data-stu-id="769b0-136">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)