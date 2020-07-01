---
title: Problemas de associação do cliente
description: Saiba como solucionar problemas que surgem ao trabalhar com associações de cliente reivindicadas de CPOR (parceiro de registro).
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.date: 06/29/2020
ms.openlocfilehash: e5ad52e128aba9884fafea3900a3c03d31d4868f
ms.sourcegitcommit: bea864212edc90c5f851566505deef6623f79723
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2020
ms.locfileid: "85719292"
---
# <a name="customer-association-issues"></a>Problemas de associação do cliente

Aplica-se a:

- Partner Center

O conteúdo abaixo ajudará você a resolver problemas que podem surgir quando você trabalha com associações de clientes.

Funções apropriadas:

- Administrador de cobrança
- Administrador global
- Administrador de incentivos

## <a name="domain-tenant-mismatch"></a>Incompatibilidade de locatário de domínio

No fluxo de declarações de associação CPOR (parceiro de registro) reivindicado, você será solicitado a fornecer a ID de locatário do cliente e o subdomínio. Se você receber um erro informando que eles não correspondem, entre em contato com o cliente para garantir que você tem os detalhes corretos.

## <a name="subscription-errors-in-the-cpor-association-claim-flow"></a>Erros de assinatura no fluxo de declaração de associação CPOR

No fluxo de declaração de associação do CPOR, você pode ser solicitado a fornecer uma assinatura para um produto que você está tentando reivindicar por meio de Business Applications (Dynamics 365). Solicitamos a assinatura porque estamos verificando dinamicamente se o produto e a assinatura pertencem ao locatário que está sendo reivindicado. Também estamos verificando se a assinatura está em status de cortesia ativo/no estado de carência.

Se você receber o erro, pode ser por vários motivos:

- O produto selecionado não existe no locatário do cliente
- A assinatura fornecida não é para o Dynamics
- A assinatura fornecida não é para o CSP
- O cliente ainda não ativou/provisionou os produtos para essa assinatura
- Esta assinatura já foi declarada
- O identificador fornecido não é uma ID de assinatura

Se você tiver alguma dúvida sobre a precisão de sua assinatura, trabalhe com seu cliente para garantir que a assinatura esteja correta e que você esteja usando a ID de locatário correta.

Se essa rota não resolveu seu problema, contate o [suporte](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="when-subscriptions-will-be-available-to-claim"></a>Quando as assinaturas estarão disponíveis para a declaração

Ao reivindicar uma assinatura, você receberá um erro se a assinatura ainda não tiver sido provisionada. Há várias etapas que o cliente precisa tomar para que a assinatura fique disponível para que a plataforma CPOR a pegue e disponibilize-a para reivindicação. Se você estiver recebendo um erro ao tentar reivindicar uma assinatura, entre em contato com seu cliente para garantir que ele foi provisionado e a assinatura que você está reivindicando está correta. Se você já executou essa rota, contate o [suporte](https://partner.microsoft.com/dashboard/support/incentives/servicerequests?category=incentives).

## <a name="which-activity-do-i-choose"></a>Qual atividade eu escolho?

A plataforma de reivindicação CPOR permite declarações de associação CPOR relacionadas a áreas de solução Business Applications e Microsoft 365. As atividades aplicáveis a cada área de solução estão abaixo. Selecione a atividade correta com base nas descrições para evitar ter que recuperar no futuro. Reivindicar com uma atividade incorreta pode resultar em ganhos de qualificação e de incentivos perdidos.


| Área da solução | Atividade | Aplicável para |
| ------ | ----------- | ----------- |
| Aplicativos de negócios      | Pré-vendas   | Selecione se você influenciar a compra de um produto qualificado e quiser se candidatar a incentivos de pré-venda. Essa opção só será aplicável se o cliente comprou esses produtos por meio do contrato de licenciamento por volume ou diretamente da Web. |
|    |  Uso  | Selecione se você impulsionar sua adoção e uso de uma carga de trabalho qualificada e quiser se candidatar a incentivos de uso. Essa opção só será aplicável se o cliente comprou esses produtos por meio do contrato de licenciamento por volume ou diretamente da Web. |
|    | Associação de receita   | Selecione se você influenciar a seleção de um produto qualificado como um influenciador de negócios. Essa opção é apenas para associação de receita, não para pagamentos de incentivo. Essa opção só será aplicável se o cliente comprou esses produtos por meio do contrato de licenciamento por volume ou diretamente da Web.   |
| Microsoft 365   | Uso   | Selecione se você impulsionar sua adoção e uso de uma carga de trabalho qualificada e quiser se candidatar a incentivos de uso. |

## <a name="which-mpn-do-i-choose"></a>Qual MPN escolho?

No fluxo de declaração de associação do CPOR, você será solicitado a escolher um MPN da empresa que deve ser associado ao trabalho que você está reivindicando no cliente final. Sua empresa pode ter muitos MPNs, alguns dos quais podem ser registrados em programas de incentivo e outros associados a um tipo de parceiro, como o FRP FastTrack. O fluxo de declaração de associação do CPOR identificará qual MPNs será registrado em um programa de incentivo, mas não dirá se ele é um tipo de parceiro específico MPN. É importante selecionar o MPN correto para evitar ter que recuperar no futuro. Reivindicar com um MPN incorreto pode resultar em ganhos de qualificação e de incentivos perdidos.

Se você não souber qual MPN usar, entre em contato com seu administrador global.

Se o MPN que você pretende usar não estiver registrado, você poderá gerenciá-lo na [guia Visão geral de incentivos](https://partner.microsoft.com/dashboard/incentives/enrollment/summary).

## <a name="choosing-a-product-vs-entering-a-subscription"></a>Escolhendo um produto vs inserindo uma assinatura

Quando um produto do Dynamics é declarado e aprovado, o parceiro pode exibir a ID da assinatura na própria declaração de associação CPOR. Quando essa assinatura é reivindicada, ela está em status ativo ou de cortesia, mas pode haver um horário em que a assinatura termina, e as novas assinaturas precisarão ser reivindicadas em uma declaração de associação CPOR separada.

## <a name="competing-claims"></a>Declarações concorrentes

Se você estiver criando uma declaração de associação CPOR para um cliente e seus produtos que já estão associados a outro parceiro, sua declaração passará pela arbitragem:

1. Depois de criar uma nova associação de cliente, a Microsoft verificará os detalhes da associação e da prova de execução fornecida para garantir sua exatidão.

2. Se você e outro parceiro alegarem o mesmo cliente e produto/carga de trabalho, a Microsoft examinará a documentação de prova de execução de cada parceiro para determinar qual parceiro aprovar.

3. Informações adicionais podem ser solicitadas de ambos os parceiros, o que pode causar atrasos no processamento de sua solicitação de associação.

4. Sua declaração de associação do CPOR ainda será revisada dentro de cinco dias úteis, embora seu status possa ficar _em análise_ por um período de tempo maior. Esse cenário pode acontecer quando a Microsoft trabalha com o parceiro que atualmente possui o produto/carga de trabalho. Você será notificado dentro da seção de comentários de sua declaração, se esse for o caso. 

>[!IMPORTANT]
>Se exigirmos informações adicionais para verificar seu CPOR Association PoE, entraremos em contato com você por meio da seção comentários de declaração de associação do CPOR.
