---
title: Campos para o arquivo. csv para importar vários usuários para uma conta de cliente
ms.topic: article
ms.date: 08/01/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Para adicionar vários usuários a uma conta de cliente, crie um arquivo de valores separados por vírgulas (. csv) com os campos apropriados.
author: parthpandyaMSFT
ms.author: parthp
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8ba08d97f1d360eae5af1941ed36753addd24939
ms.sourcegitcommit: 3c26a61982082787bbdaf5d1e92553b26f3a5076
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/06/2021
ms.locfileid: "106441414"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="27d55-103">Adicionar vários usuários a uma conta de cliente criando um arquivo. csv</span><span class="sxs-lookup"><span data-stu-id="27d55-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="27d55-104">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="27d55-104">**Appropriate roles**</span></span>

- <span data-ttu-id="27d55-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="27d55-105">Global admin</span></span>

<span data-ttu-id="27d55-106">Adicione vários usuários à conta de um cliente de uma só vez, carregando um arquivo de dados no formato de arquivo de valores separados por vírgula (. csv) no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="27d55-106">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="27d55-107">Você pode baixar um arquivo de dados de exemplo do centro de parceiros e, em seguida, editá-lo para seu uso ou pode criar um novo arquivo de dados usando o modelo de dados definido abaixo.</span><span class="sxs-lookup"><span data-stu-id="27d55-107">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="27d55-108">Requisitos de arquivo de dados:</span><span class="sxs-lookup"><span data-stu-id="27d55-108">Data file requirements</span></span>

<span data-ttu-id="27d55-109">Para adicionar vários usuários à conta de um cliente usando o processo de carregamento em massa, você precisará atender aos seguintes requisitos:</span><span class="sxs-lookup"><span data-stu-id="27d55-109">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="27d55-110">Você deve ter permissões de administrador global para a conta de cliente;</span><span class="sxs-lookup"><span data-stu-id="27d55-110">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="27d55-111">Cada usuário deve ter um endereço de email exclusivo, adicionado ao(s) domínio(s) de email do cliente;</span><span class="sxs-lookup"><span data-stu-id="27d55-111">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="27d55-112">Você pode carregar até 100 registros por vez.</span><span class="sxs-lookup"><span data-stu-id="27d55-112">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="27d55-113">Se você precisar adicionar mais de 100 usuários, crie e carregue arquivos de dados adicionais.</span><span class="sxs-lookup"><span data-stu-id="27d55-113">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="27d55-114">Todos os usuários devem estar na mesma **localização** geográfica.</span><span class="sxs-lookup"><span data-stu-id="27d55-114">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="27d55-115">Insira apenas os dados descritos abaixo.</span><span class="sxs-lookup"><span data-stu-id="27d55-115">Enter only the data described below.</span></span> <span data-ttu-id="27d55-116">Dados irrelevantes causarão a falha do upload.</span><span class="sxs-lookup"><span data-stu-id="27d55-116">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="27d55-117">Insira os seguintes dados no arquivo de dados:</span><span class="sxs-lookup"><span data-stu-id="27d55-117">Enter the following data in the data file:</span></span>

| <span data-ttu-id="27d55-118">**Nome da coluna**</span><span class="sxs-lookup"><span data-stu-id="27d55-118">**Column name**</span></span> | <span data-ttu-id="27d55-119">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="27d55-119">**Description**</span></span>  | <span data-ttu-id="27d55-120">**Limitação**</span><span class="sxs-lookup"><span data-stu-id="27d55-120">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="27d55-121">Nome</span><span class="sxs-lookup"><span data-stu-id="27d55-121">First name</span></span>  | <span data-ttu-id="27d55-122">Nome do usuário (campo opcional)</span><span class="sxs-lookup"><span data-stu-id="27d55-122">User's first name (optional field)</span></span>  | <span data-ttu-id="27d55-123">limite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="27d55-123">50-character limit</span></span>  |
| <span data-ttu-id="27d55-124">Sobrenome</span><span class="sxs-lookup"><span data-stu-id="27d55-124">Last name</span></span>  | <span data-ttu-id="27d55-125">Sobrenome do usuário (campo opcional)</span><span class="sxs-lookup"><span data-stu-id="27d55-125">User's last name (optional field)</span></span>  | <span data-ttu-id="27d55-126">limite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="27d55-126">50-character limit</span></span>  |
| <span data-ttu-id="27d55-127">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="27d55-127">Display name</span></span>    | <span data-ttu-id="27d55-128">Nome exibido no Partner Center (campo obrigatório)</span><span class="sxs-lookup"><span data-stu-id="27d55-128">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="27d55-129">limite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="27d55-129">50-character limit</span></span>                         |
| <span data-ttu-id="27d55-130">Email</span><span class="sxs-lookup"><span data-stu-id="27d55-130">Email</span></span>   | <span data-ttu-id="27d55-131">Endereço de email comercial do usuário na empresa do cliente (campo obrigatório)</span><span class="sxs-lookup"><span data-stu-id="27d55-131">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="27d55-132">Cada usuário deve ter um endereço de e-mail exclusivo</span><span class="sxs-lookup"><span data-stu-id="27d55-132">Each user must have a unique email address</span></span> |
| <span data-ttu-id="27d55-133">Atualização de status</span><span class="sxs-lookup"><span data-stu-id="27d55-133">Status update</span></span>   | <span data-ttu-id="27d55-134">Usado para indicar se o novo registro de usuário foi criado com êxito</span><span class="sxs-lookup"><span data-stu-id="27d55-134">Used to indicate whether the new user record was successfully created</span></span> | <span data-ttu-id="27d55-135">\*\*Deixar vazio\*\*</span><span class="sxs-lookup"><span data-stu-id="27d55-135">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="27d55-136">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="27d55-136">Next steps</span></span>

- [<span data-ttu-id="27d55-137">Como adicionar vários usuários para um cliente</span><span class="sxs-lookup"><span data-stu-id="27d55-137">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)