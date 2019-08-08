---
title: Confirmar a aceitação do cliente do Contrato do Microsoft Cloud | Partner Center
ms.topic: article
ms.date: 04/16/2019
Description: Como um parceiro, você precisa obter a aceitação do cliente do Contrato do Microsoft Cloud antes de você poder encomendar produtos e serviços Microsoft e serviços para o cliente. Para ajudar melhor os parceiros a atender aos requisitos de conformidade, a Microsoft solicita que os parceiros confirmem a aceitação fornecendo determinados detalhes sobre a pessoa que aceitou o contrato.
author: LauraBrenner
ms.author: labrenne
keywords: cliente, clientes, consentimento, MCA, contrato de Microsoft Cloud, modelos de contrato de cliente
ms.localizationpriority: medium
ms.openlocfilehash: fc82d3156dd50c3ad05b141f1715634031cad202
ms.sourcegitcommit: bae29ab191c72e15259d99c40c69a9e7c3f2b502
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/06/2019
ms.locfileid: "68820521"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-cloud-agreement"></a>Confirmar a aceitação do cliente do Contrato do Microsoft Cloud

**Aplica-se a**
-  Partner Center

> [!NOTE]
> O recurso de contrato atualmente tem suporte do Partner Center na nuvem pública da Microsoft. Não é aplicável a:
> * Partner Center operado pela 21Vianet
> * Partner Center do Microsoft Cloud Germany
> * Partner Center para Microsoft Cloud for US Government

Como um parceiro, você precisa obter a aceitação do cliente do Contrato do Microsoft Cloud antes de você poder encomendar produtos e serviços Microsoft e serviços para o cliente. Para ajudar mais os parceiros a atender os requisitos de conformidade, a Microsoft solicita que os parceiros confirmem a aceitação fornecendo os detalhes a seguir em relação à pessoa que aceitou o contrato: 

-   Nome

-   Sobrenome

-   Endereço de email

-   Número de telefone (opcional)

-   Data da aceitação

Para saber mais, Confira as perguntas frequentes [sobre](https://docs.microsoft.com/partner-center/confirm-consent-faq)a confirmação de aceitação do cliente do contrato de Microsoft Cloud.

Parceiros de cobrança direto e provedores indiretos devem confirmar a aceitação do cliente do contrato de Microsoft Cloud ao transagirem por meio da API do Partner Center ou do Partner Center. A confirmação é *obrigatória*.

Se a confirmação não for fornecida por um determinado cliente:

-   Você não conseguirá criar novos pedidos para esse cliente.

-   Você não poderá alterar a contagem de estações de assinaturas baseadas em estação existentes para esse cliente.

A confirmação da aceitação do cliente pode ser feita por meio do Partner Center ou da API do Partner Center. Para fazer isso por meio da API do Partner Center, consulte os seguintes tópicos: 

-   [Obter confirmação de consentimento do cliente](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-consent)

-   [Obter metadados do contrato](https://docs.microsoft.com/partner-center/develop/get-agreement-metadata)

-   [Confirmar consentimento do cliente](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent)


Isso se aplica a ambientes de produção e área restrita.

## <a name="confirming-customer-acceptance-in-partner-center"></a>Confirmando a aceitação do cliente no Partner Center

### <a name="confirm-customer-acceptance-for-a-new-customer"></a>Confirmar a aceitação do cliente para um novo cliente

Use o procedimento a seguir para confirmar a aceitação do cliente enquanto você cria um novo locatário do cliente no Partner Center. Observe que você deve ser um Agente administrativo ou Agente de vendas para fazer isso.

1. Selecione **clientes**e, em seguida, **novo cliente** e, em seguida, selecione **informações da conta**.
2. Insira as informações sobre a **Empresa** e o **Contato principal**.

![Informações da empresa](images/mca/mca1.png)

3. Em **Contrato do Microsoft Cloud**, selecione **O cliente aceitou o último contrato do Microsoft Cloud**.
4. Em **Data de aceitação do contrato**, insira a data apropriada. Você não pode definir isso como uma data futura.
5. Insira os detalhes do usuário que forneceu a aceitação.

![Adicionar data de aceitação](images/mca/MCA3.png)

Por padrão, as informações de usuário do contato principal são exibidas. Se isso não estiver correto, selecione **Atualizar** e insira o **Nome**, **Sobrenome**, **Email** e **Número de telefone* (opcional) da pessoa que aceitou o contrato.

6. Selecione **Avançar** para continuar com as etapas restantes para criar o locatário do cliente.

### <a name="confirm-customer-acceptance-for-an-existing-customer"></a>Confirmar a aceitação do cliente para um cliente existente

Você deve ser um Agente administrativo ou Agente de vendas para fazer isso.

1. Selecione **Clientes** e então localize e selecione o cliente que você deseja ver.
2. Selecione **informações da conta**.
3. Em **Contrato do Microsoft Cloud**, selecione **Atualizar**.

![Atualização](images/mca/mca4.png)

4. Insira o **Nome**, **Sobrenome**, **Email** e **Número de telefone** (opcional) do usuário que aceitou o contrato.
5. Em **Data de aceitação do contrato**, insira a data apropriada. Você não pode definir isso como uma data futura.
6. Selecione **Salvar e continuar**.

### <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>Confirmar a aceitação do cliente ao criar o novo pedido para um cliente existente

Se tentar criar um novo pedido para um cliente existente que não confirmou antes, você receberá um aviso para concluir a confirmação. Use o procedimento a seguir para fazer isso.

1. Insira o **Nome**, **Sobrenome**, **Email** e **Número de telefone** (opcional) do usuário que aceitou o contrato.
2. Em **Data de aceitação do contrato**, insira a data apropriada. Você não pode definir isso como uma data futura.
3. Selecione **Salvar e continuar**.

### <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>Recuperar a confirmação da aceitação do cliente para um cliente existente

Você pode recuperar a confirmação da aceitação do cliente para um cliente existente que você forneceu anteriormente usando o procedimento abaixo. Você deve ser um Agente administrativo ou Agente de vendas para fazer isso.

1. Selecione **Clientes** e então localize e selecione o cliente que você deseja ver.
2. Selecione **informações da conta**.
3. Em **Contrato do Microsoft Cloud**, você verá se a confirmação foi fornecida ou não para este cliente.
