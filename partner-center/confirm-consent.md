---
title: Confirmar a aceitação do cliente do Contrato do Microsoft Cloud | Partner Center
ms.topic: article
ms.date: 04/16/2019
Description: Como um parceiro, você precisa obter a aceitação do cliente do Contrato do Microsoft Cloud antes de você poder encomendar produtos e serviços Microsoft e serviços para o cliente. A melhor ajuda parceiros atende aos requisitos de conformidade, a Microsoft solicita parceiros para confirmar a aceitação fornecendo determinados detalhes sobre a pessoa que aceitou o contrato.
author: LauraBrenner
ms.author: v-petand
keywords: cliente, clientes, consentir, MCA, contrato do Microsoft Cloud, modelos de contrato do cliente
ms.localizationpriority: medium
ms.openlocfilehash: 9dad303b419f3dadd33f4937933638c60c45994b
ms.sourcegitcommit: 7022f1e3d26751e66f90db96bf6d881cb2a694d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2019
ms.locfileid: "59652248"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-cloud-agreement"></a>Confirmar a aceitação do cliente do Contrato do Microsoft Cloud

**Aplica-se a**
-  Partner Center

> [!NOTE]
> Partner Center em que a nuvem pública da Microsoft somente no momento, há suporte para o recurso de contrato. Não é aplicável a:
> * Partner Center operado pela 21Vianet
> * Partner Center do Microsoft Cloud Germany
> * Partner Center para Microsoft Cloud for US Government

Como um parceiro, você precisa obter a aceitação do cliente do Contrato do Microsoft Cloud antes de você poder encomendar produtos e serviços Microsoft e serviços para o cliente. Para ajudar mais os parceiros a atender os requisitos de conformidade, a Microsoft solicita que os parceiros confirmem a aceitação fornecendo os detalhes a seguir em relação à pessoa que aceitou o contrato: 

-   Nome

-   Sobrenome

-   Endereço de email

-   Número de telefone (opcional)

-   Data da aceitação

Para obter mais informações, consulte a confirmação de aceitação do cliente contrato do Microsoft Cloud [Frequently Asked Questions](https://docs.microsoft.com/en-us/partner-center/confirm-consent-faq).

Parceiros de fatura direto e provedores indiretos devem confirmar aceitação do cliente do contrato de nuvem da Microsoft quando transacionar por meio do Partner Center ou a API do Partner Center. A confirmação é *obrigatória*.

Se a confirmação não for fornecida por um determinado cliente:

-   Você não conseguirá criar novos pedidos para esse cliente.

-   Você não poderá alterar a contagem de estações de assinaturas baseadas em estação existentes para esse cliente.

Confirmação da aceitação do cliente pode ser feita por meio do Partner Center ou a API do Partner Center. Para fazer isso por meio da API do Partner Center, consulte os tópicos a seguir: 

-   [Obter a confirmação de consentimento do cliente](https://docs.microsoft.com/en-us/partner-center/develop/get-confirmation-of-customer-consent)

-   [Obter metadados de contrato](https://docs.microsoft.com/en-us/partner-center/develop/get-agreement-metadata)

-   [Confirme se o consentimento do cliente](https://docs.microsoft.com/en-us/partner-center/develop/confirm-customer-consent)


Isso se aplica a ambientes de área restrita e de produção.

## <a name="confirming-customer-acceptance-in-partner-center"></a>Confirmar a aceitação do cliente no Partner Center

### <a name="confirm-customer-acceptance-for-a-new-customer"></a>Confirmar a aceitação do cliente para um novo cliente

Use o procedimento a seguir para confirmar a aceitação do cliente enquanto você cria um novo locatário do cliente no Partner Center. Observe que você deve ser um Agente administrativo ou Agente de vendas para fazer isso.
 
1.  Selecione **clientes**e então **novo cliente** e, em seguida, selecione **informações de conta**.

2.  Insira as informações sobre a **Empresa** e o **Contato principal**.

![Informações da empresa](images/mca/mca1.png)

3.  Em **Contrato do Microsoft Cloud**, selecione **O cliente aceitou o último contrato do Microsoft Cloud**. 

4.  Em **Data de aceitação do contrato**, insira a data apropriada. Você não pode definir isso como uma data futura.

5.  Insira os detalhes do usuário que forneceu a aceitação. 

![Adicionar data de aceitação](images/mca/MCA3.png)

Por padrão, as informações de usuário do contato principal são exibidas. Se isso não estiver correto, selecione **Atualizar** e insira o **Nome**, **Sobrenome**, **Email** e **Número de telefone* (opcional) da pessoa que aceitou o contrato.

6.  Selecione **Avançar** para continuar com as etapas restantes para criar o locatário do cliente.

### <a name="confirm-customer-acceptance-for-an-existing-customer"></a>Confirmar a aceitação do cliente para um cliente existente

Você deve ser um Agente administrativo ou Agente de vendas para fazer isso. 

1.  Selecione **Clientes** e então localize e selecione o cliente que você deseja ver. 

2.  Selecione **informações de conta**.

3.  Em **Contrato do Microsoft Cloud**, selecione **Atualizar**.

![Atualização](images/mca/mca4.png)

4.  Insira o **Nome**, **Sobrenome**, **Email** e **Número de telefone** (opcional) do usuário que aceitou o contrato.

5.  Em **Data de aceitação do contrato**, insira a data apropriada. Você não pode definir isso como uma data futura.

6.  Selecione **Salvar e continuar**.

### <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>Confirmar a aceitação do cliente ao criar o novo pedido para um cliente existente

Se tentar criar um novo pedido para um cliente existente que não confirmou antes, você receberá um aviso para concluir a confirmação. Use o procedimento a seguir para fazer isso. 

1.  Insira o **Nome**, **Sobrenome**, **Email** e **Número de telefone** (opcional) do usuário que aceitou o contrato.

2.  Em **Data de aceitação do contrato**, insira a data apropriada. Você não pode definir isso como uma data futura.

3.  Selecione **Salvar e continuar**.


### <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>Recuperar a confirmação da aceitação do cliente para um cliente existente

Você pode recuperar a confirmação da aceitação do cliente para um cliente existente que você forneceu anteriormente usando o procedimento abaixo. Você deve ser um Agente administrativo ou Agente de vendas para fazer isso. 

1.  Selecione **Clientes** e então localize e selecione o cliente que você deseja ver. 

2.  Selecione **informações de conta**.

3.  Em **Contrato do Microsoft Cloud**, você verá se a confirmação foi fornecida ou não para este cliente.

