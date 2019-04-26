---
title: Cenários comuns de cobrança (operado pela 21Vianet do Partner Center)
ms.topic: article
ms.date: 10/29/2018
description: Este tópico explica o que você deve esperar ver em sua fatura depois de adicionar novas assinaturas, ajustar o número de estações em uma assinatura ou cancelar uma assinatura.
author: MaggiePucciEvans
ms.author: evansma
ms.openlocfilehash: 0da5bbf6a5c3259589973e25f592457da7e3e42e
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "62132336"
---
# <a name="common-billing-scenarios"></a>Cenários comuns de cobrança

**Aplica-se a**

-   Partner Center operado pela 21Vianet


Este tópico explica o que você deve esperar ver em sua fatura depois de adicionar novas assinaturas, ajustar o número de estações em uma assinatura ou cancelar uma assinatura. 


## <a name="licence-based-billing"></a>Cobrança baseada em licença


Meses sem alterações para assinaturas de licença, você verá um único item de linha para cada assinatura no seu arquivo de reconciliação e a fatura para o encargo de avanço para o próximo mês.

<table>
<colgroup>
<col width="33%" />
<col width="33%" />
<col width="33%" />
</colgroup>
<tbody>
<tr class="odd">
<td>Cenário</td>
<td>Descrição</td>
<td>Exemplo</td>
</tr>
<tr class="even">
<td>Nova assinatura</td>
<td><p>O período entre a data de início da assinatura e a data da primeira cobrança é GRÁTIS.</p>
<p>Seu arquivo de reconciliação conterá um único item de linha:</p>
<ul>
<li>cobrança antecipada do próximo mês</li>
</ul></td>
<td></td>
</tr>
<tr class="odd">
<td>Nova assinatura: cancelada antes do fechamento da fatura</td>
<td>Os encargos não serão aplicados à conta. A assinatura não aparecerá no arquivo de reconciliação. Isso é útil se você quiser fazer um teste sem precisar pagar os encargos da assinatura.</td>
<td></td>
</tr>
<tr class="even">
<td>Nova assinatura: com ajustes de quantidade de licenças durante o período gratuito</td>
<td><p>Seu arquivo de reconciliação conterá vários itens de linha:</p>
<ul>
<li>alterações na quantidade de licenças, cobradas no preço unitário 0. (Não há custo para alterações de assentos durante o período gratuito)</li>
<li>cobrança antecipada pelo próximo mês, refletindo a nova quantidade.</li>
</ul></td>
<td>Uso proporcional:
<ul>
<li>De 3 de junho a 7 de junho para 10 assentos = custo ZERO</li>
<li>De 8 de junho a 11 de junho para 20 assentos = custo ZERO</li>
<li>De 12 de junho a 14 de junho para 15 assentos = custo ZERO</li>
</ul>
<p>Recortar de cobrança: Avançar o custo para o período do mês inteiro de 15 de junho para 14 de julho para estações de 15. Supondo que a cobrança por assinatura mensal seja US$ 10, o valor será US$ 10 x 15 assentos = US$ 150.</p></td>
</tr>
<tr class="odd">
<td>Assinatura existente: Aumentar ou diminuir a quantidade de licença</td>
<td><p>Seu arquivo de reconciliação conterá vários itens de linha:</p>
<ul>
<li>a reversão da cobrança antecipada</li>
<li>encargos de uso proporcional</li>
<li>cobrança antecipada do próximo mês</li>
</ul></td>
<td><p>Uso proporcional:</p>
<ul>
<li>De 15 de julho a 19 de julho para 15 assentos = US$ 26,61</li>
<li>De 20 de julho a 30 de julho para 12 assentos = US$ 46,84</li>
<li>De 31 de julho a 9 de agosto para 18 assentos = US$ 63,87</li>
<li>De 10 de agosto a 14 de agosto para 10 assentos = US$ 17,74</li>
</ul>
Reversão da cobrança antecipada para todo o período mensal de 15 de julho a 14 de agosto = US$ -165.
<p>Recortar de cobrança: Avançar o custo para o período do mês inteiro de 15 de agosto para 14 de setembro para 10 estações = USD 110.</p></td>
</tr>
<tr class="even">
<td>Cancelamento: sem alterações de assentos anteriores</td>
<td><p>Seu arquivo de reconciliação conterá um único item de linha:</p>
<ul>
<li>Um crédito pelos dias não utilizados, já que o período integral foi cobrado antecipadamente no extrato de cobrança anterior. Isso é calculado com base na data de término da assinatura.</li>
</ul></td>
<td>Anteriormente cobrados encargos de avanço: 15 de agosto de 14 de setembro para 10 se ajuste = 100 USD.
<p>Parte consumida da cobrança antecipada de 15 de agosto de 24 de agosto.</p>
<p>Crédito por dias não utilizados: 25 de agosto a 14 de setembro para 10 se ajuste =-74.51.</p></td>
</tr>
<tr class="odd">
<td>Cancelamento: com as alterações de assentos anteriores</td>
<td><p>Seu arquivo de reconciliação conterá vários itens de linha:</p>
<ul>
<li>a reversão da cobrança antecipada</li>
<li>encargos de uso proporcional</li>
<li>um crédito pelos dias não utilizados</li>
</ul></td>
<td>Anteriormente cobrados encargos de avanço: 15 de agosto de 14 de setembro para 10 se ajuste = 100 USD.
<p>Uso proporcional:</p>
<ul>
<li>De 15 de agosto a 24 de agosto para 10 assentos</li>
<li>De 25 de agosto a 14 de setembro para 5 assentos</li>
</ul>
<p>Crédito por dias não utilizados: 1º de setembro para 14 de setembro de 5 estações.</p>
<p>Reversão da cobrança antecipada para todo o período mensal de 15 de agosto a 14 de setembro = US$ -100.</p></td>
</tr>
</tbody>
</table>
