---
title: Gerenciar sua lista de clientes
ms.topic: article
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Os registros de clientes estão entre os ativos de informações mais importantes. Saiba como exibir, Pesquisar, atualizar & informações de exportação em sua lista de clientes do Partner Center.
ms.assetid: 58444AB8-AD6E-4686-9D4E-F9FA110A99FC
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 2ba70cfccf3597868187c6b3c91c313732af1ab7
ms.sourcegitcommit: 7ec7514ee9693d62d8eb930aa38fe701cd152835
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2020
ms.locfileid: "84426025"
---
# <a name="manage-your-customer-list---search-update-or-export-customers-in-partner-center"></a>Gerenciar sua lista de clientes – Pesquisar, atualizar ou exportar clientes no Partner Center

**Aplica-se a**

- Partner Center
- Partner Center do Microsoft Cloud for US Government

Os registros de clientes estão entre seus ativos de informação mais importantes no Partner Center. Você pode pesquisar seu banco de dados de contas de clientes, exportar o banco de dados de clientes inteiro ou exportar um subconjunto para um formato de arquivo de valores separados por vírgula (.csv) compatível com o Excel. Você também pode exportar as informações de assinaturas do cliente para um arquivo .csv.

Os logs de atividades também fornecem dados exportáveis sobre transações e ações de gerenciamento de clientes. Para obter mais informações, consulte [Exibir logs de atividades do cliente](activity-logs.md).

## <a name="search-for-a-customer"></a>Procurar um cliente

1.  No menu do **centro de parceiros** , selecione **clientes**.
2.  Para procurar um cliente, insira o nome do cliente ou o nome do domínio na caixa de pesquisa.
3.  Selecione a **seta para baixo** no final da linha de um cliente para ver a ID da Microsoft dele, bem como os links rápidos de assinaturas e serviços associados.

## <a name="update-a-customers-company-name"></a>Atualize o nome da empresa do cliente

No menu do **centro de parceiros** , selecione **clientes**.
2.  Para procurar um cliente, insira o nome do cliente ou o nome do domínio na caixa de pesquisa.
3.  Selecione a **seta para baixo** no final da linha de um cliente para ver a ID da Microsoft dele, bem como os links rápidos de assinaturas e serviços associados.
4.  Nas informações de **Cobrar de** do cliente, atualize o nome da empresa. Quando você salvar o novo valor, ele será refletido na lista de clientes. Isso irá alterar somente o nome da empresa para cobrança e o valor de lista de cliente. Ele não será refletido em nenhum outro lugar.
<sup>1</sup>
## <a name="export-your-customer-list"></a>Exportar sua lista de clientes

1. No menu do **centro de parceiros** , selecione **clientes**.
2. Selecione **Exportar clientes**.

   O Partner Center converte a lista completa de clientes em um arquivo .csv e o carrega na pasta de download padrão em seu computador. Você também pode exportar os subconjuntos de dados do cliente. As colunas de dados incluem o seguinte:

   - **ID da Microsoft**;
   - **Nome da empresa**;
   - **Nome de domínio primário**;
   - **Relacionamento** — relacionamento comercial do parceiro para cada cliente listado.

    Por padrão, o Partner Center exporta a lista completa de clientes, independentemente do tamanho. Você também pode pesquisar a lista de clientes por nome de empresa ou domínio e exportar esse subconjunto de dados.

3. Se você for um provedor indireto, pode filtrar sua lista de clientes por revendedor indireto. Selecione **Filtrar por revendedor indireto** na lista e, em seguida, escolha um revendedor.
<sup>1</sup>

## <a name="export-customer-subscription-information"></a>Exportar informações de assinatura de cliente

1. No menu do **centro de parceiros** , selecione **clientes**.

2. Selecione o **Nome da empresa** de qualquer cliente. A página **Assinaturas** do cliente será aberta, mostrando a lista completa de assinaturas de produtos.

3. Selecione **Exportar assinaturas**. O Partner Center converte os dados de assinatura do cliente em um arquivo .csv e o carrega na pasta de download padrão em seu computador. As colunas de dados incluem o seguinte:
   - **ID da assinatura**;
   - **Assinatura** — o nome do produto da assinatura;
   - **Quantidade** — número de licenças adquiridas;
   - **Status**;
   - **Revendedor** — a ID do revendedor que possui e gerencia a assinatura.

> [!NOTE]  
> Para obter mais informações sobre o gerenciamento de assinaturas, consulte [Assinaturas de cliente](customer-subscriptions.md).
