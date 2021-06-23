---
title: Funcionalidades de fatura direta restritas
ms.topic: article
ms.date: 10/09/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba mais sobre requisitos de parceiro de cobrança direto do CSP (provedor de soluções na nuvem) e o que fazer para evitar que os recursos sejam restritos. Descubra se seus recursos foram restritos.
author: billLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e5bc33101809a805ba591be5a9b51d8dfff2397b
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551411"
---
# <a name="restricted-direct-bill-capabilities-and-the-requirements-needed-for-csp-direct-bill-partners"></a>Recursos de cobrança direta restritos e os requisitos necessários para parceiros de cobrança direto do CSP

**Funções apropriadas**: administrador global

## <a name="overview"></a>Visão geral

Os parceiros de cobrança direto devem atender aos novos [requisitos](direct-partner-new-requirements.md) para permanecerem no programa de parceiro de cobrança direto do CSP (provedor de soluções na nuvem). Caso contrário, o acesso às funcionalidades de cobrança direta acabará sendo restrito, e eles não poderão mais executar tarefas específicas, como fazer novas compras para clientes.

> [!Note]
> Os parceiros de cobrança direto que não atendem aos novos requisitos para o programa de parceiro de cobrança direto do CSP serão informados pela Microsoft quando seus recursos de fatura direta serão restritos. Isso se aplica a todos os parceiros de cobrança diretos, se eles optaram por fazer [a transição de um parceiro de cobrança direto para revendedores indiretos](transition-direct-to-indirect.md) ou não.  

## <a name="how-to-tell-if-your-direct-bill-capabilities-has-been-restricted"></a>Como saber se seus recursos de fatura direta foram restritos

Para confirmar se o acesso do locatário do parceiro de cobrança direto para direcionar recursos de cobrança foi restringido, siga estas etapas.

1. Entre no [Painel do Partner Center](https://partner.microsoft.com/dashboard).

2. Vá para **configurações de conta**  >  **perfil legal**.

3. Em **informações do programa**, procure **Microsoft Cloud status do provedor de solução**.

4. Se o status do programa tiver um valor **restrito**, isso significa que o acesso do locatário do parceiro de cobrança direto aos recursos de cobrança direto foi restringido.

## <a name="affected-direct-bill-capabilities"></a>Recursos de fatura direta afetados

Se seus recursos de fatura direta foram restritos, você não poderá mais fazer novas compras para seus clientes no Partner Center. Essa restrição inclui:

- Assinaturas do Azure

- Assinaturas baseadas em licença

- Adicione novos Complementos a assinaturas baseadas em licença existentes.

- Faça compras unidirecionais de produtos de software e Reserva (por exemplo, assinaturas de software, software permanente e instâncias de máquinas virtuais reservadas do Azure).

Você também não pode usar a [oferta de serviços compartilhados de parceiro do Azure](shared-services.md) no programa CSP para comprar novas assinaturas do Azure para seu próprio uso.

As assinaturas de fatura direta existentes não são afetadas. Eles permanecem válidos e são renovados em autorenovação. Você continuará sendo cobrado diretamente pela Microsoft até que eles sejam cancelados. Você ainda pode gerenciar assinaturas existentes das seguintes maneiras:

- Suspender assinaturas existentes

- Ajustar a contagem de licenças das assinaturas baseadas em licença existentes

- Ajuste a contagem de licenças de Complementos existentes para uma assinatura. 

    >[!Note]
    >Você não pode adicionar novos Complementos às assinaturas existentes, pois elas são tratadas como uma nova compra.

- Implante novos recursos do Azure e gerencie recursos existentes do Azure em assinaturas do Azure existentes. Isso inclui recursos, que estão disponíveis por meio das assinaturas do Azure Marketplace e do Visual Studio.

Além das novas compras, você não pode acessar os seguintes recursos de fatura direta no Partner Center:

- Você não pode criar novos locatários do cliente. A opção **criar cliente** na página **clientes** no Partner Center não estará disponível.

- Você não pode gerar um convite para o cliente solicitando a relação de revendedor direto. A opção **solicitar um relacionamento do revendedor** na página **clientes** no Partner Center não estará disponível.

    >[!NOTE]
    >Como parte da transição do parceiro de cobrança direto para o revendedor indireto, se você já registrou seu locatário de parceiro de cobrança direto como revendedor indireto, você pode gerar um convite para o cliente solicitando a relação de revendedor indireto.

- Você não pode criar um novo locatário de área restrita. Cada locatário de parceiro de cobrança direto pode criar um locatário de área restrita para integração direta da API de cobrança. Se você não tiver criado um anteriormente, não será permitido fazer isso depois que o recurso de parceiro de cobrança direto tiver sido restrito.  

## <a name="next-steps"></a>Próximas etapas

- [Mais informações sobre como se tornar um revendedor indireto](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf)

- [Novos requisitos do parceiro direto do CSP](direct-partner-new-requirements.md)
