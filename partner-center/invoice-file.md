---
title: Arquivos de fatura | Centro de parceiros
ms.topic: article
ms.date: 08/26/2019
description: Entenda os campos em seu arquivo de nota fiscal para cobrança do Partner Center.
ms.assetid: ''
author: MaggiePucciEvans
ms.author: evansma
keywords: cobrança, fatura
ms.localizationpriority: medium
ms.openlocfilehash: 9b3219b5752de59b9dde81343b8bd4e1128037bd
ms.sourcegitcommit: 1c3d3b95135e1daad5ba5585a090e84ab0b97594
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/22/2019
ms.locfileid: "74389834"
---
# <a name="invoice-files"></a>Arquivos de fatura

Você pode usar as tabelas a seguir para entender os campos em arquivos de notas fiscais do Partner Center.

## <a name="invoice-file-fields"></a>Campos de arquivo de fatura

Os campos a seguir aparecem nos arquivos da fatura.

| Campo | Definição |
| ----- | ---------- |
| EUA FEIN | Seu número de identificação do empregador Federal (FEIN). Este é o seu número de identificador de imposto federal Estados Unidos. |
| Número do cliente | Seu número do cliente. |
| Cobrar de | O endereço onde podemos enviar sua fatura. Você pode alterar o nome e/ou o endereço da sua empresa no perfil de cobrança do Partner Center. |
| Cobranças baseada em licença | As tarifas fixas mensais ou anuais para suas licenças baseadas em uso adquiridas, cobradas antes do serviço. Esse número é a soma de todos os encargos na coluna de **Subtotal** (coluna **T**) em seu arquivo de reconciliação baseado em licença. |
| Encargos baseados em uso | Seu uso do Azure. Isso inclui novos serviços ou aplicativos habilitados e usados durante o período de cobrança. Esse número é a soma de todos os encargos na coluna **PretaxCharges** (coluna **Z**) em seu arquivo de reconciliação baseado em uso. |
| Descontos | O desconto que o cliente recebe do preço normal da assinatura. Esse número é mostrado como um *valor fixo*, não como um preço por unidade ou licença. |
| Créditos | Créditos ou ajustes para alterações feitas em assinaturas (por exemplo, assento aumenta ou diminui). |
| Subtotal | Total antes de impostos e encargos e créditos sem imposto. |
| Tax | O imposto total para seus encargos atuais, conforme totalizado na seção de **detalhes** que começa na página 2 da fatura. Esse número é a soma de todos os encargos na coluna **TaxAmount** (coluna **AA**) em seu arquivo de reconciliação baseado em uso e a coluna de **impostos** (coluna **U**) em seu arquivo de reconciliação baseado em licença. |
| Outros créditos | Créditos sem imposto. |
| Total dos encargos atuais | O valor devido em sua moeda de cobrança para o período de cobrança. Esses encargos são devidos à data de vencimento do pagamento. |
| Instruções de pagamento | Descrição de como pagar sua fatura, com base em sua região. *Sempre certifique-se de incluir o número da fatura ao fazer um pagamento.* |
| Número da fatura | O número da sua fatura. |
| Período de cobrança | O período mensal que leva até a data da fatura. Esse é o período durante o qual os serviços baseados em uso são consumidos e os serviços baseados em licença são reconciliados para quaisquer ajustes de crédito ou alterações na contagem de licenças. |
| Data da fatura | A data de cobrança ou a data de aniversário na qual sua fatura é gerada por mês. |
| Termos de pagamento | A condição de pagamento. Para as compras únicas, sempre será 60 dias. |
| Data do pagamento | A data até a qual seu pagamento deve ser recebido. |
| PO do cliente | A ordem do número de compra. |
| Atendimento ao cliente | O endereço do site em que você pode acessar o atendimento ao cliente. |
| Destinatário do serviço | O endereço em que o serviço está sendo usado. (Este é o endereço da empresa legal associado à empresa habilitação.) |

## <a name="one-time-charges-fields"></a>Campos de encargos de uma vez

Os campos a seguir se aplicam somente a **encargos únicos** no Partner Center:

| Campo | Definição |
| ----- | ---------- |
| Date | Data da compra. |
| Descrição | Nome do produto. |
| Quantity | O número de produtos (como reservas) adquiridos. |
| Preço unitário | Preço por produto (como uma reserva). |
| Descontos | Qualquer desconto aplicável. |
| Valor pré-taxado | Subtotal das compras antes dos impostos. |
| Imposto sobre vendas | Valor do imposto. |
| Total | Valor total a ser pago. |