---
title: Confirmar aceitação do cliente do contrato de nuvem da Microsoft | Partner Center
ms.topic: article
ms.date: 10/29/2018
Description: As a partner, you need to obtain your customer’s acceptance of the Microsoft Cloud Agreement before you can order Microsoft products and services for that customer. To better help partners meet compliance requirements, Microsoft asks partners to confirm acceptance by providing certain details regarding the person who accepted the agreement.
author: v-petand
ms.author: v-petand
keywords: cliente, os clientes, consentimento
ms.localizationpriority: medium
ms.openlocfilehash: 356782420046cb8b49ac4e05981becd253d7049a
ms.sourcegitcommit: dcc0517b2441c5577994b802c455fc726cc5cb35
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/10/2019
ms.locfileid: "9000026"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-cloud-agreement"></a>Confirmar aceitação do cliente do contrato de nuvem da Microsoft

**Aplica-se ao**
-  Partner Center

Como um parceiro, você precisará obter aceitação do cliente do contrato de nuvem da Microsoft antes de você pode solicitar produtos da Microsoft e serviços para esse cliente. Para ajudar melhor os parceiros atender aos requisitos de conformidade, Microsoft solicita que os parceiros para confirmar a aceitação, fornecendo os seguintes detalhes em relação à pessoa que aceitem o contrato: 

-   Nome

-   Sobrenome

-   Email

-   Número de telefone

-   Data de aceitação

Para saber mais, consulte a [confirmação de aceitação de cliente do contrato da Microsoft Cloud perguntas frequentes](https://docs.microsoft.com/en-us/partner-center/confirm-consent-faq).

## <a name="schedule"></a>Agendar

**7 de agosto de 2018**

-   Parceiros de cobrança direta e provedores indiretos podem confirmar aceitação do cliente do contrato de nuvem da Microsoft. Confirmação é *opcional*.

-   Confirmação de aceitação do cliente pode ser feita por meio do Partner Center ou a API do Partner Center.

-   Confirmação de aceitação do cliente é compatível somente com a nuvem pública da Microsoft.


**7 de novembro de 2018**

-   Parceiros de cobrança direta e provedores indiretos **deve** Confirmar aceitação do contrato da Microsoft Cloud do cliente. Confirmação é *obrigatório*.

-   Se a confirmação não for fornecida para um determinado cliente:

    -   Você não será capaz de criar novos pedidos para este cliente.

    -   Você não poderá alterar a quantidade de estações das assinaturas existentes baseados em assento para este cliente.

-   Confirmação de aceitação do cliente pode ser feita por meio do Partner Center ou a API do Partner Center.

-   Confirmação de aceitação do cliente é compatível somente com a nuvem pública da Microsoft.


## <a name="confirming-customer-acceptance-in-partner-center"></a>Confirmar aceitação do cliente no Partner Center

### <a name="confirm-customer-acceptance-for-a-new-customer"></a>Confirmar aceitação do cliente para um novo cliente

Use o procedimento a seguir para confirmar a aceitação do cliente enquanto você cria um novo locatário do cliente no Partner Center. Observe que você deve ser um agente administrador ou agente de vendas para fazer isso. 
1.  Selecione **os clientes**e, em seguida, o **novo cliente** e, em seguida, selecione **as informações de conta**.

2.  Insira as informações sobre a **empresa** e **contato principal**.

![Informações da empresa](images/mca/mca1.png)

3.  Sob o **contrato de nuvem da Microsoft**, selecione **o cliente aceitou o contrato de nuvem da Microsoft mais recente**. 

4.  Em **Data de aceitação do contrato**, insira a data adequada. Você não pode defini-lo para uma data futura.

5.  Insira os detalhes do usuário que é fornecido a aceitação. 

![Adicionar data de aceitação](images/mca/MCA3.png)

Por padrão, as informações de usuário de contato principal são exibidas. Se isso não estiver correto, selecione a **atualização** e, em seguida, insira o **nome**, **Sobrenome**, **endereço de Email**, e **número de telefone* (opcional da pessoa que aceitem o contrato).


6.  Selecione **Avançar** para continuar com as etapas restantes para criar o locatário do cliente.

### <a name="confirm-customer-acceptance-for-an-existing-customer"></a>Confirmar aceitação do cliente para um cliente existente

Você deve ser um agente administrador ou agente de vendas para fazer isso. 

1.  Selecione **clientes**e, em seguida, localize e selecione o cliente que você deseja ver. 

2.  Selecione **as informações de conta**.

3.  Sob o **contrato da Microsoft cloud**, selecione a **atualização**.

![Update](images/mca/mca4.png)

4.  Insira o **nome**, **Sobrenome**, **endereço de Email**e **número de telefone** (opcional do usuário que aceitem o contrato).

5.  Em **Data de aceitação do contrato**, insira a data adequada. Você não pode defini-lo para uma data futura.

6.  Selecione **Salvar e continuar**.

### <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>Confirmar aceitação do cliente durante a criação de novo pedido para um cliente existente

Se você tentar criar uma nova ordem para um cliente existente que você não tiver confirmado antes, você receberá um aviso para concluir a confirmação. Use o procedimento a seguir para fazer isso. 

1.  Insira o **nome**, **Sobrenome**, **endereço de Email**e **número de telefone** (opcional do usuário que aceitem o contrato).

2.  Em **Data de aceitação do contrato**, insira a data adequada. Você não pode defini-lo para uma data futura.

3.  Selecione **Salvar e continuar**.


### <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>Recuperar a confirmação de aceitação do cliente para um cliente existente

Você pode recuperar a confirmação de aceitação do cliente para um cliente existente que você forneceu anteriormente usando o procedimento a seguir. Você deve ser um agente administrador ou agente de vendas para fazer isso. 

1.  Selecione **clientes**e, em seguida, localize e selecione o cliente que você deseja ver. 

2.  Selecione **as informações de conta**.

3.  Sob o **contrato de nuvem da Microsoft**, você verá ou não confirmação foi fornecida para este cliente.

