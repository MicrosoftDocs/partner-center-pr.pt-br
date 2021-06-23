---
title: Como ler seu arquivo de & reconhecimento
ms.topic: article
ms.date: 06/05/2020
description: Saiba mais sobre sua fatura & arquivos de reconciliação. Sua fatura mostra Partner Center encargos em todo o programa, produtos e clientes para esse período mensal.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: bbdf85d20e15841189191d6b415b54c26378850e
ms.sourcegitcommit: 8dc9f28f15d9760a8363826513b4470b76b40ff3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2021
ms.locfileid: "112551190"
---
# <a name="understand-your-bill-and-reconciliation-file---learn-how-to-find-them-in-partner-center"></a>Entender seu arquivo de cobrança e reconciliação – saiba como encontrá-los Partner Center


**Funções apropriadas:** administrador global | Administrador de cobrança | Agente administrador


Sua **fatura** é um **resumo de todas as suas Partner Center (em** todo o programa, todos os produtos e todos os clientes). 

## <a name="find-your-bill-and-reconciliation-file"></a>Encontrar seu arquivo de cobrança e reconciliação 

Você pode encontrar sua fatura na página Cobrança do painel Partner Center. Você também pode encontrar seu histórico de cobrança, tendências de gastos e arquivos de reconciliação nesta página. 

1. Entre no [painel](https://partner.microsoft.com/dashboard/home) do Partner Center. 

2. No menu à esquerda, selecione **Cobrança**. 

3. Na página de status da cobrança, selecione uma nota fiscal ou um arquivo de reconciliação para exibir informações mais detalhadas. 

Você pode encontrar um link para sua fatura mais recente na parte superior da página em Saldo da conta a partir da data da última fatura. 

Você pode encontrar faturas anteriores na seção Histórico de cobrança. Escolha o ano apropriado e, em seguida, selecione a seta para baixo ao lado do período de Cobrança apropriado. Selecione o link ao lado de Faturas (.pdf) para baixar a fatura desse período. 

## <a name="invoice-types"></a>Tipos de fatura

A Microsoft emitirá uma fatura para quaisquer encargos baseados em licença (como o Office 365) e encargos baseados em uso (como o Azure) e uma fatura separada para cobranças avuárias (como RI do Azure, Marketplace ou plano do Azure).

Por exemplo,  

**Cenário 1 [Moeda Única]**: o parceiro tem compras para a oferta de 145P e licenças do Office 365,  

- O parceiro receberá um PDF da fatura e dois arquivos de reconciliação que abrangem os encargos do Office 365 e do Azure (145p).  

**Cenário 2 [Moeda Única]**: o parceiro tem compras para o plano de RI, Marketplace e/ou Azure do Azure, juntamente com compras de 145p.

- O parceiro receberá um PDF da fatura e um arquivo de reconciliação que abrange os encargos do Azure (145p). 

- O parceiro receberá outro PDF da fatura e um arquivo de reconciliação que abrange seus encargos para RI (instância reservada) do Azure, Marketplace e plano do Azure. 

**Cenário 3 [Multi-Currency]**: o parceiro tem compras para RI do Azure em DKK e plano do Azure em EUR, juntamente com compras de 145p na EUR.

- O parceiro receberá um PDF da fatura e um arquivo de reconciliação que abrange os encargos da RI do Azure no DKK. 

- O parceiro receberá um PDF da fatura e um arquivo de reconciliação que abrange os encargos do plano do Azure na EUR. 

- O parceiro receberá outro PDF da fatura e um arquivo de reconciliação que abrange os encargos da oferta de 145p em EUR (ou moeda de cobrança do parceiro). 


## <a name="understanding-invoice-pdf"></a>Noções básicas sobre PDF da fatura 

**Faturas** de uso e encargos baseados em licença: as faturas para encargos de serviços como o Office 365 e o Azure estarão disponíveis dentro de dois (2) dias após a data de cobrança selecionada [UTC].  

**Faturas para cobranças** avuárias e recorrentes: faturas para encargos para serviços como RI do Azure, plano do Azure, Marketplace estarão disponíveis não posteriormente ao oitavo dia de cada mês.  

Abaixo estão alguns dos campos de chave no documento PDF da fatura –

**Número da** fatura: identificador exclusivo para o documento da fatura gerado para o respectivo período de cobrança. 

**Período de cobrança:** esse é o período durante o qual você tem usos e serviços baseados em licença. 

**Data da** fatura: a data de cobrança ou a data de aniversário na qual sua fatura é gerada a cada mês. 

**Data de vencimento do** pagamento: a data pela qual o pagamento deve ser recebido. 

**Encargos:** o valor devido em sua moeda de cobrança para o respectivo período de cobrança. 

**Créditos:** créditos (como SLA (contrato de nível de serviço)) ou ajustes para alterações feitas em assinaturas (por exemplo, aumentos ou diminuições de licença). 

**Instruções de pagamento:** descrição de como pagar sua fatura, com base em sua região. Sempre certifique-se de incluir o número da fatura ao fazer um pagamento. 

Para ver uma descrição detalhada de todos os campos em seu arquivo de fatura (incluindo campos para encargos avissos), consulte [Campos de arquivo da fatura](invoice-file.md). 

## <a name="understand-reconciliation-files"></a>Entender os arquivos de reconciliação

 Os arquivos de reconciliação, que fornecem um detalhamento/detalhes de seus encargos, estão disponíveis para download junto com o PDF da fatura. Os arquivos de reconciliação incluem identificadores de cliente e identificadores de assinatura que você pode usar para criar faturas do cliente. Para obter mais informações sobre arquivos de reconciliação, [consulte Como usar os arquivos de reconciliação](use-the-reconciliation-files.md). 

## <a name="next-steps"></a>Próximas etapas

- [Como usar os arquivos de reconciliação](use-the-reconciliation-files.md)