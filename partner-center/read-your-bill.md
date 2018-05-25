---
title: Ler sua cobrança | Partner Center
description: Sua fatura é um resumo de todos os encargos (entre programa, produtos e clientes) para o período atual mensal. Está disponível no painel do Partner Center.
ms.assetid: E1BA3415-732F-4385-8996-5E79E200F7F7
author: MaggiePucciEvans
keywords: cobrança de assinatura, cobrança, cobrança no partner center, ler minha cobrança, fatura, fatura do partner center, fatura do CSP, onde está minha cobrança?
ms.openlocfilehash: ce930f95eb14405e46a371fb85fc9af02f39db73
ms.sourcegitcommit: 2d3203dd5e2653af031a8009aa3b999a454acef5
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/10/2018
---
# <a name="read-your-bill"></a>Ler sua cobrança

**Aplicável a**

-  Partner Center
-  Partner Center for Microsoft Cloud for US Government
-  Partner Center for Microsoft Cloud Germany

Acesse o menu **Painel** e selecione **Cobrança** para ver seu histórico de cobrança e tendências, links para sua fatura e arquivo de reconciliação, além de seu pagamento mais recente.

Os parceiros no programa Provedor de Soluções na Nuvem que escolheram a cobrança mensal pagam à Microsoft 60 dias em atraso pelas assinaturas de seus clientes (baseadas em licença e em uso).

>**Observação**<br>
Sua fatura é um resumo de todos os encargos (entre programa, produtos e clientes) para o período de cobrança atual e é disponibilizada em até quatro (4) dias da data de cobrança selecionada.


Para obter detalhes dos encargos por itens, use os arquivos de reconciliação acompanhantes. Os arquivos de reconciliação contêm os IDs de clientes e assinaturas que você usará para criar as faturas dos clientes. Para obter mais informações, consulte [Como usar os arquivos de reconciliação](use-the-reconciliation-files.md).

## <a name="invoice-file-definitions"></a>Definições do arquivo de fatura


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><strong>Campo</strong></td>
<td><strong>Descrição</strong></td>
</tr>
<tr class="even">
<td>EUA FEIN</td>
<td>O ID do Imposto Federal.</td>
</tr>
<tr class="odd">
<td>Número do cliente</td>
<td>Seu número do cliente.</td>
</tr>
<tr class="even">
<td>Cobrar de</td>
<td>O endereço para onde enviamos sua fatura. Para alterar esse endereço, vá para Configurações da conta > Perfil de cobrança do parceiro. </td>
</tr>
<tr class="odd">
<td>Encargos recorrentes</td>
<td>Os encargos mensais (ou anuais) fixos das licenças baseadas em uso compradas, cobradas antecipadamente pelo serviço. Esse número é a soma de todos os encargos da coluna &quot;Subtotal&quot; no arquivo de reconciliação com base em licença (coluna T).</td>
</tr>
<tr class="even">
<td>Tarifas de uso</td>
<td>Uso do Azure, incluindo novos serviços ou aplicativos habilitados e usados durante o mês de cobrança. Esse número é a soma de todos os encargos na coluna &quot;PretaxCharges&quot; no arquivo de reconciliação com base em uso (coluna Z).</td>
</tr>
<tr class="odd">
<td>Créditos e ajustes</td>
<td>Créditos ou ajustes para alterações de assinaturas (exemplo: aumentos ou diminuição de assento).</td>
</tr>
<tr class="even">
<td>Outros descontos</td>
<td>Por exemplo, o desconto que o cliente recebe do preço normal da assinatura. Isso é mostrado como um valor simples, não como um preço por unidade ou licença.</td>
</tr>
<tr class="odd">
<td>Impostos</td>
<td>O total de imposto para os encargos atuais como o total no início da seção detalhes na página 2 da fatura. Esse número é a soma de todos os encargos na:
<ul>
<li>coluna &quot;TaxAmount&quot; do arquivo de reconciliação com base em uso (coluna AA), e</li>
<li>coluna &quot;Tax&quot; do arquivo com base em licença (coluna U).</li>
</ul></td>
</tr>
<tr class="even">
<td>Total dos encargos atuais</td>
<td>O valor devido em moeda de cobrança para o período de faturamento, pago no dia do vencimento.</td>
</tr>
<tr class="odd">
<td>Instruções de pagamento</td>
<td>Descreve como pagar sua fatura, com base em sua região. Inclua o número de sua fatura quando efetuar o pagamento.</td>
</tr>
<tr class="even">
<td>Número da fatura</td>
<td>O número da sua fatura.</td>
</tr>
<tr class="odd">
<td>Período de cobrança</td>
<td>Os parceiros CSP são cobrados mensalmente ou anualmente.</td>
</tr>
<tr class="even">
<td>Data da fatura</td>
<td>A data que você recebe sua fatura.</td>
</tr>

<tr class="odd">
<td>Termos de pagamento</td>
<td>Para as compras únicas, sempre será 60 dias.</td>
</tr>


<tr class="even">
<td>Data do pagamento</td>
<td>Seu pagamento deve ser recebido até essa data.</td>
</tr>
<tr class="odd">
<td>PO do cliente</td>
<td>O número da ordem de compra.</td>
</tr>
<tr class="even">
<td>Atendimento ao cliente</td>
<td>O endereço do site para acessar o atendimento ao cliente.</td>
</tr>
<tr class="odd">
<td>Destinatário do serviço</td>
<td>O endereço onde o serviço é usado. (Esse é o endereço de pessoa jurídica associado à verificação da empresa e não pode ser alterado.)</td>
</tr>
</tbody>
</table>

## <a name="itemized-list-of-one-time-charges"></a>Lista detalhada de encargos únicos

|**Campo** |**Definição**|
|:----------------|:-----------------------------|
|Data |Data da compra. |
|Descrição |Nome do produto. |
|Quantidade |O número de produtos (reservas, por exemplo) comprados. |
|Preço unitário |Preço por produto (reserva, por exemplo). |
|Descontos |Qualquer desconto aplicável. |
|Valor pré-taxado |Subtotal das compras antes dos impostos. |
|Imposto sobre vendas |Valor do imposto. |
|Total |Total a ser pago. |
 



