---
title: Criar, suspender ou cancelar assinaturas de cliente | Centro de parceiros
ms.topic: article
ms.date: 11/20/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Learn how to sell your customers subscriptions to products in the catalog after you have created a customer record in Partner Center.
ms.assetid: E95F1538-60E1-464C-B72B-52764BF3A820
author: LauraBrenner
ms.author: labrenne
Keywords: subscription, create new, add subscription, suspend, cancel, suspension, suspend, SaaS, license, ISV, third party
ms.localizationpriority: medium
ms.openlocfilehash: d829ba7ee520cab42ec5985ac2156ddff60d8e99
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253454"
---
# <a name="create-suspend-or-cancel-customer-subscriptions"></a>Criar, suspender ou cancelar assinaturas de clientes

**Aplica-se a**

-  Partner Center
-  Partner Center do Microsoft Cloud for US Government
-  Parceiros CSP

**Appropriate roles**

- Administração global
- Agente administrativo

Depois de criar um registro de seu cliente no Partner Center, você pode vender as assinaturas para os produtos no catálogo. This includes products published by Microsoft as well as Software as a Service (SaaS) products published by third-party Independent Software Vendors (ISVs) to the [commercial marketplace](https://azuremarketplace.microsoft.com/marketplace). 

Note que algumas ofertas são limitadas a uma assinatura por cliente. Para ver uma lista das ofertas restritas, visite a página Ofertas e Preços do Partner Center.

>[!IMPORTANT]
As a partner in the CSP program, you can only purchase **license-based** SaaS subscriptions from ISV publishers within Partner Center. This means you can purchase any **license-based** SaaS offer the ISV publisher has made available to you, including [exclusive offers](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to which you have access. To purchase or manage other, commercial marketplace offers from ISVs (such as **usage-based**, metered or consumption-based offers involving Azure applications, Containers or VMs), you must go to the [Azure management portal](https://portal.azure.com/). For more information, see [Purchase commercial marketplace products](csp-commercial-marketplace-purchase.md).

## <a name="create-a-new-subscription"></a>Crie uma nova assinatura

1. Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).

2. No menu do centro de parceiros, **selecione**clientes e, em seguida, escolha um cliente na lista.

3. Selecione **Adicionar assinatura**. The **Online Services** tab will show all available Marketplace SaaS offers.

4. Para ver apenas determinados tipos de assinaturas, faça seleções nos filtros disponíveis:
   - **Publisher**: Choose **Microsoft** to see only offers from Microsoft, or **Partner** to see commercial marketplace products published by ISVs.
   - **Billing type**: Select the type of subscription billing you want to use: **License** or **Usage**. Consulte [as perguntas frequentes sobre](faq-about-new-billing-features.md) novos recursos de cobrança para obter informações que o ajudarão a decidir entre a frequência de cobrança mensal e anual.
   - **Category**: Choose **Enterprise**, **Small business**, or **Trial**. Para obter informações sobre assinaturas de avaliação, consulte [oferecer a seus clientes avaliações de produtos da Microsoft](offer-your-customers-trials-of-microsoft-products.md).

5. Select the product subscriptions you want to purchase for your customer. The products you see depend on the type of customer segment (education, government, etc.) and the filters you have applied. Some offers shown on the Marketplace may not always be available to a specific customer or a specific CSP partner. This can be because:

    - The customer already has a subscription to that product and is only allowed one

    - The customer's subscription may have been suspended (In this case, you can reactivate the subscription rather than purchase a new one.)
    
    - For ISV SaaS offers, there may be a few reasons why the offer is not available to purchase: The ISV may not support the customer's billing country or region; the ISV may have chosen not to make the offer available through the CSP program; or, the ISV may have made the offer [exclusive](csp-commercial-marketplace-discover.md#learn-about-marketplace-exclusive-offers) to only certain CSP partners. The ISV offer may also not be transactable through the Partner Center (e.g. containers or some usage-based offers).  

6. For each subscription you want to add, enter the number of licenses (if needed) and select **Add to cart**.

7. When you are finished adding subscriptions, select **Review** and review your order.

8. Once you've reviewed your orders and are ready to purchase these subscriptions, select **Buy**.

9. After you buy a subscription for a customer, the following will occur:

    - You can review or edit the subscription by selecting the subscription name from that customer's **Subscriptions** page. A partir daqui, você pode selecionar licenças de complemento, se houver alguma disponível, alterar a quantidade de licenças ou suspender a assinatura.

    **For ISV SaaS (license-based) subscriptions:**
    - You will receive a link to the ISV publisher's site. This link should help you complete the deployment or account setup of the customer's subscription. (Note that neither you nor your customer will receive an email with instructions to complete account set up/provisioning for this type of ISV subscription.)
    
    - If your subscription comes with a 30-day free trial, the free trial period will be applied automatically. As a partner in the CSP program, you cannot waive the free trial period on offers you purchase for customers. Once the free trial period ends, the subscription term will begin and the subscription will convert to paid. The subscription will then auto-renew according to the same schedule.

## <a name="suspend-or-cancel-a-subscription"></a>Suspender ou cancelar uma assinatura

Os parceiros podem suspender ou cancelar uma assinatura se solicitado pelo cliente ou em casos de fraude ou falta de pagamento.

### <a name="suspend-a-subscription"></a>Suspender uma assinatura

Quando você alterar o status de uma assinatura para **Suspensa**, os usuários não poderão entrar nem acessar os serviços.

1. Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).

2. No menu do centro de parceiros, **selecione**clientes e, em seguida, escolha um cliente na lista.

3. Escolha a assinatura que deseja gerenciar.

4. Na seção **Status**, escolha **Suspensa**. Em seguida, **Envie**  suas alterações.

5. Todos os dados serão excluídos, a menos que a assinatura seja reativada dentro de 90 dias ou 90 dias mais o número de dias entre a hora em que a conta foi aberta e o primeiro período de cobrança (máximo de 120 dias).

Quando você suspende uma assinatura, a data que você vê abaixo **do** botão suspenso indica quando a assinatura expirará automaticamente se você não a reativar. For more information, see [FAQ about new billing features](faq-about-new-billing-features.md).

### <a name="cancel-a-subscription"></a>Cancelar uma assinatura

You have the option to cancel license-based SaaS subscriptions from third-party ISV publishers within the Partner Center [commercial marketplace](csp-commercial-marketplace-overview.md). As long as you cancel within the cancellation period, you will receive a full refund.

For ISV offers billed monthly:

- If you cancel less than 24 hours after you placed the order, you will receive a full credit on the next invoice.

- If you cancel later than 24 hours after you placed the order, the cancellation will be scheduled to occur at renewal.

For offers billed annually:

- If you cancel less than 14 days after you place the order, you will receive a full credit on the next invoice.

- If you cancel later than 14 days after you place the order, the cancellation will be scheduled to occur at renewal.

After these periods are over, you will no longer see the option to cancel the subscription.

> [!NOTE]
> Usage-based and metered, third-party ISV services (that use virtual machines or containers, for example) are not eligible for return. Usage-based services can be de-provisioned as a cancellation method. Since charges are billed after use, these services are not eligible for a refund.

To cancel a license-based SaaS subscription from an ISV publisher, do the following:

1. Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).

2. No menu do centro de parceiros, **selecione**clientes e, em seguida, escolha um cliente na lista.

3. Locate the subscription you want to cancel.

4. In the **Status** column, select **Cancel**. Em seguida, **Envie**  suas alterações.

5. If a dialog box appears, fill out any relevant details then select **Submit**.

6. To confirm the cancellation, select **Yes, cancel**.

> [!NOTE]
> You can also choose to cancel an Azure Marketplace subscription using APIs. To do so, see [Cancel an Azure Marketplace subscription](https://docs.microsoft.com/partner-center/develop/cancel-an-azure-marketplace-subscription).

### <a name="choose-whether-to-automatically-renew-a-commercial-marketplace-subscription"></a>Escolha se deseja renovar automaticamente uma assinatura do Marketplace comercial

Por padrão, as assinaturas ativas são definidas para renovar automaticamente quando o período de assinatura expira. Para [assinaturas para produtos](csp-commercial-marketplace-overview.md)do Marketplace comercial, opcionalmente, você pode optar por não renovar automaticamente a assinatura.

To stop an active commercial marketplace subscription from automatically renewing:

1. Sign into the Partner Center [dashboard](https://partner.microsoft.com/dashboard).

2. No menu do centro de parceiros, **selecione**clientes e, em seguida, escolha um cliente na lista.

3.  Select **Subscriptions**. This lists any license-based subscriptions you have purchased for the customer.

4.  In the **Subscription** column, select the subscription you want to modify.

5. In the subscription details page, locate the **Status** section and uncheck the **Auto-renew** box. 

6. Selecione **Enviar**.

## <a name="see-also"></a>Consulte também

- [Purchase commercial marketplace products for your customers](csp-commercial-marketplace-purchase.md)
- [Manage commercial marketplace products for your customers](csp-commercial-marketplace-manage.md)
- [Commercial marketplace overview](csp-commercial-marketplace-overview.md)


