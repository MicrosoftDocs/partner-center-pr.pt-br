---
title: Vender assinaturas de software por meio do CSP | Partner Center
ms.topic: article
ms.date: 11/20/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Learn how partners in the CSP program can use Partner Center to buy, manage, sell, and cancel Azure reserved instances and Server subscriptions for customers.
author: MaggiePucciEvans
ms.author: evansma
keywords: Provedor de Soluções na Nuvem, CSP, Serviços baseados na nuvem, Azure, Azure RI, Windows Server, SQL Server, assinaturas de software
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 32efdc721bd9a81ff04527ca82e5e71c1fe7cb58
ms.sourcegitcommit: 524d3121e5053a74911e2fd4e9cf5aab14f6b48d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/20/2019
ms.locfileid: "74253546"
---
# <a name="sell-software-subscriptions-through-csp"></a>Vender assinaturas de software por meio do CSP

With Azure reservations and Server subscriptions (Windows Server and SQL Server subscriptions), partners in the CSP program can better address the fast-growing customer demand for more cost-effective solutions to support highly predictable and persistent cloud workloads. 

You can now acquire, provision, and manage Azure reservations and Server subscriptions on behalf of commercial customers through Partner Center and the Azure Portal by taking advantage of the Azure Hybrid Benefit. 

O Benefício Híbrido do Azure ajuda você a obter mais valor de suas licenças do Windows Server e a economizar até 40% em máquinas virtuais. Você pode usar o benefício com licenças do Windows Server Datacenter e Standard edition cobertas com Software Assurance. Depending on the edition, you can convert or re-use your licenses to run Windows Server virtual machines in Azure and pay a lower base compute rate (Linux virtual machine rates, e.g.).

> [!NOTE]  
> Azure reservations are not available in the following markets:  
> * Argentina
> * Brasil
> * China
> * Indonésia
> * Liechtenstein
> * Jersey
> * Malásia
> * México
> * Rússia
> * Arábia Saudita
> * África do Sul
> * Turquia

<!--March 20, 2019 - this list of countries was correct as of today. Maggie last updated the list according to FAREAST\v-pubobb in bug 20907186.
-->

## <a name="buy-software-subscriptions-on-behalf-of-customers"></a>Comprar assinaturas de software em nome dos clientes

To buy software subscriptions on behalf of a customer, go to the customer's detail page, select **Add products**, and then follow the on-screen instructions to create and pay for your order. All commercial pricing excludes tax with the exception of Australia and Brazil. For Australia and Brazil, the price includes tax.

## <a name="activate-and-manage-software-subscriptions"></a>Ativar e gerenciar assinaturas de software

After you purchase the software subscription, follow the steps below to download it.

>[!NOTE]
>You must be an Admin agent to download software and get activation keys.

1. Acesse a página de detalhes do cliente e então selecione **Software**. You'll see a list of all the software you've purchased on behalf of the customer. 
2.  Expanda o produto que você deseja baixar. No campo **Selecionar produto**, selecione a **Versão**, o **Idioma** e o **Tipo de arquivo/sistema operacional** desejados. 
3.  Selecione **Enviar** para exibir os produtos específicos. 
4.  Selecione **Obter chaves e downloads**. 
5.  Selecione **Baixar** para iniciar o download ou selecione **Copiar link** para copiar o link e enviá-lo ao cliente. 

>[!NOTE]
>Esse link expirará após duas semanas ou 50 downloads, o que ocorrer primeiro. Depois que o link expirar, retorne a essa página e selecione **Obter chaves e downloads** novamente para habilitar outras duas semanas ou 50 downloads. Você pode fazer isso quantas vezes precisar. 

## <a name="view-activity-for-software-key-access-and-software-downloads"></a>View activity for software key access and software downloads
For auditing or compliance purposes, you may need to check a list of users who have either accessed Server subscription software keys or downloaded Server subscription software. Use the procedure below to access this information. 

>[!NOTE]
>You must be a Global administrator, Account admin, Referral admin, or Marketing content admin to see these activity logs. 

1.  In Partner Center, select the gear icon from the upper right corner. 
2.  In the menu, select **Activity log**.
3.  Enter the date range for the activity you want to see. The activity log will display a list of users who have either accessed software keys or downloaded software during the time you specified. 

## <a name="cancel-a-purchase"></a>Cancelar uma compra

You can cancel a software purchase within 60 days of the purchase date. Microsoft does not charge an early termination fee, however, you can't cancel a purchase after 60 days from the purchase date.

After you cancel the purchase, the software key will be revoked. 

Follow the steps below to cancel a purchase:

>[!NOTE]
>Você deve ser um agente administrativo para cancelar uma compra. 

1.  Antes do início do processo, verifique se você tem o seguinte:
    -   O GUID do locatário do cliente ou o nome de domínio
    -   ID do Pedido ou ID da Assinatura
    -   Motivo do reembolso
    -   Quantidade solicitada

2.  On the customer's details page, select **Software** to see the list of all the software you've purchased for the customer. 

3.  Locate the software you want to cancel, and then select **Cancel**. A página **Relatar um problema com o Partner Center** abre. 

4.  Em **Detalhes**, na lista **Tipo de problema**, selecione **Compra/Reembolso de CSP em nome de clientes**.

5.  Preencha os campos **Impacto** e **Título**. 

6.  No campo **Descrição**, forneça o seguinte: 
    -   O GUID do locatário do cliente ou o nome de domínio
    -   ID do Pedido ou ID da Assinatura
    -   Motivo do reembolso
    -   Quantidade solicitada

7.  No campo **Contato**, insira seu nome, email e número de telefone. 

8.  Se você precisar anexar um arquivo por qualquer motivo, selecione **Adicionar arquivos**. Esta etapa é opcional. 

9.  When you're finished, select **Submit**.
