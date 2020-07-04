---
title: Usar seus arquivos de reconciliação
ms.topic: article
ms.date: 06/08/2020
description: Saiba mais sobre os arquivos de reconciliação no Partner Center e como interpretar as exibições detalhadas de item de linha de encargos para um determinado ciclo de cobrança.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: cdb72310368dd76c43d01129a19328d776c00469
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/03/2020
ms.locfileid: "85949561"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a>Saiba como ler os itens de linha em seus arquivos de reconciliação do Partner Center

Aplica-se a:

- Partner Center
- Partner Center do Microsoft Cloud for US Government

Você pode baixar seus arquivos de reconciliação do Partner Center para obter uma exibição detalhada de item de linha de cada encargo em um ciclo de cobrança. Os detalhes do item de linha incluem encargos para as assinaturas de cada cliente e eventos detalhados (como uma adição de estações de mercado para uma assinatura).

Funções apropriadas:

- Administrador de cobrança
- Administrador global

Para obter informações sobre como ler sua **fatura**, consulte [ler sua fatura](read-your-bill.md).

## <a name="understand-reconciliation-file-fields"></a>Entender os campos de arquivo de reconciliação

- [Campos de arquivo de reconciliação com base em licença](license-based-recon-files.md)
- [Campos de arquivo de reconciliação com base no uso](usage-based-recon-files.md)
- [Campos de arquivo de reconciliação recorrentes e de uso único](one-time-recurring-recon-files.md)
- [Campos de arquivo de reconciliação de uso com classificação diária](daily-rated-usage-recon-files.md)

## <a name="understand-charge-types-in-reconciliation-files"></a>Entender os tipos de encargo em arquivos de reconciliação

Para entender os tipos de encargos em arquivos de reconciliação (a coluna **chargetype** ), confira [tipos de encargo de arquivo de reconciliação](recon-file-charge-types.md).

## <a name="fix-formatting-issues"></a>Corrigir problemas de formatação

Ocasionalmente, um arquivo de reconciliação pode conter problemas de formatação. Por exemplo, esse problema pode ocorrer se a localidade en-US não for usada.

Siga estas etapas para corrigir quaisquer problemas de formatação em seus arquivos de reconciliação:

1. Abra o arquivo de reconciliação (no formato. csv) no Microsoft Excel.
2. Selecione a primeira coluna no arquivo.
3. Abra o **Assistente para converter texto em colunas**. Na faixa de opções, selecione **dados**e, em seguida, selecione **texto para colunas**.
4. No assistente, selecione **tipo de arquivo delimitado**. Em seguida, selecione **Avançar**.
5. No campo **delimitadores** , selecione **vírgula**. (Se a **guia** já estiver selecionada, você poderá deixar essa opção selecionada.) Em seguida, selecione **Avançar**.
6. No campo **formato de dados da coluna** , selecione **Data: MDY**. Em seguida, selecione **Avançar**.
7. No campo **formato de dados da coluna** , selecione **texto** para todas as colunas de valor. Em seguida, selecione **Concluir**.

## <a name="download-reconciliation-files-programmatically"></a>Baixar arquivos de reconciliação programaticamente

Os arquivos de reconciliação podem ser muito grandes e, às vezes, são difíceis de baixar. Para baixar arquivos de reconciliação programaticamente, consulte [obter itens de linha da fatura](https://docs.microsoft.com/partner-center/develop/get-invoiceline-items).

## <a name="map-taxes-or-vat"></a>Impostos do mapa ou IVA

Para mapear impostos ou IVA (imposto sobre valor agregado) para sua fatura:

- Some a coluna de **impostos** do arquivo baseado em licença.
- Some a coluna **TaxAmount** do arquivo baseado em uso.

## <a name="itemize-reconciliation-files-by-partner"></a>Discriminar arquivos de reconciliação por parceiro

Os parceiros no **modelo indireto** podem usar esses campos adicionais em arquivos de reconciliação baseados em licença e de uso para discriminar os arquivos pelo revendedor.

| ID MPN | Descrição |
| ------ | ----------- |
| ID MPN | O identificador de Microsoft Partner Network (MPN) do parceiro CSP (provedor de soluções na nuvem) (direto ou indireto). |
| [ID do MPN do revendedor](#reseller-mpn-id) | O [identificador de MPN do revendedor do registro para a assinatura](#reseller-mpn-id). Este campo corresponde à ID do revendedor listada para a assinatura específica no Partner Center. Só aparece em arquivos de reconciliação para parceiros no modelo indireto. |

### <a name="reseller-mpn-id"></a>ID do MPN do revendedor

Se um parceiro CSP vendeu a assinatura diretamente ao cliente, sua **ID MPN** é listada duas vezes, como a **ID MPN** e a **ID de MPN do revendedor**.

Se um parceiro CSP tiver um revendedor sem **ID MPN**, esse valor será definido como a ID de **MPN** do parceiro em vez disso.

Se o parceiro CSP remover uma **ID de MPN do revendedor**, esse valor será definido como *-1*.

Para exibir ou atualizar a **ID de MPN do revendedor**:

1. Conecte-se ao Partner Center.
2. No menu Partner Center, selecione **Clientes**.
3. Escolha o cliente na lista.
4. No menu cliente, selecione **assinaturas**.
5. Escolha a assinatura na lista.
6. Selecione **Atualizar** para alterar o **Revendedor (ID do MPN)**.
