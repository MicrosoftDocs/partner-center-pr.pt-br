---
title: Migrar assinaturas do Dynamics AX para o Dynamics 365 | Partner Center
ms.topic: article
ms.date: 10/29/2018
description: A Microsoft apresenta o Dynamics 365, a mais nova geração de aplicativos de negócios inteligentes que permitem que sua organização cresça, evolua e transforme-se para atender às necessidades de seus clientes e aproveitar novas oportunidades.
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: MaggiePucciEvans
ms.author: evansma
ms.localizationpriority: medium
ms.openlocfilehash: e992a3cdfc0bbb01a303a8b00bfeda3cf60d1882
ms.sourcegitcommit: ed22f6825d3af1d19385198b4d511e4b39d5e353
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/29/2018
ms.locfileid: "5797129"
---
# <a name="migrate-dynamics-ax-subscriptions-to-dynamics-365"></a>Migrar assinaturas do Dynamics AX para o Dynamics 365

**Aplicável a**

-  Partner Center

A Microsoft apresenta o Dynamics 365, a mais nova geração de aplicativos de negócios inteligentes que permitem que sua organização cresça, evolua e transforme-se para atender às necessidades de seus clientes e aproveitar novas oportunidades. Como parte do novo produto, a Microsoft apresentou novos planos de assinatura do Microsoft Dynamics para clientes em 1º de novembro de 2016, que são semelhantes, mas não idênticos aos seus planos atuais.

As instruções neste documento descrevem como provedores indiretos podem migrar as assinaturas existentes do Microsoft Dynamics AX dos clientes para o novo Microsoft Dynamics 365. As instruções também se aplicam a outros produtos da Microsoft que são atualizados para novas versões, exigindo que os provedores migrem as assinaturas dos clientes para uma nova SKU.

Os planos do Microsoft Dynamics CRM Online e AX forem desativados.  Desde 1 de julho de 2017, você não pode renovar em planos legados, e assinaturas E4 existentes não serão renovadas automaticamente quando expiram.

Quando as assinaturas CRM Online e AX terminarem, elas serão canceladas. Para garantir a continuidade dos clientes, você deve fazer a transição de clientes com assinaturas E4 vencidas para uma opção de SKU com suporte, listada abaixo. É recomendável mover os clientes para as novas assinaturas antes da data de término da assinatura anual, para evitar possíveis interrupções de serviço. 

Na página de detalhes da assinatura, o status da assinatura E4 foi alterado para "Expira em [data]" de "Renovação automática em [data]". 

Se você usar a API (CREST ou Partner Center), você pode descobrir assinaturas vencidas avaliando a data de término da assinatura juntamente com a propriedade de renovação automática = Falso. Você pode mover os clientes para um novo plano a qualquer momento. 

**Alterações de licenciamento do Microsoft Dynamics AX**

A linha de produtos Microsoft Dynamics AX foi desativada, em vigor a partir de 1º de novembro de 2016. Para saber mais sobre as novas opções de licenciamento do Dynamics 365, examine o [Guia de Licenciamento](http://download.microsoft.com/documents/dynamics/pricing/Dynamics_365_Enterprise_edition_Licensing_Guide.pdf).

 Consulte a tabela a seguir para obter detalhes sobre o mapeamento de licenças:

|**SKU desativado**   |**Dynamics 365 SKU**   |
|-------------------|:----------------------|
|Enterprise SKU|Microsoft Dynamics 365 for Unified Operations ou Microsoft Dynamics 365 Plan |
|Tarefa|MB2-717: Microsoft Dynamics 365 for Sales
|Tarefa/autoatendimento|Microsoft Dynamics 365 for Team Members|
|Dispositivo|Microsoft Dynamics 365 for Operations Device|

## <a name="microsoft-dynamics-crm-online-licensing-changes"></a>Alterações de licenciamento do Microsoft Dynamics CRM Online 

**Microsoft Dynamics CRM Online**

A partir de 1º de novembro de 2016, o plano Microsoft Dynamics CRM Online atual estará desativado. Para saber mais sobre as novas opções de licenciamento do microsoft Dynaics 365, revise o [guia de licenciamento](http://download.microsoft.com/documents/dynamics/pricing/Dynamics_365_Enterprise_edition_Licensing_Guide.pdf). Consulte [Informações importantes para clientes do CRM Online](https://go.microsoft.com/fwlink/?linkid=831667) para saber mais sobre as novas opções de licenciamento.

Consulte a tabela a seguir para obter detalhes sobre o mapeamento de licenças:

|**SKU desativado**   |**Dynamics 365 SKU**   |
|-------------------|:----------------------|
|Enterprise|Plano de engajamento do cliente Dynamics 365 Enterprise |
|Professional|Plano de engajamento de cliente do Dynamics 365 Enterprise, Dynamics 365 for Sales ou Dynamics 365 for Customer Service|
|Básico|Dynamics 365 for Team Members, Dynamics 365 for Sales, Dynamics 365 for Customer Service, or plano de engajamento de cliente Dynamics 365 Enterprise|
|Essential|Dynamics 365 for Team Member|
|Complemento do serviço de campo|Plano de envolvimento de cliente do Dynamics 365 Enterprise ou Dynamics 365 for Field Service|
|Complemento de automação de serviço de projeto|Plano de envolvimento de cliente do Dynamics 365 ou Dynamics 365 for Project Service Automation|



## <a name="transition-customers-to-new-product-plans"></a>Transição dos clientes para novos planos do produto


A Microsoft oferece continuamente novos produtos e serviços para revendedores e provedores. Nesses casos, talvez o revendedor precise fazer o upgrade dos clientes para novos serviços ou migrar as assinaturas de SKUs que serão encerradas em breve. A migração dos clientes de SKUs antigas para as mais recentes requer a seguinte sequência:

-   [Comprar a nova assinatura](#manual-subscription-migration-purchasenewsubsc);
-   [Reatribuir as licenças de usuário atuais](#manual-subscription-migration-reassignlicenses);
-   [Cancelar a assinatura antiga](#manual-subscription-migration-cancelsubscriptions).

Nos procedimentos a seguir, você migrará um cliente do Microsoft Dynamics AX ou CRM Online para o Dynamics 365.

O revendedor precisa migrar o cliente com uma assinatura existente do Dynamics AX Enterprise para o Dynamics 365 for Operations. A primeira etapa é comprar o Dynamics 365 for Operations.  Repita essas etapas para um cliente CRM Online mudando para o Microsoft Dynamics 365.

<a href="" id="purchasenewsubsc"></a>

**Comprar a nova assinatura**

1.  No menu **Partner Center** , selecione **os clientes**, selecione o cliente que você deseja mover e escolha **Adicionar assinaturas**.
2.  Selecione a assinatura que deseja comprar no catálogo (nesse caso, Dynamics 365 for Operations, Enterprise Edition), insira o número de licenças e escolha **Enviar**.

    Agora seu cliente deve ter assinaturas novas e antigas: neste exemplo, o antigo Dynamics AX Enterprise, e a nova assinatura de "destino", Dynamics 365 for Operations, Enterprise Edition.

<a href="" id="reassignlicenses"></a> A próxima etapa é reatribuir todas as licenças de usuário existentes para a nova assinatura.

**Reatribuir licenças de usuário**

1.  No menu **Partner Center** , selecione **os clientes**, selecione o cliente que você deseja mover e escolha **os usuários e licenças**. A página Usuários e Licenças do cliente será aberta.
2.  Para reatribuir licenças de usuário, selecione o usuário a ser reatribuído e selecione **Gerenciar licenças**.
3.  Na página **Gerenciar licenças**, desmarque a caixa de seleção da licença **Dynamics AX Enterprise** e selecione a licença **Dynamics 365 for Operations**.
4.  Selecione **Enviar**. Uma página de confirmação lista as novas atribuições de licença.
5.  Siga as mesmas etapas com outros usuários do cliente que precisam de reatribuição de licença.

<a href="" id="cancelsubscriptions"></a> Depois de migrar as licenças de usuário para o novo serviço, você pode cancelar com segurança a assinatura antiga no nível superior do cliente.

**Cancelar a assinatura antiga**

1.  No menu **Partner Center** , selecione **os clientes**, selecione o cliente que você deseja mover e selecione a assinatura que deseja cancelar.
2.  Na página de detalhes da assinatura, defina o **Status** da assinatura para **Suspensa**.
3.  Selecione **Enviar**.

A assinatura antiga será suspensa e a nova assinatura será ativada. A assinatura suspensa será desprovisionada automaticamente após 120 dias. O cliente não pagará custos adicionais pela assinatura antiga.

## <a name="additional-considerations"></a>Considerações adicionais


Se o cliente for migrar do Programa Open Channel para o Programa de Serviços na Nuvem para mais provisionamento de assinaturas, você também precisará migrar as assinaturas existentes dele:

-   Se o cliente tiver recebido a assinatura antiga pelo Open Channel, a migração do CSP para a nova SKU será simples.
-   Se o cliente ainda não estiver estabelecido como seu cliente, você poderá convidá-lo. Para obter informações, consulte o tópico de ajuda [Solicitar uma relação com um cliente](https://msdn.microsoft.com/en-us/library/partnercenter/mt750320.aspx).

Depois que o cliente aceitar você como seu provedor indireto, as etapas de provisionamento serão basicamente as mesmas que foram descritas acima: você compra a nova assinatura e depois atribui as licenças de usuário. A única diferença envolve o cancelamento de assinaturas antigas. Um novo provedor não pode suspender/cancelar assinaturas adquiridas por meio de outros canais. Se o cliente tiver adquirido assinaturas anteriores em outro canal de vendas, como o Open Channel, ele precisará cancelá-las por meio desse canal.

 

 



