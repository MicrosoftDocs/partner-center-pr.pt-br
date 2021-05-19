---
title: Entender Partner Center faturas de cobrança
ms.topic: article
ms.date: 05/18/2020
description: Entenda os campos em seu arquivo de fatura para Partner Center cobrança. Incluídos estão campos e definições para todos os campos da fatura e campos de cobrança única.
author: sodeb
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5cb60c775bd8de38b8d7ca69c4dd97cf11b919fd
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110146605"
---
# <a name="understand-partner-center-billing-invoice-fields"></a>Entender Partner Center de fatura de cobrança

**Funções apropriadas:** administrador global | Administrador de gerenciamento de usuários | Administrador de cobrança | Agente de helpdesk

Você pode usar as tabelas a seguir para entender os campos em Partner Center de fatura.

## <a name="invoice-file-fields"></a>Campos de arquivo da fatura

Os campos a seguir aparecem em seus arquivos de fatura.

| Campo | Definição |
| ----- | ---------- |
| US FEIN | Seu FEIN (Número de Identificação do Seu Funcionário Federal). Esse é o seu Estados Unidos de identificador de imposto federal. |
| Número do cliente | Seu número de cliente. |
| Enviar cobrança para | O endereço para onde enviamos sua fatura. Você pode alterar o nome e o endereço da sua empresa em seu Partner Center de cobrança. |
| Cobranças baseada em licença | Os encargos mensais ou anuais simples para suas licenças baseadas em uso adquiridas, cobradas com antecedência do serviço. Esse número é a soma de todos os encargos na **coluna Subtotal** (coluna **T**) no arquivo de reconciliação baseado em licença. |
| Encargos baseados em uso | Seu uso do Azure. Isso inclui novos serviços ou aplicativos habilitados e usados durante o período de cobrança. Esse número é a soma de todos os encargos na **coluna PretaxCharges** (coluna **Z**) em seu arquivo de reconciliação baseado em uso. |
| Descontos | O desconto que o cliente recebe do preço normal da assinatura. Esse número é mostrado como um *valor simples,* não como um preço por unidade ou licença. |
| Credits | Créditos ou ajustes para alterações feitas em assinaturas (por exemplo, aumentos ou diminuições de licença). |
| Subtotal | Total antes de impostos e encargos e créditos sem imposto. |
| Imposto | O imposto total para os encargos atuais, conforme total na seção **Detalhes,** começando na página 2 da sua fatura. Esse número é a soma de todos os encargos na coluna **TaxAmount** (coluna **AA**) em seu arquivo de reconciliação baseado em uso e a coluna de **impostos** (coluna **U**) em seu arquivo de reconciliação baseado em licença. |
| Outros créditos | Créditos sem imposto. |
| Total de encargos atuais | O valor devido em sua moeda de cobrança para o período de cobrança. Esses encargos são devidos à data de vencimento do pagamento. |
| Instruções de pagamento | Descrição de como pagar sua fatura, com base em sua região. *Sempre certifique-se de incluir o número da fatura ao fazer um pagamento.* |
| Número da fatura | O número da sua fatura. |
| Período de pagamento | O período mensal que leva até a data da fatura. Esse é o período durante o qual os serviços baseados em uso são consumidos e os serviços baseados em licença são reconciliados para quaisquer ajustes de crédito ou alterações na contagem de licenças. |
| Data da fatura | A data de cobrança ou a data de aniversário na qual sua fatura é gerada por mês. |
| Termos de pagamento | A condição de pagamento. Para as compras únicas, sempre será 60 dias. |
| Data de vencimento | A data até a qual seu pagamento deve ser recebido. |
| OC Cliente | A ordem do número de compra. |
| Serviço de atendimento ao consumidor | O endereço do site em que você pode acessar o atendimento ao cliente. |
| Destinatário de serviço | O endereço em que o serviço está sendo usado. (Este é o endereço da empresa legal associado à empresa habilitação.) |

## <a name="one-time-charges-fields"></a>Campos de encargos de uma vez

Os campos a seguir se aplicam somente a **encargos únicos** no Partner Center:

| Campo | Definição |
| ----- | ---------- |
| Data | Data da compra. |
| Descrição | Nome do produto. |
| Quantidade | O número de produtos (como reservas) adquiridos. |
| Preço unitário | Preço por produto (como uma reserva). |
| Descontos | Qualquer desconto aplicável. |
| Valor pré-taxado | Subtotal das compras antes dos impostos. |
| Imposto sobre vendas | Valor do imposto. |
| Total | Valor total a ser pago. |
