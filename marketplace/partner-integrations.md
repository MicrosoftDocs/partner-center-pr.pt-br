---
title: Integrações de parceiros do Azure Marketplace
description: Saiba mais sobre as soluções do Azure Marketplace que se integram ao seu ambiente do Azure e obtenha links para guias de implantação de parceiros da Microsoft.
ms.service: partner-services
ms.topic: conceptual
author: JasonWHowell
ms.author: jasonh
ms.date: 11/16/2020
ms.openlocfilehash: 56e72af367cdcb264cc444446c5fcbedcd880451
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276477"
---
# <a name="azure-marketplace-partner-integrations"></a>Integrações de parceiros do Azure Marketplace

Saiba como integrar soluções de parceiros em seu ambiente do Azure. Este artigo fornece uma visão geral de cada solução e links para guias de implantação detalhados. As soluções são listadas em ordem alfabética. 

## <a name="apache-kafka-on-confluent-cloud"></a>Apache Kafka na Confluent Cloud

![Nuvem confluente.](./media/partners/confluent-cloud.png)

O Azure permite que você integre com a nuvem confluente, além de seus aplicativos de nuvem. Os clientes confluentes geralmente navegam entre a portal do Azure e a nuvem confluente. Por exemplo, quando um usuário adquire uma oferta de nuvem confluente no Azure Marketplace, espera-se que eles configurem uma conta com a nuvem confluente. Esse processo adiciona complexidade e tempo e exige que os usuários gerenciem a configuração e os recursos entre os dois portais. Para reduzir a carga de gerenciamento entre plataformas, a Microsoft, em parceria com a nuvem confluente, criou uma camada de provisionamento integrado do Azure para a nuvem confluente. A solução está disponível no Azure Marketplace e fornece uma experiência direta para usar a oferta de nuvem confluente no Azure

A solução usa um provedor de recursos habilitado no Azure para provisionar recursos de nuvem confluentes. Isso permite que os usuários acessem o streaming de eventos em tempo real por meio dos SDKs portal do Azure, CLI do Azure e Azure. A nuvem confluente possui e executa o aplicativo SaaS, que inclui ambientes, clusters, tópicos, chaves de API e conectores gerenciados.

A profunda integração com a nuvem confluente permite os seguintes recursos:

- Provisione um novo recurso de organização de nuvem confluente do portal do Azure com infraestrutura totalmente gerenciada.
- Simplifique o logon único do Azure para a nuvem confluente com o Azure Active Directory; nenhuma autenticação separada é necessária no portal de nuvem confluente.
- Obtenha cobrança unificada de encargos de consumo de nuvem entre outros por meio do faturamento de assinatura do Azure.
- Gerencie recursos de nuvem confluentes do portal do Azure e acompanhe-os na página **todos os recursos** , juntamente com os recursos do Azure.

[Guias de implantação de nuvem confluentes](https://docs.confluent.io/current/cloud/marketplace/index.html)

Para problemas relacionados ao Microsoft Fluent no Azure, vá para [https://support.confluent.io](https://support.confluent.io) . Se você for um usuário da primeira vez, redefina sua senha antes de entrar no portal de suporte do influente. Se você não tiver uma conta com o de Fluent, envie um email para [cloud-support@confluent.io](mailto:cloud-support@confluent.io) .

## <a name="datadog"></a>Datadog

![Logotipo do DataDog.](./media/partners/datadog.png)

O Datadog fornece ferramentas de observação e de segurança para que os usuários do Azure compreendam a integridade e o desempenho de seus aplicativos em ambientes híbridos e de várias nuvens. Mas a configuração das integrações necessárias geralmente requer a navegação entre a portal do Azure e o Datadog. Para simplificar a configuração e o gerenciamento de recursos nos portais, a Microsoft trabalhou com o Datadog para criar uma solução Datadog integrada no Azure. Disponível por meio do Azure Marketplace, essa solução fornece uma experiência integrada para os clientes do Azure usarem a solução de monitoramento de nuvem do Datadog.

Consulte a [documentação do Azure monitor](/azure/azure-monitor/platform/partners#datadog) para saber mais sobre essa solução e se inscrever para a visualização pública.

## <a name="next-steps"></a>Próximas etapas

- [Loja online do Azure Marketplace](https://azure.microsoft.com/marketplace/)
- [Microsoft Learn: criar uma conta do Azure](/learn/modules/create-an-azure-account/)
