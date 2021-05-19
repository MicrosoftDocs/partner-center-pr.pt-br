---
title: Cálculo de preço unitário efetivo
ms.topic: how-to
ms.date: 04/02/2021
description: Saiba mais sobre o preço unitário efetivo e como ele é calculado. Este artigo também inclui um cálculo de exemplo.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 84beac77d41b8c11be9ac3cad87460eec9632ac4
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147115"
---
# <a name="effective-unit-price-calculation-for-azure-plan-consumption"></a>Cálculo de preço unitário efetivo para consumo do plano do Azure

**Funções apropriadas**: administrador de cobrança

## <a name="the-effective-unit-price"></a>O preço unitário efetivo

O preço unitário efetivo é calculado no nível de medidor (ao contrário do nível de recurso) e é ajustado diariamente de acordo com o uso do medidor.

Calculamos o preço unitário efetivo usando os três fatores a seguir:

- Consumo, que é monitorado diariamente durante todo o ciclo de cobrança
- Custo Faturável para o medidor
- Camadas (se aplicável)

Como monitoramos o consumo diário durante todo o ciclo de cobrança, o preço unitário efetivo ficará flutuando. O preço final de um determinado ciclo de cobrança estará disponível depois de parar o cálculo de consumo e fechar o período de cobrança. Você verá a maioria das alterações no consumo após o quarto ou quinto lugar decimal.

## <a name="find-out-whether-your-meter-uses-tiered-pricing"></a>Descubra se seu medidor usa preços em camadas

Se você não souber se o medidor usa preços em camadas, use o procedimento abaixo para descobrir. 

1. Entre no painel [Partner Center](https://partner.microsoft.com/dashboard/).
2. Selecione **vender**, selecione **preços e ofertas** e, em seguida, selecione **preços do plano do Azure**.
3. Localize seu medidor por ID e, em seguida, baixe os dados de preços. 

## <a name="sample-calculation"></a>Exemplo de cálculo

A tabela a seguir fornece um exemplo de como calculamos o preço unitário efetivo durante o período de abertura.

Na tabela, os seguintes valores se aplicam: 

- **UP** = Preço unitar do recurso/hora = 0,868

- **BCU** = unidade de consumo de cobrança para o medidor

- **BC** = Custo cobrado pelo medidor = BCU * UP * 0,85. Isso reflete um ajuste para o desconto de PEC de 15%. Em seguida, usamos o limite inferior da função para limitar o valor a dois dígitos após o ponto decimal, para cobrar a quantidade mínima. 

- **Preço unitártico** efetivo = BCU/BC

>[!NOTE]

>Observação: o medidor neste exemplo não tem camadas em preços ou outros descontos— os fatores de Preço Unitário Efetivo em percentuais de desconto e outros ajustes.


| Data | BCU (unidade de consumo de cobrança) | BC (custo cobrado) | Preço unitidade efetivo |
| ------ | ----------- | ----------- | ----------- |  
| 3 de agosto | 29 | 21.39 | 0.737586206896552 |
| 10 de agosto | 210.950039 | 155.63 | 0.737757626107858 |
| 25 de agosto | 555.950039 | 410.17 | 0.737782122900436 |

## <a name="next-steps"></a>Próximas etapas

- [Cobrança e impostos](billing.md)
