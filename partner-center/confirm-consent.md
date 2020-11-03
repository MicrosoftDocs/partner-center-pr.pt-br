---
title: Confirmar a aceitação do cliente do Contrato de Cliente da Microsoft
description: Aprenda a confirmar a aceitação do cliente do Contrato de Cliente da Microsoft. Isso pode ser necessário para solicitar serviços e produtos da Microsoft para clientes.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 06/30/2020
ms.openlocfilehash: aacca72e9af45b2777364734c2b07dbe8101989d
ms.sourcegitcommit: 22af0997d52a87417b62f44fb0a7d711bec77b35
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/19/2020
ms.locfileid: "92333908"
---
# <a name="updated-method-to-confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a>Atualização do método para confirmar a aceitação do cliente do Contrato de Cliente da Microsoft

**Aplica-se a**

-  Partner Center

**Funções apropriadas**

- Agente administrativo
- Agente de vendas

> [!NOTE]
> No momento, há suporte para o recurso Contrato no Partner Center somente na nuvem pública da Microsoft. Não é aplicável a:
> * Partner Center operado pela 21Vianet
> * Partner Center do Microsoft Cloud Germany
> * Partner Center do Microsoft Cloud for US Government

>[!NOTE]
>A partir de 31 de janeiro de 2020, todos os clientes, existentes e novos, devem assinar o novo Contrato de Cliente da Microsoft. Para saber mais, leia [Confirmar a aceitação pelo cliente do Contrato de Cliente da Microsoft](confirm-customer-agreement.md).

Como parceiro, você precisa obter a aceitação pelo cliente do Contrato de Cliente da Microsoft antes de poder solicitar produtos e serviços da Microsoft para esse cliente. Para ajudar mais os parceiros a atender os requisitos de conformidade, a Microsoft solicita que os parceiros confirmem a aceitação fornecendo os detalhes a seguir em relação à pessoa que aceitou o contrato:

- Nome

- Sobrenome

- Endereço de email

- Número de telefone (opcional)

- Data da aceitação

Parceiros de cobrança direta e Provedores Indiretos devem confirmar a aceitação pelo cliente do Contrato de Cliente da Microsoft ao fazer transações por meio do Partner Center ou da API do Partner Center. A confirmação é *obrigatória* .

Se a confirmação não for fornecida por um determinado cliente:

- Você não conseguirá criar pedidos para esse cliente.

- Você não poderá alterar a contagem de licenças das assinaturas baseadas em licenças existentes para esse cliente.

A confirmação da aceitação pelo cliente poderá ser feita por meio do Partner Center ou da API do Partner Center. Para fazer isso por meio da API do Partner Center, confira os seguintes tópicos:

- [Obter confirmação de consentimento do cliente](/partner-center/develop/get-confirmation-of-customer-consent)

- [Obter metadados do contrato](/partner-center/develop/get-agreement-metadata)

- [Confirmar o consentimento do cliente](/partner-center/develop/confirm-customer-consent)

Isso se aplica a ambientes de produção e área restrita.

## <a name="confirm-customer-acceptance-for-a-new-customer"></a>Confirmar a aceitação do cliente para um novo cliente

Use o procedimento a seguir para confirmar a aceitação do cliente enquanto você cria um locatário do cliente no Partner Center. Você deve ser um Agente administrativo ou Agente de vendas para fazer isso.

1. Selecione **Clientes** e, em seguida, **Novo cliente** e, em seguida, selecione **Informações da conta** .

2. Insira as informações sobre a **Empresa** e o **Contato principal** .

   :::image type="content" source="images/mca/mca1.png" alt-text="Informações da empresa":::

3. Em **contrato de cliente da Microsoft** , selecione **O cliente aceitou o contrato de cliente da Microsoft mais recente** .

4. Em **Data de aceitação do contrato** , insira a data apropriada. Você não pode definir isso como uma data futura.

5. Insira os detalhes do usuário que forneceu a aceitação.

   :::image type="content" source="images/mca/MCA3.png" alt-text="Informações da empresa":::

   Por padrão, as informações de usuário do contato principal são exibidas. Se isso não estiver correto, selecione **Atualizar** e insira o **Nome** , **Sobrenome** , **Endereço de email** e * *Número de telefone* (opcional) da pessoa que aceitou o contrato.

6. Selecione **Avançar** para continuar com as etapas restantes para criar o locatário do cliente.

## <a name="confirm-customer-acceptance-for-an-existing-customer"></a>Confirmar a aceitação do cliente para um cliente existente

Você deve ser um Agente administrativo ou Agente de vendas para fazer isso.

1. Selecione **Clientes** e então localize e selecione o cliente que você deseja ver.

2. Selecione **Informações da Conta** .

3. Em **Contrato de cliente da Microsoft** , selecione **Atualizar** .

   :::image type="content" source="images/mca/mca4.png" alt-text="Informações da empresa":::

4. Insira o **Nome** , **Sobrenome** , **Endereço de email** e **Número de telefone** (opcional) do usuário que aceitou o contrato.

5. Em **Data de aceitação do contrato** , insira a data apropriada. Você não pode definir isso como uma data futura.

6. Selecione **Salvar e continuar** .

## <a name="confirm-customer-acceptance-while-creating-new-order-for-an-existing-customer"></a>Confirmar a aceitação do cliente ao criar o pedido para um cliente existente

Se você tentar criar um pedido para um cliente existente que não fez a confirmação antes, receberá um aviso para concluir a confirmação. Use o procedimento a seguir para fazer isso.

1. Insira o **Nome** , **Sobrenome** , **Endereço de email** e **Número de telefone** (opcional) do usuário que aceitou o contrato.

2. Em **Data de aceitação do contrato** , insira a data apropriada. Você não pode definir isso como uma data futura.

3. Selecione **Salvar e continuar** .

## <a name="retrieve-confirmation-of-customer-acceptance-for-an-existing-customer"></a>Recuperar a confirmação da aceitação do cliente para um cliente existente

Você pode recuperar a confirmação da aceitação do cliente para um cliente existente que você forneceu anteriormente usando o procedimento abaixo. Você deve ser um Agente administrativo ou Agente de vendas para fazer isso.

1. Selecione **Clientes** e então localize e selecione o cliente que você deseja ver.

2. Selecione **Informações da Conta** .

3. Em **Contrato de cliente da Microsoft** , você verá se a confirmação foi fornecida ou não para este cliente.

## <a name="next-steps"></a>Próximas etapas

- [Confirmar a aceitação do Contrato de Cliente da Microsoft pelo cliente no programa de parceiro CSP](confirm-customer-agreement.md)

- [Atestar a aceitação do Contrato de Cliente da Microsoft em nome do seu cliente](attest-acceptance-customer-agreement.md)