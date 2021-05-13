---
title: Funcionalidades de fatura direta restritas
ms.topic: article
ms.date: 10/09/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba mais sobre os requisitos do parceiro de cobrança direta do CSP e o que fazer para evitar que as funcionalidades se restrinam. Descubra se suas funcionalidades foram restritas.
author: billLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: b3b1f3e1593f7e35bd3b9ed6c56ea28683bff95a
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855481"
---
# <a name="restricted-direct-bill-capabilities-and-the-requirements-needed-for-csp-direct-bill-partners"></a>Recursos restritos de cobrança direta e os requisitos necessários para parceiros de cobrança direta do CSP

**Funções apropriadas:** Administrador global

## <a name="overview"></a>Visão geral

Os parceiros de cobrança direta devem atender aos [novos requisitos](direct-partner-new-requirements.md) para permanecerem no programa de parceiros de cobrança direta do CSP. Caso contrário, o acesso às funcionalidades de cobrança direta acabará sendo restrito, e eles não poderão mais executar tarefas específicas, como fazer novas compras para clientes.

> [!Note]
> Os parceiros de cobrança direta que não atenderem aos novos requisitos do programa de parceiros de cobrança direta do CSP serão informados pela Microsoft quando seus recursos de cobrança direta serão restritos. Isso se aplica a todos os parceiros de cobrança direta, quer eles tenham optado pela transição do parceiro de cobrança direta para [revendedores indiretos](transition-direct-to-indirect.md) ou não.  

## <a name="how-to-tell-if-your-direct-bill-capabilities-has-been-restricted"></a>Como saber se as funcionalidades de cobrança direta foram restritas

Para confirmar se o acesso do locatário do parceiro de cobrança direta aos recursos de cobrança direta foi restrito, siga estas etapas.

1. Entre no [Painel do Partner Center](https://partner.microsoft.com/dashboard).

2. Acesse **Configurações da conta**  ->  **Perfil Jurídico**.

3. Em **Informações do programa,** procure Provedor de Soluções na Nuvem da Microsoft **status**.

4. Se o status do programa tiver valor **restrito,** isso significa que o acesso do locatário do parceiro de cobrança direta aos recursos de cobrança direta foi restrito.

## <a name="affected-direct-bill-capabilities"></a>Recursos de cobrança direta afetados

Se suas funcionalidades de cobrança direta foram restritas, você não poderá mais fazer novas compras para seus clientes Partner Center. Essa restrição inclui:

- Assinaturas do Azure

- Assinaturas baseadas em licença

- Adicione novos complementos a assinaturas baseadas em licença existentes.

- Faça compras avursas de software e produtos de reserva (por exemplo, assinaturas de software, software perpétuo e instâncias de Máquina Virtual Reservada do Azure).

Você também não pode usar a oferta de serviços compartilhados de parceiros do [Azure](shared-services.md) no programa CSP para comprar novas assinaturas do Azure para seu próprio uso.

As assinaturas de cobrança direta existentes não são afetadas. Eles permanecem válidos e são renovados automaticamente. Você continuará sendo cobrado diretamente pela Microsoft até que eles sejam cancelados. Você ainda pode gerenciar assinaturas existentes das seguintes maneiras:

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
