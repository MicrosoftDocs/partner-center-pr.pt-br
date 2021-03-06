---
title: Gerenciar sua lista de clientes
ms.topic: how-to
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Os registros de clientes estão entre os ativos de informações mais importantes. Saiba como exibir, Pesquisar, atualizar & informações de exportação em sua lista de clientes do Partner Center.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 6e73aa98e0cfaf82521a5fe63e34ebf0b44363fb
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854495"
---
# <a name="manage-your-customer-list---search-update-or-export-customers-in-partner-center"></a>Gerenciar sua lista de clientes – Pesquisar, atualizar ou exportar clientes no Partner Center

**Aplica-se a**: Partner Center | Partner Center para Microsoft Cloud do governo dos EUA

**Funções apropriadas**: agente de administração | Administrador global

Os registros de clientes estão entre seus ativos de informação mais importantes no Partner Center. Você pode pesquisar seu banco de dados de contas de clientes, exportar o banco de dados de clientes inteiro ou exportar um subconjunto para um formato de arquivo de valores separados por vírgula (.csv) compatível com o Excel. Você também pode exportar as informações de assinaturas do cliente para um arquivo .csv.

Os logs de atividades também fornecem dados exportáveis sobre transações e ações de gerenciamento de clientes. Para obter mais informações, consulte [Exibir logs de atividades do cliente](activity-logs.md).

## <a name="search-for-a-customer"></a>Procurar um cliente

1. No menu do **centro de parceiros** , selecione **clientes**.
2. Para procurar um cliente, insira o nome do cliente ou o nome do domínio na caixa de pesquisa.
3. Selecione a **seta para baixo** no final da linha de um cliente para ver a ID da Microsoft dele, bem como os links rápidos de assinaturas e serviços associados.

## <a name="update-a-customers-company-name"></a>Atualize o nome da empresa do cliente

No menu do **centro de parceiros** , selecione **clientes**.
2. Para procurar um cliente, insira o nome do cliente ou o nome do domínio na caixa de pesquisa.
3. Selecione a **seta para baixo** no final da linha de um cliente para ver a ID da Microsoft dele, bem como os links rápidos de assinaturas e serviços associados.
4. Nas informações de **Cobrar de** do cliente, atualize o nome da empresa. Quando você salvar o novo valor, ele será refletido na lista de clientes. Isso irá alterar somente o nome da empresa para cobrança e o valor de lista de cliente. Ele não será refletido em nenhum outro lugar.

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
