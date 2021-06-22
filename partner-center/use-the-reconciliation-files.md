---
title: Usar seus arquivos de reconciliação
ms.topic: article
ms.date: 03/26/2021
description: Saiba mais sobre arquivos de reconciliação Partner Center e como interpretar as exibições detalhadas de itens de linha de encargos para um determinado ciclo de cobrança.
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: sodeb
ms.author: sodeb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 1a7d5f3169c4b338a07475a7e246e87841b8dcfb
ms.sourcegitcommit: bce54ddb9fff7332a03d6aa228ba9414a87d76b7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2021
ms.locfileid: "112431566"
---
# <a name="learn-how-to-read-the-line-items-in-your-partner-center-reconciliation-files"></a>Saiba como ler os itens de linha em seus arquivos Partner Center reconciliação

**Funções apropriadas:** administração de cobrança | Administrador global

Você pode baixar seus arquivos de reconciliação Partner Center para uma exibição detalhada de item de linha de cada cobrança em um ciclo de cobrança. Os detalhes do item de linha incluem encargos para assinaturas de cada cliente e eventos detalhados (como uma adição de licenças de médio prazo a uma assinatura).

Para obter informações sobre como ler sua **fatura,** consulte [Ler sua fatura.](read-your-bill.md)

## <a name="understand-reconciliation-file-fields"></a>Entender os campos do arquivo de reconciliação

- [Campos do arquivo de reconciliação baseados na licença](license-based-recon-files.md)
- [Campos do arquivo de reconciliação baseados no uso](usage-based-recon-files.md)
- [Campos do arquivo de reconciliação de uso com classificação diária](daily-rated-usage-recon-files.md)
- [Campos de arquivo de reconciliação do CSP de compra única](modern-invoice-reconciliation-file.md)

## <a name="understand-charge-types-in-reconciliation-files"></a>Entender os tipos de cobrança em arquivos de reconciliação

Para entender os tipos de encargos em arquivos de reconciliação (a **coluna ChargeType),** consulte Tipos de cobrança de arquivo [de reconciliação](recon-file-charge-types.md).

## <a name="fix-formatting-issues"></a>Corrigir problemas de formatação

Ocasionalmente, um arquivo de reconciliação pode conter problemas de formatação. Por exemplo, esse problema poderá ocorrer se a localidade en-US não for usada.

Siga estas etapas para corrigir problemas de formatação em seus arquivos de reconciliação:

1. Abra o arquivo de reconciliação (no .csv) no Microsoft Excel.
2. Selecione a primeira coluna no arquivo.
3. Abra o **Assistente para Converter Texto em Colunas**. Na faixa de opções, selecione **Dados** e, em **seguida, selecione Texto em Colunas.**
4. No assistente, selecione **Tipo de arquivo delimitado**. Em seguida, selecione **Avançar**.
5. No campo **Delimitadores,** selecione **Vírgula**. (Se **Tab** já estiver selecionado, você poderá deixar essa opção selecionada.) Em seguida, selecione **Próximo.**
6. No campo **Formato de dados da** coluna, selecione **Data:MDY.** Em seguida, selecione **Avançar**.
7. No campo **Formato de dados de** coluna, selecione Texto **para** todas as colunas de valor. Em seguida, selecione **Concluir**.

## <a name="download-reconciliation-files-programmatically"></a>Baixar arquivos de reconciliação programaticamente

Os arquivos de reconciliação podem ser muito grandes e, às vezes, são difíceis de baixar. Para baixar arquivos de reconciliação programaticamente, consulte [Obter itens de linha da fatura](/partner-center/develop/get-invoiceline-items).

## <a name="if-your-file-exceeds-the-row-limit-in-excel"></a>Se o arquivo exceder o limite de linha no Excel

Se você conseguir baixar um arquivo de reconciliação, mas não abri-lo no Microsoft Excel, isso provavelmente significa que o arquivo contém mais linhas do que o Excel permitirá. Se isso acontecer, você poderá usar qualquer um dos procedimentos abaixo para abrir o arquivo.

### <a name="open-a-recon-file-in-power-bi"></a>Abra um arquivo de reconhecimento no Power BI

1. Baixe o arquivo de reconciliação como faria normalmente.
2. Baixe, instale e abra uma instância do Microsoft Power BI.
3. Na guia Power BI **Página** Base, selecione **Obter dados**.
4. Na lista de fontes **de dados comuns,** selecione **Texto/CSV.**
5. Quando solicitado, abra o arquivo de reconhecimento.

### <a name="open-a-recon-file-in-an-excel-pivot-table"></a>Abrir um arquivo de reconhecimento em uma tabela dinâmica do Excel

1. Baixe o arquivo de reconciliação como faria normalmente.
2. Abra um novo arquivo no Microsoft Excel.
3. Na guia **Dados,** selecione **Obter dados,** selecione **Do arquivo** e, em seguida, **selecione Texto/CSV.**
4. Quando solicitado, abra o arquivo de reconhecimento. Seus dados serão exibidos.
5. No menu **suspenso** Carregar, selecione **Carregar para** e, em seguida, selecione **OK.**
6. Na caixa **de diálogo Importar** Dados, selecione Relatório de Tabela **Dinâmica** para abrir o arquivo.

## <a name="negative-amount-displayed"></a>Valor negativo exibido

Você pode ver uma quantidade negativa em seu arquivo de reconciliação. As causas podem ser:

- Você cancelou ou reduziu recentemente seu número de licenças
- Você recebeu crédito por um SLA (Contrato de Licença de Serviço) ou pelo consumo do Azure

Confira mais informações sobre essa transação examinando o atributo de tipo de encargo em seu arquivo de reconciliação.

## <a name="map-taxes-or-vat"></a>Mapear impostos ou IVA

Para mapear os impostos ou o IVA (imposto sobre valor agregado) para sua fatura:

- Soma a **coluna Imposto** do arquivo baseado em licença.
- Soma a **coluna TaxAmount** do arquivo baseado em uso.

## <a name="itemize-reconciliation-files-by-partner"></a>Itemizar arquivos de reconciliação por parceiro

Os parceiros no **modelo indireto** podem usar esses campos adicionais em arquivos de reconciliação baseados em licença e em uso para itemizar os arquivos por revendedor.

| ID MPN | Descrição |
| ------ | ----------- |
| ID MPN | O Microsoft Partner Network (MPN) do parceiro Provedor de Soluções na Nuvem (CSP) (direto ou indireto). |
| [ID do MPN do revendedor](#reseller-mpn-id) | O [identificador MPN do revendedor de registro para a assinatura](#reseller-mpn-id). Esse campo corresponde à ID do revendedor listada para a assinatura específica no Partner Center. Só aparece em arquivos de reconciliação para parceiros no modelo indireto. |

### <a name="reseller-mpn-id"></a>ID do MPN do revendedor

Se um parceiro CSP vender a assinatura diretamente para o cliente, sua ID do **MPN** será listada duas vezes, como a **ID** do MPN e a ID do **MPN do Revendedor.**

Se um parceiro CSP tiver um revendedor sem ID do **MPN,** esse valor será definido como a ID do **MPN do** parceiro.

Se o parceiro CSP remover uma **ID do MPN** do Revendedor, esse valor será definido como *-1*.

Para exibir ou atualizar a **ID do MPN do Revendedor:**

1. Conecte-se ao Partner Center.
2. No menu Partner Center, selecione **Clientes**.
3. Escolha o cliente na lista.
4. No menu do cliente, selecione **Assinaturas**.
5. Escolha a assinatura na lista.
6. Selecione **Atualizar** para alterar o **Revendedor (ID do MPN)**.

## <a name="next-steps"></a>Próximas etapas

- [Como ler seu arquivo de & reconhecimento](read-your-bill.md) 