---
title: Migrate Dynamics AX subscriptions to Dynamics 365 | Partner Center
description: Microsoft introduces Dynamics 365, the next generation of intelligent business applications that enable your organization to grow, evolve and transform to meet the needs of your customers and capture new opportunities.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: MaggiePucciEvans
ms.openlocfilehash: 39f254488dab4335a24a5a36fc593d2e281adbf8
ms.sourcegitcommit: 2c948321945d0e61153f7d766a1a669782df4a54
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2017
---
# <a name="migrate-dynamics-ax-subscriptions-to-dynamics-365"></a>Migrate Dynamics AX subscriptions to Dynamics 365

**Applies to**

-  Partner Center

Microsoft introduces Dynamics 365, the next generation of intelligent business applications that enable your organization to grow, evolve and transform to meet the needs of your customers and capture new opportunities. Como parte do novo produto, a Microsoft apresentou novos planos de assinatura do Microsoft Dynamics para clientes em 1º de novembro de 2016, que são semelhantes, mas não idênticos aos seus planos atuais.

As instruções neste documento descrevem como provedores indiretos podem migrar as assinaturas existentes do Microsoft Dynamics AX dos clientes para o novo Microsoft Dynamics 365. The instructions also apply to other Microsoft products that update to new versions, requiring providers to migrate customers’ subscriptions to a new SKU.

Os planos do Microsoft Dynamics CRM Online e AX forem desativados.  Desde 1 de julho de 2017, você não pode renovar em planos legados, e assinaturas E4 existentes não serão renovadas automaticamente quando expiram.

Quando as assinaturas CRM Online e AX terminarem, elas serão canceladas. Para garantir a continuidade dos clientes, você deve fazer a transição de clientes com assinaturas E4 vencidas para uma opção de SKU com suporte, listada abaixo. É recomendável mover os clientes para as novas assinaturas antes da data de término da assinatura anual, para evitar possíveis interrupções de serviço. 

Na página de detalhes da assinatura, o status da assinatura E4 foi alterado para "Expira em [data]" de "Renovação automática em [data]". 

Se você usar a API (CREST ou Partner Center), você pode descobrir assinaturas vencidas avaliando a data de término da assinatura juntamente com a propriedade de renovação automática = Falso. Você pode mover os clientes para um novo plano a qualquer momento. 

**Alterações de licenciamento do Microsoft Dynamics AX**

A linha de produtos Microsoft Dynamics AX foi desativada, em vigor a partir de 1º de novembro de 2016. Para saber mais sobre as novas opções de licenciamento do Dynamics 365, examine o [Guia de Licenciamento](http://download.microsoft.com/documents/dynamics/pricing/Dynamics_365_Enterprise_edition_Licensing_Guide.pdf).

 Consulte a tabela a seguir para obter detalhes sobre o mapeamento de licenças:

|**SKU desativado**   |**Dynamics 365 SKU**   |
|-------------------|:----------------------|
|Enterprise SKU|Microsoft Dynamics 365 for Unified Operations ou Microsoft Dynamics 365 Plan |
|Tarefa|MB2-717: Microsoft Dynamics 365 for Sales
|Tarefa/autoatendimento|Microsoft Dynamics 365 for Team Members|
|Dispositivo|Microsoft Dynamics 365 for Operations Device|

## <a name="microsoft-dynamics-crm-online-licensing-changes"></a>Alterações de licenciamento do Microsoft Dynamics CRM Online 

**Microsoft Dynamics CRM Online**

A partir de 1º de novembro de 2016, o plano Microsoft Dynamics CRM Online atual estará desativado. Para saber mais sobre as novas opções de licenciamento do microsoft Dynaics 365, revise o [guia de licenciamento](http://download.microsoft.com/documents/dynamics/pricing/Dynamics_365_Enterprise_edition_Licensing_Guide.pdf). Consulte [Informações importantes para clientes do CRM Online](https://go.microsoft.com/fwlink/?linkid=831667) para saber mais sobre as novas opções de licenciamento.

Consulte a tabela a seguir para obter detalhes sobre o mapeamento de licenças:

|**SKU desativado**   |**Dynamics 365 SKU**   |
|-------------------|:----------------------|
|Enterprise|Plano de engajamento do cliente Dynamics 365 Enterprise |
|Professional|Plano de engajamento de cliente do Dynamics 365 Enterprise, Dynamics 365 for Sales ou Dynamics 365 for Customer Service|
|Básico|Dynamics 365 for Team Members, Dynamics 365 for Sales, Dynamics 365 for Customer Service, or plano de engajamento de cliente Dynamics 365 Enterprise|
|Essential|Dynamics 365 for Team Member|
|Complemento do serviço de campo|Plano de envolvimento de cliente do Dynamics 365 Enterprise ou Dynamics 365 for Field Service|
|Complemento de automação de serviço de projeto|Plano de envolvimento de cliente do Dynamics 365 ou Dynamics 365 for Project Service Automation|



## <a name="transition-customers-to-new-product-plans"></a>Transição dos clientes para novos planos do produto


Microsoft continuously offers new products and services to resellers and providers. In these cases, a reseller may need to upgrade customers to new services or migrate their subscriptions from SKUs that will eventually be shut down. Migrating customers from old SKUs to newer ones requires the following sequence:

-   [Purchase the new subscription](#manual-subscription-migration-purchasenewsubsc);
-   [Re-assign current user licenses](#manual-subscription-migration-reassignlicenses);
-   [Cancelar a assinatura antiga](#manual-subscription-migration-cancelsubscriptions).

Nos procedimentos a seguir, você migrará um cliente do Microsoft Dynamics AX ou CRM Online para o Dynamics 365.

O revendedor precisa migrar o cliente com uma assinatura existente do Dynamics AX Enterprise para o Dynamics 365 for Operations. A primeira etapa é comprar o Dynamics 365 for Operations.  Repita essas etapas para um cliente CRM Online mudando para o Microsoft Dynamics 365.

<a href="" id="purchasenewsubsc"></a>

**Comprar a nova assinatura**

1.  From the **Dashboard** menu, select **Customers**, select the customer you wish to move, and choose **Add Subscriptions**.
2.  Select the subscription you want to purchase from the catalog (in this case, Dynamics 365 for Operations, Enterprise Edition), enter the number of licenses, and choose **Submit**.

    Your customer should now have both old and new subscriptions: in this example, the old Dynamics AX Enterprise, and the new ‘target’ subscription, Dynamics 365 for Operations, Enterprise Edition.

<a href="" id="reassignlicenses"></a> The next step is to reassign all existing user licenses to the new subscription.

**Reassign user licenses**

1.  From the **Dashboard** menu, select **Customers**, select the customer you wish to move, and choose **Users and licenses**. The customer’s Users and Licenses page opens.
2.  To re-assign user licenses, select the user to reassign and then select **Manage licenses**.
3.  On the **Manage licenses** page, clear the **Dynamics AX Enterprise** license check box and select the **Dynamics 365 for Operations** license.
4.  Select **Submit**. A confirmation page lists the new license assignments.
5.  Continue the same steps with any other customer users that need license reassignment.

<a href="" id="cancelsubscriptions"></a> After moving the user licenses to the new service, you can safely cancel the old subscription at the top Customer level.

**Cancel the old subscription**

1.  From the **Dashboard** menu, select **Customers**, select the customer you wish to move, and select the subscription you want to cancel.
2.  In the subscription details page, set the subscription **Status** to **Suspended**.
3.  Select **Submit**.

The old subscription is suspended, and the new subscription is active. The suspended subscription will automatically be de-provisioned after 120 days. The customer incurs no additional costs for the old subscription.

## <a name="additional-considerations"></a>Additional considerations


If your customer is moving from the Open Channel to the Cloud Services Program for further subscription provisioning, you will also need to migrate their existing subscriptions:

-   If the customer received their old subscription through the Open Channel, moving to the CSP on the new SKU is straightforward.
-   If the customer is not yet established as your customer, you can invite them. For information, see the [Request a relationship with a customer](https://msdn.microsoft.com/en-us/library/partnercenter/mt750320.aspx) help topic.

After the customer accepts you as their indirect provider, the provisioning steps are mostly the same as described above: you purchase the new subscription, and then assign the user licenses. The only difference involves cancellation of old subscription(s). A new provider cannot cancel suspend/cancel subscriptions acquired via other channels. If the customer acquired prior subscriptions in another sales channel, such as the Open channel, the customer will need to cancel it themselves through that channel.

 

 



