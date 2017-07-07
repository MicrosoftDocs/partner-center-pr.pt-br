---
title: "Cenários comuns de cobrança | Partner Center"
description: "Este tópico explica o que você deve esperar ver em sua fatura depois de adicionar novas assinaturas, ajustar o número de licenças em uma assinatura ou cancelar uma assinatura. As assinaturas baseadas em uso e em licença serão afetadas de forma diferente."
ms.assetid: E4BBD3E7-AFE2-4998-950D-0D27D1178160
author: MaggiePucciEvans
ms.openlocfilehash: 92805672975e319b53c2cd89063442df2feb1267
ms.sourcegitcommit: e8b504fa98b3ec4c7c8fd954f63ea81299791906
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/01/2017
---
# <a name="common-billing-scenarios"></a>Cenários comuns de cobrança

**Aplicável a**

-  Partner Center
-  Partner Center do Microsoft Cloud for US Government
-  Partner Center do Microsoft Cloud Alemanha

Este tópico explica o que você deve esperar ver em sua fatura depois de adicionar novas assinaturas, ajustar o número de licenças de uma assinatura ou cancelar uma assinatura. As assinaturas baseadas em uso e em licença são afetadas de forma diferente.

## <a name="in-this-section"></a>Nesta seção


-   [Cobrança baseada em uso](#usagebased)

-   [Cobrança baseada em licença](#licensebased)

## <a href="" id="usagebased"></a>Cobrança baseada em uso


Você é cobrado somente pelos serviços usados no período de cobrança anterior. Quaisquer serviços ou aplicativos do Azure habilitados ou usados durante o período de cobrança aparecerão na fatura.

-   As taxas de serviço limitadas podem ser alteradas durante o ciclo de fatura.
    -   Aumentos de preço: é fornecido um aviso prévio de 30 dias.
    -   As reduções de preço são refletidas no dia em que elas entram em vigor.
    -   As assinaturas existentes são cobradas usando-se a taxa em vigor no início do ciclo de cobrança.
    -   As novas assinaturas (aqueles criadas durante o ciclo de cobrança) são cobradas com a taxa em vigor quando foram adicionadas.
-   Se você cancelar uma assinatura durante o primeiro ciclo de cobrança, as cobranças por uso aparecerão no arquivo de reconciliação pelo período em que a assinatura estava ativa.

## <a href="" id="licensebased"></a>Cobrança baseada em licença

Para os meses sem alterações nas assinaturas baseadas em licença, você verá um item de linha único para cada assinatura em sua fatura. Isso é para a cobrança antecipada para o próximo mês.

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
<td>Nova assinatura adicionada</td>
<td><p>O período entre a data de início da assinatura e a data da primeira cobrança é GRÁTIS.</p>
<p>Seu arquivo de reconciliação conterá um único item de linha:</p>
<ul>
<li>A cobrança antecipada para o próximo mês</li>
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
<li>Alterações na quantidade de licenças, cobradas pelo preço unitário 0. (Não há custo para alterações de licenças durante o período gratuito)</li>
<li>Cobrança antecipada pelo próximo mês, refletindo a nova quantidade.</li>
</ul></td>
<td>Uso proporcional:
<ul>
<li>De 3 de junho a 7 de junho para 10 licenças = custo ZERO</li>
<li>De 8 de junho a 11 de junho para 20 licenças = custo ZERO</li>
<li>De 12 de junho a 14 de junho para 15 licenças = custo ZERO</li>
</ul>
<p>Limite de cobrança: cobrança antecipada para o período inteiro do mês, de 15 de junho a 14 de julho para 15 licenças. Supondo que a cobrança por assinatura mensal seja 10 USD, o valor será 10 USD x 15 licenças = 150 USD.</p></td>
</tr>
<tr class="odd">
<td>Assinatura existente: aumento ou redução da quantidade de licenças</td>
<td><p>Seu arquivo de reconciliação conterá vários itens de linha:</p>
<ul>
<li>A reversão da cobrança antecipada</li>
<li>Encargos de uso proporcional</li>
<li>Cobrança antecipada do próximo mês</li>
</ul></td>
<td><p>Uso proporcional:</p>
<ul>
<li>De 15 de julho a 19 de julho para 15 licenças = 26,61 USD</li>
<li>De 20 de julho a 30 de julho para 12 licenças = 46,84 USD</li>
<li>De 31 de julho a 9 de agosto para 18 licenças = 63,87 USD</li>
<li>De 10 de agosto a 14 de agosto para 10 licenças = 17,74 USD</li>
</ul>
Reversão da cobrança antecipada para todo o período mensal de 15 de julho a 14 de agosto = -165 USD.
<p>Limite de cobrança: cobrança antecipada para o período inteiro do mês de 15 de agosto a 14 de setembro para 10 licenças = 110 USD.</p></td>
</tr>
<tr class="even">
<td>Cancelamento: sem alterações de licenças anteriores</td>
<td><p>Seu arquivo de reconciliação conterá um único item de linha:</p>
<ul>
<li>Um crédito pelos dias não utilizados, já que o período integral foi cobrado antecipadamente no extrato de cobrança anterior. Isso é calculado com base na data de término da assinatura.</li>
</ul></td>
<td>Cobrança antecipada feita anteriormente: de 15 de agosto a 14 de setembro para 10 licenças = 100 USD.
<p>Parte consumida da cobrança antecipada de 15 de agosto de 24 de agosto.</p>
<p>Crédito por dias não utilizados: de 25 de agosto a 14 de setembro para 10 licenças = -74,51 USD.</p></td>
</tr>
<tr class="odd">
<td>Cancelamento: com alterações de licenças anteriores</td>
<td><p>Seu arquivo de reconciliação conterá vários itens de linha:</p>
<ul>
<li>A reversão da cobrança antecipada</li>
<li>Encargos de uso proporcional</li>
<li>Um crédito pelos dias não utilizados</li>
</ul></td>
<td>Cobrança antecipada feita anteriormente: de 15 de agosto a 14 de setembro para 10 licenças = 100 USD.
<p>Uso proporcional:</p>
<ul>
<li>De 15 de agosto a 24 de agosto para 10 licenças</li>
<li>De 25 de agosto a 14 de setembro para 5 licenças</li>
</ul>
<p>Crédito por dias não utilizados: de 1 de setembro a 14 de setembro para 5 licenças.</p>
<p>Reversão da cobrança antecipada para todo o período mensal de 15 de agosto a 14 de setembro = -100 USD.</p></td>
</tr>
</tbody>
</table>




 



