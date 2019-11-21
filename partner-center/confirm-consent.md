---
title: Confirmar a aceitação do cliente do Contrato do Microsoft Cloud | Partner Center
ms.topic: article
ms.date: 11/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Learn how to confirm customer acceptance of the Microsoft Cloud Agreement. This may be needed to order Microsoft products and services for customers.
author: LauraBrenner
ms.author: labrenne
keywords: customer, customers, consent, MCA, Microsoft Cloud Agreement, customer agreement templates
ms.localizationpriority: medium
ms.openlocfilehash: d9b2df8f9cf8795eedb75bc23773942e365c83fe
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/20/2019
ms.locfileid: "74252585"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-cloud-agreement"></a>Confirmar a aceitação do cliente do Contrato do Microsoft Cloud

**Aplica-se a**
-  Partner Center

> [!NOTE]
> The Agreement resource is currently supported by Partner Center in the Microsoft public cloud only. It is not applicable to:
> * Partner Center operado pela 21Vianet
> * Partner Center do Microsoft Cloud Germany
> * Partner Center do Microsoft Cloud for US Government

>[!NOTE]
>This agreement is valid until January 31, 2020. After that date, all customers, existing and new, must sign the new Microsoft Customer Agreement. To learn more, read [Confirm customer acceptance of the Microsoft Customer Agreement](confirm-customer-agreement.md).

As a partner, you need to obtain your customer's acceptance of the Microsoft Cloud Agreement before you can order Microsoft products and services for that customer. Para ajudar mais os parceiros a atender os requisitos de conformidade, a Microsoft solicita que os parceiros confirmem a aceitação fornecendo os detalhes a seguir em relação à pessoa que aceitou o contrato: 

-   Nome

-   Sobrenome

-   Endereço de email

-   Número de telefone (opcional)

-   Data da aceitação

To learn more, see the Microsoft Cloud Agreement customer acceptance confirmation [Frequently Asked Questions](https://docs.microsoft.com/partner-center/confirm-consent-faq).

Direct bill partners and Indirect Providers must confirm customer acceptance of the Microsoft Cloud Agreement when transacting through Partner Center or Partner Center API. A confirmação é *obrigatória*.

Se a confirmação não for fornecida por um determinado cliente:

-   You won't be able to create new orders for this customer.

-   You won't be able to change the seat count of existing seat-based subscriptions for this customer.

Confirmation of customer acceptance can be done via Partner Center or the Partner Center API. To do this through the Partner Center API, see the following topics: 

-   [Get confirmation of customer consent](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-consent)

-   [Get agreement metadata](https://docs.microsoft.com/partner-center/develop/get-agreement-metadata)

-   [Confirm customer consent](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent)


This applies to both production and sandbox environments.

## <a name="confirming-customer-acceptance-in-partner-center"></a>Confirming customer acceptance in Partner Center

### <a name="confirm-customer-acceptance-for-a-new-customer"></a>Confirmar a aceitação do cliente para um novo cliente

Use the following procedure to confirm customer acceptance while you create a new customer tenant in Partner Center. Observe que você deve ser um Agente administrativo ou Agente de vendas para fazer isso.

1. Select **Customers**, and then **New customer** and then select **Account info**.
2. Insira as informações sobre a **Empresa** e o **Contato principal**.

![Company information](images/mca/mca1.png)

3. Em **Contrato do Microsoft Cloud**, selecione **O cliente aceitou o último contrato do Microsoft Cloud**.
4. Em **Data de aceitação do contrato**, insira a data apropriada. Você não pode definir isso como uma data futura.
5. Insira os detalhes do usuário que forneceu a aceitação.

![Add acceptance date](images/mca/MCA3.png)

Por padrão, as informações de usuário do contato principal são exibidas. If this isn't correct, select **Update** and then enter the **First name**, **Last name**, **Email address**, and **Phone number* (optional) of the person who accepted the agreement.

6. Selecione **Avançar** para continuar com as etapas restantes para criar o locatário do cliente.

### <a name="confirm-customer-acceptance-for-an-existing-customer"></a>Confirmar a aceitação do cliente para um cliente existente

Você deve ser um Agente administrativo ou Agente de vendas para fazer isso.

1. Selecione **Clientes** e então localize e selecione o cliente que você deseja ver.
2. Selecione **Informações da Conta**.
3. Em **Contrato do Microsoft Cloud**, selecione **Atualizar**.

![Atualizar](images/mca/mca4.png)

4. Insira o **Nome**, **Sobrenome**, **Email** e **Número de telefone** (opcional) do usuário que aceitou o contrato.
5. Em **Data de aceitação do contrato**, insira a data apropriada. Você não pode definir isso como uma data futura.
6. Selecione **Salvar e continuar**.

### <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>Confirmar a aceitação do cliente ao criar o novo pedido para um cliente existente

If you try to create a new order for an existing customer which you have not confirmed before, you'll receive a prompt to complete the confirmation. Use o procedimento a seguir para fazer isso.

1. Insira o **Nome**, **Sobrenome**, **Email** e **Número de telefone** (opcional) do usuário que aceitou o contrato.
2. Em **Data de aceitação do contrato**, insira a data apropriada. Você não pode definir isso como uma data futura.
3. Selecione **Salvar e continuar**.

### <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>Recuperar a confirmação da aceitação do cliente para um cliente existente

Você pode recuperar a confirmação da aceitação do cliente para um cliente existente que você forneceu anteriormente usando o procedimento abaixo. Você deve ser um Agente administrativo ou Agente de vendas para fazer isso.

1. Selecione **Clientes** e então localize e selecione o cliente que você deseja ver.
2. Selecione **Informações da Conta**.
3. Under **Microsoft cloud agreement**, you'll see whether or not confirmation has been provided for this customer.
