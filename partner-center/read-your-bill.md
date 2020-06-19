---
title: Como ler o arquivo Bill & reconhecimento
ms.topic: article
ms.date: 06/05/2020
description: Saiba mais sobre sua fatura & arquivos de reconciliação. Sua fatura mostra cobranças do Partner Center entre o programa, os produtos e os clientes por esse período mensal.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: LauraBrenner
ms.author: labrenne
keywords: cobrança de assinatura, cobrança, cobrança no partner center, ler minha cobrança, fatura, fatura do partner center, fatura do CSP, onde está minha cobrança?
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: df330ce2e66cf198ce97919c02a15eb7a50f6486
ms.sourcegitcommit: e0a1b4506840486f4bb82620051e0f6a5e81662a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/18/2020
ms.locfileid: "84991882"
---
# <a name="understand-your-bill-and-reconciliation-file---learn-how-to-find-them-in-partner-center"></a>Entenda sua fatura e seu arquivo de reconciliação-saiba como encontrá-las no Partner Center

**Aplica-se a**

- Partner Center
- Partner Center do Microsoft Cloud for US Government

**Funções apropriadas**

- Administrador global
- Administrador de cobrança
- Agente administrativo


Sua **fatura** é um **Resumo de todos os seus encargos do Partner Center** (em todo o programa, todos os produtos e todos os clientes). 

## <a name="invoice-types"></a>Tipos de fatura

A Microsoft emitirá uma fatura para quaisquer encargos baseados em licença (como o Office 365) e encargos com base no uso (como o Azure) e uma fatura separada para cobranças individuais (como Azure RI, Marketplace ou plano do Azure).

Por exemplo,  

**Cenário 1 [moeda única]**: o parceiro tem compras para ofertas de 145P e licenças do O365,  

- O parceiro obterá um PDF de nota fiscal e 2 arquivos de reconciliação que abrangem os encargos do O365 e do Azure (145p).  

**Cenário 2 [moeda única]**: o parceiro tem compras para o Azure ri, o Marketplace e/ou o plano do Azure, juntamente com as compras do 145p.

- O parceiro obterá um PDF de nota fiscal e um arquivo de reconciliação que abrange os encargos do Azure (145p). 

- O parceiro receberá outro PDF de fatura e um arquivo de reconciliação que abrange seus encargos para o Azure RI, Marketplace, plano do Azure. 

**Cenário 3 [várias moedas]**: o parceiro tem compras para o Azure ri em DKK e o plano do Azure em EUR, juntamente com compras 145P em EUR.

- O parceiro receberá um PDF de nota fiscal e um arquivo de reconciliação que abrange os encargos para o Azure RI em DKK. 

- O parceiro receberá um PDF de nota fiscal e um arquivo de reconciliação que abrange os encargos do plano do Azure em EUR. 

- O parceiro receberá outro PDF de fatura e um arquivo de reconciliação que abrange seus encargos para a oferta de 145p em EUR (ou moeda de cobrança do parceiro). 

## <a name="find-your-bill"></a>Encontre sua fatura 

Você pode encontrar sua fatura na página de cobrança do painel no Partner Center. Você também pode encontrar seu histórico de cobrança, tendências de gastos e arquivos de reconciliação nesta página. 

1. Entre no [Painel](https://partner.microsoft.com/dashboard/home) do Partner Center. 

2. No menu à esquerda, selecione **cobrança**. 

3. Na página cobrança, selecione a fatura que você deseja baixar. 

Você pode encontrar um link para a fatura mais recente na parte superior da página em saldo de conta até a data da última nota fiscal. 

Você pode encontrar notas fiscais anteriores na seção Histórico de cobrança. Escolha o ano apropriado e, em seguida, selecione a seta suspensa ao lado do período de cobrança apropriado. Selecione o link ao lado de notas fiscais (. pdf) para baixar a fatura do período. 

## <a name="understanding-invoice-pdf"></a>Noções básicas sobre nota fiscal PDF 

**Notas fiscais para uso e cobranças com base em licença**: faturas para cobranças de serviços como o Office 365 e o Azure estarão disponíveis em dois (2) dias de sua data de cobrança selecionada [UTC].  

**Notas fiscais para encargos de OneTime e recorrente**: faturas de encargos para serviços como o Azure ri, plano do Azure, o Marketplace estará disponível não mais tarde, de 8 a cada mês.  

Abaixo estão alguns dos campos de chave no documento PDF da nota fiscal –

**Número da nota fiscal**: identificador exclusivo para o documento de nota fiscal gerado para o respectivo período de cobrança. 

**Período de cobrança**: esse é o período durante o qual você tem usos e serviços baseados em licença. 

**Data da fatura**: a data de cobrança ou a data de vencimento na qual sua fatura é gerada por mês. 

**Data de vencimento do pagamento**: a data até a qual seu pagamento deve ser recebido. 

**Encargos**: o valor devido em sua moeda de cobrança para o respectivo período de cobrança. 

**Créditos**: créditos (como SLA) ou ajustes para alterações feitas em assinaturas (por exemplo, assento aumenta ou diminui). 

**Instruções de pagamento**: Descrição de como pagar sua fatura, com base em sua região. Sempre certifique-se de incluir o número da fatura ao fazer um pagamento. 

Para obter uma descrição detalhada de todos os campos em seu arquivo de nota fiscal (incluindo campos para encargos de uma vez), consulte [campos de arquivo de nota fiscal](invoice-file.md). 

## <a name="understand-reconciliation-files"></a>Entender os arquivos de reconciliação

 Os arquivos de reconciliação, que fornecem detalhes detalhados/discriminados de seus encargos, estão disponíveis para download junto com o PDF da fatura. Os arquivos de reconciliação incluem identificadores de cliente e identificadores de assinatura que você pode usar para criar faturas de cliente. Veja  [como usar os arquivos de reconciliação](use-the-reconciliation-files.md) para obter mais detalhes sobre os arquivos reconhecimento. 
