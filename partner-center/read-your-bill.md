---
title: Ler sua cobrança | Partner Center
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Sua fatura é um resumo de todos os encargos (entre programa, produtos e clientes) para o período atual mensal. Ele está disponível no Partner Center.
ms.assetid: E1BA3415-732F-4385-8996-5E79E200F7F7
author: MaggiePucciEvans
ms.author: evansma
keywords: cobrança de assinatura, cobrança, cobrança no partner center, ler minha cobrança, fatura, fatura do partner center, fatura do CSP, onde está minha cobrança?
ms.localizationpriority: medium
ms.openlocfilehash: 37469a72137d5bc399f5ab765c49c8accd36808d
ms.sourcegitcommit: dbaa6c2e8a0e6431f1420e024cca6d0dd54f1425
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/06/2019
ms.locfileid: "73652180"
---
# <a name="read-your-bill"></a>Ler sua cobrança

**Aplica-se a**

-  Partner Center
-  Partner Center do Microsoft Cloud for US Government


Para sua fatura, vá para o menu do **Partner Center** e, em seguida, selecione **cobrança** para ver seu histórico de cobrança e tendências, links para sua fatura e arquivo de reconciliação e o pagamento mais recente.

Os parceiros no programa Provedor de Soluções na Nuvem que escolheram a cobrança mensal pagam à Microsoft 60 dias em atraso pelas assinaturas de seus clientes (baseadas em licença e em uso).

> [!NOTE]  
> Sua fatura é um resumo de todos os encargos, entre o programa, os produtos e os clientes – para o período de cobrança atual e está disponível dentro de dois (2) dias de sua data de cobrança selecionada em hora UTC. Por exemplo, se você tiver uma data de cobrança de 12 de setembro, o processo de geração de nota fiscal começará em 12:10:00 UTC na 13 e será concluído por 12:10:00 UTC no dia 14. Se você não vir sua fatura por 11:59PM UTC no dia 15, você está fora de seu Contrato de Nível de Serviço e deve arquivar uma solicitação de serviço. 

Você receberá uma fatura para encargos baseados em licença (Office365) e baseados em uso (Azure) e uma fatura separada para encargos (instâncias de VM reservadas do Azure).

Para obter detalhes discriminados sobre os encargos, use os arquivos de reconciliação correspondentes. Os arquivos de reconciliação contêm os IDs de clientes e assinaturas que você usará para criar as faturas dos clientes. Para obter mais informações, consulte [Como usar os arquivos de reconciliação](use-the-reconciliation-files.md).

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
<td>O endereço para onde enviamos sua fatura. Para alterar o nome ou o endereço da empresa, edite seu perfil de cobrança do Partner Center. </td>
</tr>
<tr class="odd">
<td>Cobranças baseada em licença</td>
<td>Os encargos mensais (ou anuais) fixos das licenças baseadas em uso compradas, cobradas antecipadamente pelo serviço. Esse número é a soma de todos os encargos da coluna &quot;Subtotal&quot; no arquivo de reconciliação com base em licença (coluna T).</td>
</tr>
<tr class="even">
<td>Encargos baseados em uso</td>
<td>Uso do Azure, incluindo novos serviços ou aplicativos habilitados e usados durante o mês de cobrança. Esse número é a soma de todos os encargos na coluna &quot;PretaxCharges&quot; no arquivo de reconciliação com base em uso (coluna Z).</td>
</tr>
<tr class="odd">
<td>Descontos</td>
<td>Por exemplo, o desconto que o cliente recebe do preço normal da assinatura. Isso é mostrado como um valor simples, não como um preço por unidade ou licença.</td>
</tr>
<tr class="odd">
<td>Créditos</td>
<td>Créditos ou ajustes para alterações de assinaturas (exemplo: aumentos ou reduções de estações).</td>
</tr>
<tr class="even">
<tr class="even">
<td>Subtotal</td>
<td>Total antes de impostos e encargos e créditos sem imposto.</td>
</tr>
<td>Tax</td>
<td>O total de imposto para os encargos atuais como o total no início da seção detalhes na página 2 da fatura. Esse número é a soma de todos os encargos na:
<ul>
<li>coluna &quot;TaxAmount&quot; do arquivo de reconciliação com base em uso (coluna AA), e</li>
<li>a coluna &quot;Imposto&quot; do arquivo com base em licença (coluna U).</li>
</ul></td>
</tr>
<tr class="odd">
<td>Outros créditos</td>
<td>Créditos sem imposto.</td>
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
<td>O período mensal que leva até a data da fatura. Esse é o período durante o qual os serviços baseados em uso são consumidos e os serviços baseados em licença são reconciliados para quaisquer ajustes de crédito ou alterações na contagem de licenças.</td>
</tr>
<tr class="even">
<td>Data da fatura</td>
<td>Sua data de cobrança ou data de aniversário na qual sua fatura é gerada por mês.</td>
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
<td>O endereço onde o serviço é usado. (Este é o endereço da empresa legal associado à empresa habilitação.)</td>
</tr>
</tbody>
</table>

## <a name="itemized-list-of-one-time-charges"></a>Lista detalhada de encargos únicos

|**Campo** |**Definição**|
|:----------------|:-----------------------------|
|Data |Data da compra. |
|Descrição |Nome do produto. |
|Quantity |O número de produtos (reservas, por exemplo) comprados. |
|Preço unitário |Preço por produto (reserva, por exemplo). |
|Descontos |Qualquer desconto aplicável. |
|Valor pré-taxado |Subtotal das compras antes dos impostos. |
|Imposto sobre vendas |Valor do imposto. |
|Total |Total a ser pago. |
 



