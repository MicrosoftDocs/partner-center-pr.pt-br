---
title: Recursos de cobrança direta restrita | Centro de parceiros
ms.topic: article
ms.date: 01/24/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Os parceiros de cobrança direto que não atendem ao novo requisito terão recursos diretos de cobrança restritos
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
keywords: fatura direta, restringir
ms.openlocfilehash: 7f2dae72edff59b3e6d84c74f93bae437be4ce30
ms.sourcegitcommit: d11c52e1386c181e177df72d6c7244508f1d6c0e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/29/2020
ms.locfileid: "76860497"
---
# <a name="restricted-direct-bill-capabilities"></a>Recursos de cobrança direta restrita  

**Visão geral**

Os parceiros de cobrança direto devem atender aos novos [requisitos](direct-partner-new-requirements.md) para permanecerem no programa de parceiro de cobrança direto do CSP. Caso contrário, o acesso aos recursos de cobrança direto eventualmente será restrito e poderá mais executar tarefas específicas, como fazer novas compras para seus clientes. 

>[!Note]
>Os parceiros de cobrança direto que não atendem aos novos requisitos para o programa de parceiro de cobrança direto do CSP serão informados pela Microsoft quando seus recursos de fatura direta serão restritos. Isso se aplica a todos os parceiros de cobrança diretos, se eles optaram por fazer [a transição de um parceiro de cobrança direto para revendedores indiretos](transition-direct-to-indirect.md) ou não.  
 
## <a name="how-to-tell-if-your-direct-bill-capabilities-has-been-restricted"></a>Como saber se seus recursos de fatura direta foram restritos 

Para confirmar se o acesso do locatário do parceiro de cobrança direto aos recursos de cobrança direto foi restrito: 

1. Faça logon no [painel do Partner Center](https://partner.microsoft.com/dashboard). 

2. Vá para **configurações de parceiro** -> **perfil de parceiro**. 

3. Em **informações do programa**, procure **Microsoft Cloud status do provedor de solução**. 

4. Se o status do programa tiver um valor **restrito**, isso significa que o acesso do locatário do parceiro de cobrança direto aos recursos de cobrança direto foi restringido. 
 
## <a name="affected-direct-bill-capabilities"></a>Recursos de fatura direta afetados 

Se seus recursos de fatura direta foram restritos, você não poderá mais fazer novas compras para seus clientes no Partner Center. Isso inclui: 

- Assinaturas do Azure 
- Assinaturas baseadas em assento 
- Adicione novos Complementos a assinaturas baseadas em assento existentes. 
- Faça compras unidirecionais de produtos de software e Reserva (por exemplo, assinaturas de software, software permanente e instâncias de máquinas virtuais reservadas do Azure) 

Você também não pode adquirir novas assinaturas do Azure para seu próprio uso usando a [oferta de serviços compartilhados de parceiro do Azure](shared-services.md) no programa CSP. 

As assinaturas de fatura direta existentes não são afetadas. Eles permanecem válidos e são renovados automaticamente. Você continuará sendo cobrado diretamente pela Microsoft até que eles sejam cancelados. Você ainda pode gerenciar assinaturas existentes das seguintes maneiras: 

- Suspender assinaturas existentes 
- Ajustar a contagem de estações de assinaturas baseadas em assentos existentes 
- Ajustar a contagem de estações de Complementos existentes para uma assinatura. Observação: você não pode adicionar novos Complementos a assinaturas existentes, pois elas são tratadas como uma nova compra. 
- Implante novos recursos do Azure e gerencie recursos existentes do Azure em assinaturas do Azure existentes. Isso inclui recursos que estão disponíveis por meio das assinaturas do Azure Marketplace e do Visual Studio. 

Além das novas compras, você não pode acessar os seguintes recursos de fatura direta no Partner Center: 

- Você não pode criar novos locatários do cliente. A opção **criar cliente** na página **clientes** no Partner Center não estará disponível. 
- Você não pode gerar um convite para o cliente solicitando a relação de revendedor direto. A opção **solicitar um relacionamento do revendedor** na página **clientes** no Partner Center não estará disponível. 

    >[!Note]
    >Como parte da transição do parceiro de cobrança direto para o revendedor indireto, se você já registrou seu locatário de parceiro de cobrança direto como revendedor indireto, você pode gerar um convite para o cliente solicitando a relação de revendedor indireto. 
 
- Você não pode criar um novo locatário de área restrita. Cada locatário de parceiro de cobrança direto pode criar um locatário de área restrita com a finalidade de integração direta da API de cobrança. Se você ainda não tiver criado um, não terá permissão para fazê-lo depois que o recurso do parceiro de cobrança direto tiver sido restrito.  

## <a name="see-also"></a>Veja também 
- [Informações adicionais sobre como se tornar um revendedor indireto](https://assetsprod.microsoft.com/csp-directbill-to-indirect-transition.pdf) 
- [Novos requisitos do parceiro direto do CSP](direct-partner-new-requirements.md)