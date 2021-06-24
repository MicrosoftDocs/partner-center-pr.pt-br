---
title: Comprando software e soluções do Azure Marketplace
description: Saiba mais sobre as ferramentas que simplificam e simplificam as compras e o gerenciamento de software Azure Marketplace.
ms.service: marketplace-customer
ms.topic: conceptual
author: Guyshu
ms.author: gushuchm
ms.date: 06/22/2021
ms.openlocfilehash: 0e79674825f8ab28fa4b0e68dd01c9c1b7e8c27a
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "112565178"
---
# <a name="azure-marketplace-purchasing"></a>Azure Marketplace compra

Azure Marketplace tem várias ferramentas e recursos que simplificam e simplificam o processo de compra, faturamento e gerenciamento de política de compra.

## <a name="simplified-procurement"></a>Aquisição simplificada

O Azure Marketplace ajuda você a simplificar o processo de aquisição ao disponibilizar diferentes opções de compra. Se você comprar produtos usando um cartão de crédito associado à sua conta do Azure, todas as compras serão consolidadas em uma única fatura e cobradas no cartão de crédito de sua escolha. Se você for um cliente grande, poderá comprar usando um Enterprise Agreement. Com um EA, todas as compras de software são incluídas automaticamente em sua fatura do Azure. A fatura vai conter primeiro os encargos de uso do Azure, seguidos pelos encargos do Azure Marketplace.

Ao comprar por meio Azure Marketplace, você elimina a complexidade de gerenciar faturas e relações de fornecedor individuais. Você recebe uma fatura mensal consolidada e única da Microsoft que inclui as compras Azure Marketplace e os encargos do Azure.

## <a name="permission-to-purchase"></a>Permissão para comprar

Depois de encontrar o aplicativo de software certo, concluir a compra é simples. No entanto, você precisará de permissões adequadas na assinatura do Azure. Como o Azure opera em um modelo de RBAC  [(Controle](/azure/role-based-access-control/overview) de Acesso Baseado em Função), sua conta precisa de permissões de colaborador ou proprietário da assinatura para fazer uma compra. 

Antes de concluir uma compra, certifique-se de que o usuário tem a configuração correta no locatário do Azure. Isso ajudará a evitar erros durante a compra.

Na Azure Marketplace no portal do Azure, encontre o aplicativo que deseja comprar e  selecione Criar ou **Configurar + assinar**. Você será solicitado a concluir algumas informações antes de poder usar sua nova solução.

> [!CAUTION]
> A aprovação no Marketplace Privado não indica a aquisição de uma solução.

:::image type="content" source="media/overview/offer-create-screen.png" alt-text="O botão Criar oferta.":::

:::image type="content" source="media/overview/button-set-up-and-subscribe.png" alt-text="O botão Configurar + assinar.":::

Se você quiser implantar uma solução da Azure Marketplace online, selecione Obter agora na página de descrição do produto e entre com suas credenciais de conta do Azure. 

:::image type="content" source="media/overview/sign-in-to-azure-marketplace.png" alt-text="A Azure Marketplace caixa de diálogo de login.":::

Depois de entrar, você será redirecionado para o produto no portal do Azure para concluir sua compra.

## <a name="purchase-policy-management"></a>Gerenciamento de política de compra

A Microsoft permite que você gerencie compras de usuário por meio de seu perfil de cobrança como o administrador da assinatura do Azure. Escolha entre três opções:

- **Gratuito + Pago** – permite que os usuários adquira qualquer Azure Marketplace de software.
- **Gratuito** – permite que os usuários implantem somente software gratuito do Azure Marketplace.
- **Não** – impede que os usuários implantem qualquer software Azure Marketplace.

Essas configurações se aplicam a todos os usuários com acesso à sua assinatura do Azure, o que oferece a capacidade de controlar a aquisição de TI por meio do portal do Azure.

:::image type="content" source="media/overview/billing-profile-policy-settings.png" alt-text="Controlar a aquisição de IT por meio da portal do Azure.":::

## <a name="cost-management"></a>Gerenciamento de custo

À medida que você compra produtos Azure Marketplace, você deseja obter insights que ajudam a gerenciar os custos. Gerenciamento de Custos do Azure é uma ferramenta gratuita para exibir informações sobre os produtos comprados. Você pode usar o Gerenciamento de Custos para ver detalhes de quais serviços você está gastando dinheiro ao longo do tempo e como esses custos acompanham os orçamentos que você definiu. Além de definir orçamentos, você pode agendar relatórios e analisar os custos de assinatura. Saiba mais sobre Gerenciamento de Custos do Azure concluindo o módulo Microsoft Learn em Analisar custos e criar [orçamentos com Gerenciamento de Custos do Azure](/learn/modules/analyze-costs-create-budgets-azure-cost-management/).

Veja seus encargos e suas faturas do Azure Marketplace na ferramenta de análise de custo em Gerenciamento de Custos do Azure.

:::image type="content" source="media/overview/azure-cost-management.png" alt-text="Use Gerenciamento de Custos do Azure para obter informações sobre seus produtos comprados.":::

## <a name="purchase-validation-checks"></a>Verificações de validação de compra

A compra de uma oferta por meio Azure Marketplace pode falhar por diferentes motivos. É mais provável que o uso da CLI (interface de linha de comando) para uma compra cause erros, pois você pode estar tentando comprar uma oferta que não está disponível ou visível no Azure Marketplace. A seguir estão as verificações que podem causar falha em uma compra:

1. A assinatura pertence a um Enterprise Agreement (EA) e o administrador do EA desabilitado Azure Marketplace compras.
1. O administrador do EA habilitar compras apenas para ofertas gratuitas e a oferta é uma oferta paga.
1. A oferta não foi encontrada no marketplace.
1. O ISV (Fornecedor Independente de Software) parou de vender a oferta, pelo menos em sua região.
1. A assinatura que você está usando pertence a uma conta de cobrança em uma região em que a oferta não está disponível.
1. A conta de assinatura/cobrança não está associada a um meio de pagamento válido (como um cartão de crédito válido).
1. A assinatura pertence a um Provedor de Soluções na Nuvem (CSP) e o ISV se recusou a vender por meio de um CSP.
1. O Marketplace Privado está habilitado para a assinatura e a oferta não está na lista de ofertas permitidas.
1. A oferta é Privada/Versão Prévia para clientes específicos e a assinatura não está na lista de clientes permitidos.

A compra de ofertas do marketplace poderá falhar se entrar em conflito com Azure Policy definido pelo administrador do Azure em sua organização. Por exemplo, você não poderá comprar o Microsoft.SaaS se ele não estiver na lista de permissão **da sua** organização. Para obter detalhes, consulte [Azure Policy documentação](/azure/governance/policy/)do .

## <a name="next-steps"></a>Próximas etapas

- [Cobrança e faturamento](billing-invoicing.md)