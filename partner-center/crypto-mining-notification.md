---
title: Notificação do Partner Center para atividade de mineração de criptografia | Centro de parceiros
ms.topic: article
ms.date: 03/15/2019
description: Notificação sobre o andamento de potencial criptomineração.
author: LauraBrenner
ms.author: labrenne
Keywords: criptografia-mineração, mineração de criptomoeda, segurança
robots: noindex, nofollow
ms.localizationpriority: medium
ms.openlocfilehash: febce4039e1634fb5e82d083f83e2c11ef47040f
ms.sourcegitcommit: 9d01fb30eafc523784ecc3568c05da9bbe9a1e8c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/01/2019
ms.locfileid: "68708844"
---
# <a name="partner-center-notification-for-cryptocurrency-mining-activity"></a><span data-ttu-id="c6255-104">Notificação do Partner Center para atividade de mineração de criptomoeda</span><span class="sxs-lookup"><span data-stu-id="c6255-104">Partner Center notification for cryptocurrency mining activity</span></span>

<span data-ttu-id="c6255-105">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="c6255-105">**Applies to**</span></span>

-  <span data-ttu-id="c6255-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="c6255-106">Partner Center</span></span>
-  <span data-ttu-id="c6255-107">Parceiros CSP</span><span class="sxs-lookup"><span data-stu-id="c6255-107">CSP partners</span></span>

<span data-ttu-id="c6255-108">Você pode ter recebido a seguinte notificação do Partner Center sobre a mineração de criptomoeda:</span><span class="sxs-lookup"><span data-stu-id="c6255-108">You may have received the following Partner Center notification about cryptocurrency mining:</span></span>
 
![Imagem de notificação de segurança no Partner Center](images/crypto1.png)

<span data-ttu-id="c6255-110">A finalidade dessa notificação é informá-lo de que detectamos mineração de criptomoedas em uma ou mais das suas assinaturas do Azure na semana passada.</span><span class="sxs-lookup"><span data-stu-id="c6255-110">The purpose of this notification is to inform you that we've detected cryptocurrency mining on one or more of your Azure subscriptions within the past week.</span></span> <span data-ttu-id="c6255-111">A mineração de criptomoedas não significa necessariamente que houve uma atividade fraudulenta.</span><span class="sxs-lookup"><span data-stu-id="c6255-111">Cryptocurrency mining does not necessarily equal fraudulent activity.</span></span> <span data-ttu-id="c6255-112">No entanto, é incomum porque o custo da execução da mineração de criptomoedas no Azure tende a superar qualquer recompensa financeira em potencial.</span><span class="sxs-lookup"><span data-stu-id="c6255-112">However, it's unusual because the cost of running cryptocurrency mining in Azure tends to outweigh any potential financial rewards.</span></span> <span data-ttu-id="c6255-113">Para proteger-se contra fraude financeira que possa afetar você ou seu cliente, considere as seguintes etapas:</span><span class="sxs-lookup"><span data-stu-id="c6255-113">To protect against financial fraud that may impact you or your customer, consider the following steps:</span></span>

1.  <span data-ttu-id="c6255-114">Analise e confirme se a conta do cliente tem boa reputação.</span><span class="sxs-lookup"><span data-stu-id="c6255-114">Review and confirm that the customer account is in good standing.</span></span> <span data-ttu-id="c6255-115">Você pode acessar a assinatura diretamente clicando na notificação.</span><span class="sxs-lookup"><span data-stu-id="c6255-115">You can access the subscription directly by clicking on the notification.</span></span>

2.  <span data-ttu-id="c6255-116">Analise os padrões de uso do Azure para a assinatura.</span><span class="sxs-lookup"><span data-stu-id="c6255-116">Review Azure usage patterns for the subscription.</span></span> <span data-ttu-id="c6255-117">Picos repentinos podem sugerir atividades inesperadas.</span><span class="sxs-lookup"><span data-stu-id="c6255-117">Sudden spikes may suggest unexpected activity.</span></span>

3.  <span data-ttu-id="c6255-118">Contate o cliente para confirmar se a atividade é esperada.</span><span class="sxs-lookup"><span data-stu-id="c6255-118">Contact the customer to confirm that the activity is expected.</span></span>

<span data-ttu-id="c6255-119">Se a atividade for esperada, retorne à página de detalhes da assinatura do Azure do cliente e confirme se a mineração de criptomoedas é legítima.</span><span class="sxs-lookup"><span data-stu-id="c6255-119">If the activity is expected, return to the customer's Azure subscription detail page and confirm that the cryptocurrency mining is legitimate.</span></span> 


![Imagem da página de detalhes da assinatura do Azure do cliente](images/crypto2.png)

<span data-ttu-id="c6255-121">Se a atividade for inesperada, considere o seguinte:</span><span class="sxs-lookup"><span data-stu-id="c6255-121">If the activity is unexpected, consider the following:</span></span>

1.  <span data-ttu-id="c6255-122">Confirme se os recursos do Azure para mineração de criptomoedas não são necessários e os exclua para evitar outros encargos do Azure.</span><span class="sxs-lookup"><span data-stu-id="c6255-122">Confirm that the Azure resources for cryptocurrency mining are not needed and delete them to avoid further Azure charges.</span></span>

2.  <span data-ttu-id="c6255-123">Para começar, entenda como os recursos foram criados.</span><span class="sxs-lookup"><span data-stu-id="c6255-123">Understand how the resources were created in the first place.</span></span> <span data-ttu-id="c6255-124">Isso pode exigir que você analise os logs do Gerenciamento de Recursos do Azure para atividades de provisionamento de recursos.</span><span class="sxs-lookup"><span data-stu-id="c6255-124">This may require you to review the Azure Resource Management logs for resource provisioning activities.</span></span>

3.  <span data-ttu-id="c6255-125">Se você precisar descobrir quem criou a assinatura, examine os logs de atividade do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="c6255-125">If you need to find out who created the subscription, review Partner Center activity logs.</span></span>

<span data-ttu-id="c6255-126">A detecção de atividades de mineração de criptomoedas se baseia em heurística e pode não ser 100% precisa.</span><span class="sxs-lookup"><span data-stu-id="c6255-126">Detection of cryptocurrency mining activities is based on heuristics and may not be 100% accurate.</span></span> <span data-ttu-id="c6255-127">Verifique se há sistemas de governança e de monitoramento preparados para proteger contra atividades fraudulentas ou outras atividades não permitidas.</span><span class="sxs-lookup"><span data-stu-id="c6255-127">Be sure to have governance and monitoring systems in place to protect against fraudulent or other unpermitted activities.</span></span> <span data-ttu-id="c6255-128">Para obter mais informações, consulte [Não pagamento, fraude ou uso indevido](https://docs.microsoft.com/partner-center/non-payment--fraud--or-misuse).</span><span class="sxs-lookup"><span data-stu-id="c6255-128">For more information, see [Non-payment, fraud, or misuse](https://docs.microsoft.com/partner-center/non-payment--fraud--or-misuse).</span></span>

<span data-ttu-id="c6255-129">Se tiver dúvidas ou preocupações sobre a notificação, você pode usar o procedimento a seguir para abrir uma solicitação de suporte.</span><span class="sxs-lookup"><span data-stu-id="c6255-129">If you have questions or concerns about the notification, you can use the following procedure to open a support request.</span></span>

1.  <span data-ttu-id="c6255-130">No Partner Center, selecione **suporte** e, em seguida, selecione **solicitações do Partner Center**.</span><span class="sxs-lookup"><span data-stu-id="c6255-130">In the Partner Center, select **Support** and then select **Partner Center requests**.</span></span>
3.  <span data-ttu-id="c6255-131">Selecione **Nova solicitação**.</span><span class="sxs-lookup"><span data-stu-id="c6255-131">Select **New Request**.</span></span> 
4.  <span data-ttu-id="c6255-132">No menu suspenso **Tipo de problema**, selecione **Adding or managing customers**.</span><span class="sxs-lookup"><span data-stu-id="c6255-132">In the **Type of problems** dropdown menu, select **Adding or managing customers**.</span></span>
5.  <span data-ttu-id="c6255-133">No menu suspenso **Impacto**, selecione **Moderado**.</span><span class="sxs-lookup"><span data-stu-id="c6255-133">In the **Impact** dropdown menu, select **Moderate**.</span></span>
6.  <span data-ttu-id="c6255-134">No campo **Título**, insira **Crypto-mining notification**.</span><span class="sxs-lookup"><span data-stu-id="c6255-134">In the **Title** field, enter **Crypto-mining notification**.</span></span>
7.  <span data-ttu-id="c6255-135">No campo **Descrição**, insira o nome da assinatura afetada juntamente com suas outras dúvidas ou preocupações.</span><span class="sxs-lookup"><span data-stu-id="c6255-135">In the **Description** field, enter the name of the affected subscription along with your other questions or concerns.</span></span> 
8.  <span data-ttu-id="c6255-136">Insira suas informações de contato.</span><span class="sxs-lookup"><span data-stu-id="c6255-136">Enter your contact information.</span></span>
9.  <span data-ttu-id="c6255-137">Selecione **Enviar**.</span><span class="sxs-lookup"><span data-stu-id="c6255-137">Select **Submit**.</span></span>



