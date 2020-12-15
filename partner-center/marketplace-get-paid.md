---
title: Sendo pago no Partner Center
description: Saiba mais sobre como receber pagamentos de ganhos como um parceiro da Microsoft, como por meio de ofertas do Marketplace comercial, programas de incentivo e o programa do provedor de soluções na nuvem. Inclui política de pagamento, status de retenção de pagamento e instruções de pagamento.
ms.service: marketplace
ms.topic: conceptual
ms.date: 11/25/2020
author: eunjkim520
ms.author: eunjkim
ms.openlocfilehash: fc1eea0d8a90bb2b5e11dad24a71c9c34fd1a4a0
ms.sourcegitcommit: 4e36d1a4ca2f074b55f9b9a08e300734eae1f06d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/15/2020
ms.locfileid: "97492442"
---
# <a name="getting-paid-in-partner-center"></a>Sendo pago no Partner Center

**Funções apropriadas:**

- Administrador de conta
- Administrador global

Este artigo tem informações importantes sobre o recebimento de pagamentos para suas ofertas, Complementos e anúncios de publicidade. Ele resume a política de pagamento, as etapas necessárias antes de serem pagas e a visão geral da instrução de pagamento.

## <a name="payout-policies-and-agreements"></a>Contratos e políticas de pagamento

A obtenção de pagamento exige que você respeite os contratos e a política de pagamento.

- [Microsoft Azure Marketplace contrato de fornecedor](https://go.microsoft.com/fwlink/p/?LinkID=699560): antes de ser pago, você deve aceitar este contrato de editor. Este contrato explica a relação entre você e a Microsoft como pertence às ofertas do vendedor no mercado comercial, incluindo a taxa de armazenamento que a Microsoft cobra por cada venda feita.
- A [política](payout-policy-details.md) de pagamento mostra as políticas de pagamento de pagamentos, incluindo o plano de pagamento e os métodos de pagamento. A política também explica o processo para não pagamentos de clientes.
- Os [detalhes do imposto](tax-details-marketplace.md) explicam a consideração do imposto sobre a seleção de preço e a responsabilidade do imposto no contrato do Microsoft [Publisher](https://go.microsoft.com/fwlink/p/?LinkID=699560).
- As **tarifas de armazenamento** são oficialmente definidas no contrato do editor. A taxa de armazenamento é aplicada a todas as vendas de ofertas coletadas pelo Marketplace comercial, incluindo Complementos.
- Os **pagamentos** são feitos mensalmente (desde que o limite de pagamento tenha sido atingido). Normalmente, enviamos qualquer pagamento devido em um determinado mês pelo 15º dia desse mês. Os pagamentos geralmente levam de 3 a 10 dias úteis adicionais para alcançar sua conta de pagamento. Para obter detalhes, confira [Limites, formas e períodos de pagamento](payment-thresholds-methods-timeframes.md).

## <a name="prerequisite-steps-before-getting-paid"></a>Etapas de pré-requisito antes de serem pagas

Antes de ser pago pela primeira vez, você deve configurar sua conta de pagamento e concluir o banco e os formulários de impostos necessários. Em formulários bancários e de impostos, você fornecerá seus métodos de pagamento preferenciais e os formulários de imposto para retenção de imposto. Os formulários bancários e de impostos são necessários antes de poder pagá-lo. Para obter detalhes, consulte [configurar sua conta de pagamento e formulários de impostos](set-up-your-payout-account.md).

### <a name="payout-hold-status"></a>Status de retenção de pagamento

Por padrão, enviamos os pagamentos mensalmente, conforme descrito acima. No entanto, você tem a opção de colocar seus pagamentos em um programa em espera, e a Microsoft não liberará seu pagamento para sua conta. Se você optar por colocar seus pagamentos em espera, continuaremos registrando quaisquer ganhos na página de **pagamentos** . No entanto, não enviaremos nenhum pagamento à sua conta até que você remova a espera.

Para posicionar seus pagamentos em espera, selecione o ícone de engrenagem **configurações** na parte superior direita e, em seguida, **configurações da conta**. Selecione **pagamento e imposto** no menu à esquerda e, na seção **atribuição de perfil de pagamento e imposto** , localize o programa para o qual deseja que os pagamentos sejam mantidos. Marque a caixa de seleção **manter meu pagamento** para manter os pagamentos deste programa. Você pode alterar o status de espera de pagamento a qualquer momento, mas sua decisão afetará o pagamento mensal seguinte. Por exemplo, se você quiser colocar o pagamento de abril em espera, defina o status de pagamento em espera para **Ativado** antes do final de março.

Depois de definir seu status de espera de pagamento como **ativado**, todos os pagamentos desse programa ficarão em espera até que você desmarque a caixa de seleção para **desativado**. Ao fazer isso, você será incluído durante o próximo ciclo de pagamento mensal (desde que o limite de pagamentos tenha sido atingido). Se você tiver seus pagamentos em espera, mas quiser ter um pagamento gerado em junho, desmarque a caixa de seleção para **desativado** antes do final de maio.

>[!Note]
> O status de retenção de pagamento se aplica a cada programa individualmente (Microsoft Store, publicidade, Azure Marketplace e assim por diante). Se você quiser manter pagamentos para todos os seus programas, mantenha o pagamento em cada programa individualmente.

## <a name="payout-statements"></a>Demonstrativos de pagamento

A instrução pagamento mostra os ganhos das vendas de suas ofertas e Complementos no histórico de transações. Você também pode exibir detalhes de pagamento e baixar relatórios no formato TSV ou CSV. Consulte as [instruções de pagamento](payout-statement.md) para saber mais sobre como acessar a instrução de pagamento e os detalhes do histórico de transações e dos relatórios de pagamento. Além disso, você pode usar a [API de pagamentos do parceiro](https://apidocs.microsoft.com/services/partnerpayouts) para efetuar pull de forma sistemática dos relatórios de pagamento.

## <a name="next-steps"></a>Próximas etapas

- [API de pagamentos de parceiros](https://apidocs.microsoft.com/services/partnerpayouts)
- [Perguntas frequentes sobre pagamentos](payout-faq.md)
