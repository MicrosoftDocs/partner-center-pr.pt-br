---
title: "Cenários comuns de cobrança | Partner Center"
description: "Este tópico explica o que você deve esperar ver em sua fatura depois de adicionar novas assinaturas, ajustar o número de estações em uma assinatura ou cancelar uma assinatura. As assinaturas baseadas em uso e em licença serão afetadas de forma diferente."
ms.assetid: E4BBD3E7-AFE2-4998-950D-0D27D1178160
author: MaggiePucciEvans
ms.openlocfilehash: 5ac69f33ca78be1eca2af439a48d6d0904a4cfc5
ms.sourcegitcommit: b7bc0c63a98c458fb19e16c73c47ad80e2ce9429
ms.translationtype: HT
ms.contentlocale: pt-BR
---
# <a name="common-billing-scenarios"></a>Cenários comuns de cobrança

**Aplicável a**

-  Partner Center
-  Partner Center do Microsoft Cloud Alemanha

Este tópico explica o que você deve esperar ver em sua fatura depois de adicionar novas assinaturas, ajustar o número de estações em uma assinatura ou cancelar uma assinatura. As assinaturas baseadas em uso e em licença serão afetadas de forma diferente.

## <a name="in-this-section"></a>Nesta seção


-   [Cobrança baseada em uso](#usagebased)

-   [Cobrança baseada em licença](#licensebased)

## <a href="" id="usagebased"></a>Cobrança baseada em uso


Você é cobrado somente pelos serviços usados no período de cobrança anterior. Quaisquer serviços ou aplicativos do Azure habilitados ou usados durante o período de cobrança aparecerão na fatura.

-   A primeira fatura inclui o período inicial a partir da data de início da assinatura até a data da primeira cobrança.
-   As taxas de serviço limitadas podem ser alteradas dentro do ciclo de fatura.
    -   Preço aumenta: 30 dias de aviso prévio é fornecido.
    -   Preço diminui: dia de alteração refletido.
    -   As assinaturas existentes usam a taxa em vigor no início do ciclo de cobrança.
    -   As novas assinaturas (criadas no ciclo de cobrança) usam a taxa em vigor na data de criação.
-   Se você cancelar uma assinatura antes do fechamento da primeira fatura, ou no meio de um ciclo de cobrança, as cobranças por uso aparecerão no arquivo de reconciliação pelo período em que a assinatura estava ativa.

## <a href="" id="licensebased"></a>Cobrança baseada em licença


Para os meses sem alterações nas assinaturas baseadas em licença, você verá um único item de linha para cada assinatura em seu arquivo de reconciliação e na fatura — a cobrança antecipada pelo próximo mês.

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
<p>Limite de cobrança: cobrança antecipada para o período inteiro do mês, de 15 de junho a 14 de julho para 15 assentos. Supondo que a cobrança por assinatura mensal seja US$ 10, o valor será US$ 10 x 15 assentos = US$ 150.</p></td>
</tr>
<tr class="odd">
<td>Assinatura existente: aumento ou redução da quantidade de licenças</td>
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
<p>Limite de cobrança: cobrança antecipada para o período inteiro do mês de 15 de agosto a 14 de setembro para 10 assentos = US$ 110.</p></td>
</tr>
<tr class="even">
<td>Cancelamento: sem alterações de assentos anteriores</td>
<td><p>Seu arquivo de reconciliação conterá um único item de linha:</p>
<ul>
<li>Um crédito pelos dias não utilizados, já que o período integral foi cobrado antecipadamente no extrato de cobrança anterior. Isso é calculado com base na data de término da assinatura.</li>
</ul></td>
<td>Previously billed advance charge: August 15th to September 14th for 10 seats = 100 USD.
<p>Parte consumida da cobrança antecipada de 15 de agosto de 24 de agosto.</p>
<p>Crédito por dias não utilizados: 25 de agosto a 14 de setembro para 10 assentos = US$ -74,51.</p></td>
</tr>
<tr class="odd">
<td>Cancelamento: com as alterações de assentos anteriores</td>
<td><p>Seu arquivo de reconciliação conterá vários itens de linha:</p>
<ul>
<li>a reversão da cobrança antecipada</li>
<li>encargos de uso proporcional</li>
<li>um crédito pelos dias não utilizados</li>
</ul></td>
<td>Cobrança antecipada cobrada anteriormente: 15 de agosto a 14 de setembro para 10 assentos = US$ 100.
<p>Uso proporcional:</p>
<ul>
<li>De 15 de agosto a 24 de agosto para 10 assentos</li>
<li>De 25 de agosto a 14 de setembro para 5 assentos</li>
</ul>
<p>Crédito por dias não utilizados: de 1 de setembro a 14 de setembro para 5 assentos.</p>
<p>Reversão da cobrança antecipada para todo o período mensal de 15 de agosto a 14 de setembro = US$ -100.</p></td>
</tr>
</tbody>
</table>

 

 

 



