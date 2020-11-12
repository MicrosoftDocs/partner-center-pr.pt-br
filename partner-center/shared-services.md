---
title: Adicionar os Serviços Compartilhados com Parceiros do Azure
description: Use os serviços compartilhados do parceiro do Azure para comprar assinaturas do Azure para seu próprio uso e para ter um método uniforme de compra, acompanhamento e gerenciamento do Azure.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 11/11/2020
ms.openlocfilehash: 93ee3e142bf11c3b329fd27ec7320b93aea780b8
ms.sourcegitcommit: cc30a06abe55b9da32177a24e74bfd6fc7d8bbb9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/12/2020
ms.locfileid: "94532031"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a>Adicionar serviços compartilhados de parceiros do Azure para que os parceiros possam comprar assinaturas do Azure para seu próprio uso

 
**Funções apropriadas**

- Administrador global
- Agente administrativo
- Agente de vendas

Os Serviços Compartilhados do Parceiro Azure são um novo tipo de oferta para parceiros no programa CSP, permitindo que os parceiros adquiram assinaturas do Azure para uso próprio.  Ele gera a oportunidade para os parceiros usarem um método uniforme de compra, rastreamento e gerenciamento do Azure, além da capacidade de consolidar seus contratos de licenciamento e revenda do Azure com a Microsoft. Com os serviços compartilhados de parceiros do Azure, os parceiros agora têm a mesma flexibilidade para usar as assinaturas do Azure no CSP, como no Microsoft Enterprise Agreement e nos programas Web Direct, abrindo cenários como: criar ambientes de desenvolvimento e teste, implantar cargas de trabalho internas e hospedar serviços compartilhados ou aplicativos multilocatários.  

## <a name="create-the-shared-services-tenant"></a>Criar o locatário de serviços compartilhados

1. Vá para **configurações**  >  **configurações de conta**  >  **serviços compartilhados**.

   :::image type="content" source="images/sharedservices2.png" alt-text="Configurações de conta > serviços compartilhados":::

2. Se você ainda não tiver um locatário de serviços compartilhados, clique em **Criar serviços compartilhados**.

   :::image type="content" source="images/sharedservices3.png" alt-text="Criar serviços compartilhados":::

3. Isso cria um locatário serviços compartilhados e compra a assinatura de Serviços Compartilhados do Azure CSP para serem usados para recursos compartilhados e carga de trabalho interna.

   :::image type="content" source="images/sharedservices5.png" alt-text="Criar o locatário e comprar a assinatura":::

## <a name="about-the-azure--internalshared-services-offer"></a>Sobre a oferta dos Serviços Compartilhados/Internos do Azure

- A assinatura Azure-Serviços Compartilhados/Internos é um novo tipo de oferta do Azure no CSP acessado por meio do Partner Center que os parceiros obtêm para seu próprio uso do Azure.

- Azure-Serviços Compartilhados/Internos oferta é elegível para descontos e incentivos.  As assinaturas dos serviços compartilhados do parceiro do Azure são elegíveis e podem ser usadas para comprar o RIs.

- A oferta Azure - Serviços Compartilhados/Internos só pode ser aplicada ao locatário de serviços compartilhados.

- O uso principal para a assinatura Azure-Serviços Compartilhados/Internos é para que você possa usar o Azure para suas próprias finalidades de desenvolvimento. O locatário compartilhado que você usa para provisionar essa oferta não pode ser usado para outros serviços, como o Office 365 ou as licenças do Dynamics.

- Você pode cancelar a assinatura como qualquer outra assinatura. Vá para as **configurações**  >  **Exibir todas as configurações**  >  **serviços compartilhados**. Selecione a assinatura do Azure - Serviços Compartilhados/Internos e cancele-a.

## <a name="accessing-azure-partner-shared-services-consumption-details"></a>Acessando os detalhes de consumo de Serviços Compartilhados do Parceiro Azure

Você encontrará o consumo do Azure em sua fatura do CSP e no arquivo de reconciliação. Ele será incluído como parte do item de linha do Microsoft Azure na fatura. As informações detalhadas de consumo estarão disponíveis no arquivo de reconciliação registrado em relação ao locatário que foi criado para esta oferta.

## <a name="azure-partner-shared-services-pricing"></a>Preços dos Serviços Compartilhados do Parceiro Azure

Para ver o novo arquivo de preços dos serviços compartilhados do parceiro do Azure, vá para **vender**  >  **preços e ofertas** e selecione a lista de preços do mês atual. Nas próximas semanas, também será lançada uma API de tabela de tarifas específica.

## <a name="marketplace-offers-and-azure-partner-shared-services"></a>Ofertas do Marketplace e serviços compartilhados de parceiros do Azure

A partir de 1º de março de 2019, o APSS (serviços compartilhados de parceiros do Azure) não oferece mais suporte a ofertas do Marketplace.

|**Suporte do Marketplace**   |**APSS com suporte antes de 1º de março de 2019**|**Após 1º de março de 2019**|
|---------------------------|:----------------------------|:-------------------|
|BYOL (traga sua própria licença) e serviços gratuitos   | Sim   | Não|
|Outras ofertas de Marketplace de terceiros   | Não   |Não|

Os parceiros que têm serviços BYOL ou gratuitos implantados usando o APSS não serão afetados; no entanto, após 1º de março de 2019, eles não poderão comprar novos BYOL ou serviços gratuitos.

Para aproveitar o catálogo completo de ofertas do Marketplace disponíveis (não apenas BYOL e serviços gratuitos), recomendamos que os parceiros CSP implantem serviços compartilhados usando assinaturas do Azure Direct Web.  Os parceiros CSP que implantaram BYOL de terceiros e recursos de serviço gratuitos do Marketplace anteriormente e desejavam continuar a usá-los e implantar mais ofertas de terceiros são incentivados a migrar a assinatura APSS para a Web Direct [migrando assinaturas do Azure existentes](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions).

Os parceiros, que planejam continuar usando a assinatura do APSS após 1º de março de 2019 e desejam implantar novos [serviços de BYOL](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) de terceiros ou serviços gratuitos, podem seguir as instruções de ISVs para implantá-las em suas assinaturas do APSS.

## <a name="next-steps"></a>Próximas etapas

- [Vender assinaturas de software por meio do CSP](csp-software-subscriptions.md)