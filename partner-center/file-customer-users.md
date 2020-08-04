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
ms.openlocfilehash: 07a28e5310716f3df11caa36e51339e877e65627
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/03/2020
ms.locfileid: "87528173"
---
# <a name="add-multiple-users-to-a-customer-account-by-creating-a-csv-file"></a><span data-ttu-id="40d26-103">Adicionar vários usuários a uma conta de cliente criando um arquivo. csv</span><span class="sxs-lookup"><span data-stu-id="40d26-103">Add multiple users to a customer account by creating a .csv file</span></span>

<span data-ttu-id="40d26-104">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="40d26-104">**Applies to**</span></span>

- <span data-ttu-id="40d26-105">Partner Center</span><span class="sxs-lookup"><span data-stu-id="40d26-105">Partner Center</span></span>

<span data-ttu-id="40d26-106">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="40d26-106">**Appropriate roles**</span></span>

- <span data-ttu-id="40d26-107">Administrador global</span><span class="sxs-lookup"><span data-stu-id="40d26-107">Global admin</span></span>

<span data-ttu-id="40d26-108">Adicione vários usuários à conta de um cliente de uma só vez, carregando um arquivo de dados no formato de arquivo de valores separados por vírgula (. csv) no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="40d26-108">Add multiple users to a customer's account all at once, by uploading a data file in the comma-separated value file format (.csv) to the Partner Center.</span></span> <span data-ttu-id="40d26-109">Você pode baixar um arquivo de dados de exemplo do centro de parceiros e, em seguida, editá-lo para seu uso ou pode criar um novo arquivo de dados usando o modelo de dados definido abaixo.</span><span class="sxs-lookup"><span data-stu-id="40d26-109">You can download a sample data file from the Partner Center and then edit it for your use, or you can create a new data file using the data model defined below.</span></span>

## <a name="data-file-requirements"></a><a href="" id="creatingtheimportcsvfile"></a><span data-ttu-id="40d26-110">Requisitos de arquivo de dados:</span><span class="sxs-lookup"><span data-stu-id="40d26-110">Data file requirements</span></span>

<span data-ttu-id="40d26-111">Para adicionar vários usuários à conta de um cliente usando o processo de carregamento em massa, você precisará atender aos seguintes requisitos:</span><span class="sxs-lookup"><span data-stu-id="40d26-111">To add multiple users to a customer's account using the bulk upload process, you'll need to meet the following requirements:</span></span>

- <span data-ttu-id="40d26-112">Você deve ter permissões de administrador global para a conta de cliente;</span><span class="sxs-lookup"><span data-stu-id="40d26-112">You must have global administrator permissions to the customer account;</span></span>
- <span data-ttu-id="40d26-113">Cada usuário deve ter um endereço de email exclusivo, adicionado ao(s) domínio(s) de email do cliente;</span><span class="sxs-lookup"><span data-stu-id="40d26-113">Each user must have a unique email address, appended to the customer's email domain(s);</span></span>
- <span data-ttu-id="40d26-114">Você pode carregar até 100 registros por vez.</span><span class="sxs-lookup"><span data-stu-id="40d26-114">You can upload up to 100 records at a time.</span></span> <span data-ttu-id="40d26-115">Se você precisar adicionar mais de 100 usuários, crie e carregue arquivos de dados adicionais.</span><span class="sxs-lookup"><span data-stu-id="40d26-115">If you need to add more than 100 users, create and upload additional data files.</span></span>
- <span data-ttu-id="40d26-116">Todos os usuários devem estar na mesma **localização** geográfica.</span><span class="sxs-lookup"><span data-stu-id="40d26-116">All users must be in the same geographic **Location**.</span></span>
- <span data-ttu-id="40d26-117">Insira apenas os dados descritos abaixo.</span><span class="sxs-lookup"><span data-stu-id="40d26-117">Enter only the data described below.</span></span> <span data-ttu-id="40d26-118">Dados irrelevantes causarão a falha do upload.</span><span class="sxs-lookup"><span data-stu-id="40d26-118">Extraneous data will cause the upload to fail.</span></span>

<span data-ttu-id="40d26-119">Insira os seguintes dados no arquivo de dados:</span><span class="sxs-lookup"><span data-stu-id="40d26-119">Enter the following data in the data file:</span></span>

| <span data-ttu-id="40d26-120">**Nome da coluna**</span><span class="sxs-lookup"><span data-stu-id="40d26-120">**Column name**</span></span> | <span data-ttu-id="40d26-121">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="40d26-121">**Description**</span></span>  | <span data-ttu-id="40d26-122">**Limitação**</span><span class="sxs-lookup"><span data-stu-id="40d26-122">**Limitation**</span></span>  |
|:-------- |:------  |:----- |
| <span data-ttu-id="40d26-123">Nome</span><span class="sxs-lookup"><span data-stu-id="40d26-123">First name</span></span>  | <span data-ttu-id="40d26-124">Nome do usuário (campo opcional)</span><span class="sxs-lookup"><span data-stu-id="40d26-124">User's first name (optional field)</span></span>  | <span data-ttu-id="40d26-125">limite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="40d26-125">50-character limit</span></span>  |
| <span data-ttu-id="40d26-126">Sobrenome</span><span class="sxs-lookup"><span data-stu-id="40d26-126">Last name</span></span>  | <span data-ttu-id="40d26-127">Sobrenome do usuário (campo opcional)</span><span class="sxs-lookup"><span data-stu-id="40d26-127">User's last name (optional field)</span></span>  | <span data-ttu-id="40d26-128">limite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="40d26-128">50-character limit</span></span>  |
| <span data-ttu-id="40d26-129">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="40d26-129">Display name</span></span>    | <span data-ttu-id="40d26-130">Nome exibido no Partner Center (campo obrigatório)</span><span class="sxs-lookup"><span data-stu-id="40d26-130">Name displayed in the Partner Center (required field)</span></span>                            | <span data-ttu-id="40d26-131">limite de 50 caracteres</span><span class="sxs-lookup"><span data-stu-id="40d26-131">50-character limit</span></span>                         |
| <span data-ttu-id="40d26-132">Email</span><span class="sxs-lookup"><span data-stu-id="40d26-132">Email</span></span>   | <span data-ttu-id="40d26-133">Endereço de email comercial do usuário na empresa do cliente (campo obrigatório)</span><span class="sxs-lookup"><span data-stu-id="40d26-133">User's business email address at customer company (required field)</span></span>           | <span data-ttu-id="40d26-134">Cada usuário deve ter um endereço de e-mail exclusivo</span><span class="sxs-lookup"><span data-stu-id="40d26-134">Each user must have a unique email address</span></span> |
| <span data-ttu-id="40d26-135">Atualização de status</span><span class="sxs-lookup"><span data-stu-id="40d26-135">Status update</span></span>   | <span data-ttu-id="40d26-136">Usado para indicar se o novo registro de usuário foi ou não criado com êxito</span><span class="sxs-lookup"><span data-stu-id="40d26-136">Used to indicate whether or not the new user record was successfully created</span></span> | <span data-ttu-id="40d26-137">\*\*Deixar vazio\*\*</span><span class="sxs-lookup"><span data-stu-id="40d26-137">\*\*Leave empty\*\*</span></span>                        |

## <a name="next-steps"></a><span data-ttu-id="40d26-138">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="40d26-138">Next steps</span></span>

- [<span data-ttu-id="40d26-139">Como adicionar vários usuários a um cliente</span><span class="sxs-lookup"><span data-stu-id="40d26-139">How to add multiple users for a customer</span></span>](adding-multiple-users-to-a-customer-account.md)