---
title: Adicionar Serviços Compartilhados do Parceiro Azure | Partner Center
ms.topic: article
ms.date: 03/15/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Use os serviços compartilhados do parceiro do Azure para comprar assinaturas do Azure para seu próprio uso e para ter um método uniforme de compra, acompanhamento e gerenciamento do Azure.
author: LauraBrenner
ms.author: labrenne
Keywords: Azure, serviços compartilhados, locatário
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 2d6c51ceb9151298f21bb0ebfd696e57bd8d13fb
ms.sourcegitcommit: 9a628b8fc73d4db995b7cb42faaf4d6c3b573e45
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/09/2019
ms.locfileid: "74943449"
---
# <a name="add-azure-partner-shared-services"></a>Adicionar os Serviços Compartilhados com Parceiros do Azure

**Aplica-se a**

-  Partner Center

Os Serviços Compartilhados do Parceiro Azure são um novo tipo de oferta para parceiros no programa CSP, permitindo que os parceiros adquiram assinaturas do Azure para uso próprio.  Ele cria a oportunidade para que os parceiros usem um método uniforme para comprar, controlar e gerenciar o Azure além da capacidade de consolidar o licenciamento do Azure e revender contratos com a Microsoft. Com os Serviços Compartilhados do Parceiro Azure, agora os parceiros têm a mesma flexibilidade para usar assinaturas do Azure no CSP que eles têm nos programas Microsoft Enterprise Agreement e Web Direct, abrindo cenários como: criação de ambientes de desenvolvimento e teste, implantação de cargas de trabalho internas e hospedagem de serviços compartilhados ou aplicativos de multilocatários.  

## <a name="create-the-shared-services-tenant"></a>Criar o locatário de serviços compartilhados

1. Acesse **Configurações** > **Exibir todas as configurações** > **Serviços compartilhados**.

    ![**Configurações de conta**>**Serviços compartilhados**](images/sharedservices2.png)

2. Se você ainda não tiver um locatário de serviços compartilhados, clique em **Criar serviços compartilhados**.

    ![Criar serviços compartilhados](images/sharedservices3.png)

3. Isso cria um locatário serviços compartilhados e compra a assinatura de Serviços Compartilhados do Azure CSP para serem usados para recursos compartilhados e carga de trabalho interna.

    ![Criar o locatário e comprar a assinatura](images/sharedservices5.png)

## <a name="about-the-azure--internalshared-services-offer"></a>Sobre a oferta dos Serviços Compartilhados/Internos do Azure

- A assinatura Azure-Serviços Compartilhados/Internos é um novo tipo de oferta do Azure no CSP acessado por meio do Partner Center que os parceiros obtêm para seu próprio uso do Azure. 

- A oferta de Azure-Serviços Compartilhados/Internos não está qualificada para descontos e incentivos.

- A oferta Azure - Serviços Compartilhados/Internos só pode ser aplicada ao locatário de serviços compartilhados.

- O uso principal para a assinatura Azure-Serviços Compartilhados/Internos é para que você possa usar o Azure para suas próprias finalidades de desenvolvimento. O locatário compartilhado que você usa para provisionar esta oferta não pode ser usado para outros serviços como o Office 365 ou estações do Dynamics. 

- Você pode cancelar a assinatura como qualquer outra assinatura. Acesse as **configurações** > **Exibir todas as configurações** > **Serviços compartilhados**. Selecione a assinatura do Azure - Serviços Compartilhados/Internos e cancele-a.

## <a name="accessing-azure-partner-shared-services-consumption-details"></a>Acessando os detalhes de consumo de Serviços Compartilhados do Parceiro Azure

Você encontrará o consumo do Azure em sua fatura do CSP e no arquivo de reconciliação. Ele será incluído como parte do item de linha do Microsoft Azure na fatura. As informações detalhadas de consumo estarão disponíveis no arquivo de reconciliação registrado em relação ao locatário que foi criado para esta oferta. 

## <a name="azure-partner-shared-services-pricing"></a>Preços dos Serviços Compartilhados do Parceiro Azure

Para ver o novo arquivo de definição de preços dos Serviços Compartilhados do Parceiro Azure, acesse **Vender** > **Preços e ofertas** e selecione a lista de preços do mês atual. Nas próximas semanas, também será lançada uma API de tabela de tarifas específica.

## <a name="marketplace-offers-and-azure-partner-shared-services"></a>Ofertas do Marketplace e serviços compartilhados de parceiros do Azure

A partir de 1º de março de 2019, o APSS (serviços compartilhados de parceiros do Azure) não oferece mais suporte a ofertas do Marketplace.   

|**Suporte do Marketplace**   |**APSS com suporte antes de 1º de março de 2019**|**Após 1º de março de 2019**|
|---------------------------|:----------------------------|:-------------------|
|BYOL (traga sua própria licença) e serviços gratuitos   | Sim   | Não|
|Outras ofertas de Marketplace de terceiros   | Não   |Não|


Os parceiros que têm serviços BYOL ou gratuitos implantados usando o APSS não serão afetados; no entanto, após 1º de março de 2019, eles não poderão comprar novos BYOL ou serviços gratuitos. 

Para aproveitar o catálogo completo das ofertas do Marketplace disponíveis (não apenas BYOL e serviços gratuitos), recomendamos que os parceiros CSP implantem serviços compartilhados usando assinaturas do Azure Direct Web.  Os parceiros CSP que implantaram BYOL de terceiros e recursos de serviço gratuitos do Marketplace anteriormente e desejavam continuar a usá-los e implantar mais ofertas de terceiros são incentivados a migrar a assinatura do APSS para a Web Direct [migrando assinaturas existentes do Azure](https://docs.microsoft.com/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions).

Os parceiros, que planejam continuar usando a assinatura do APSS após 1º de março de 2019 e desejam implantar novos [serviços de BYOL](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) de terceiros ou serviços gratuitos, podem seguir as instruções de ISVs para implantá-los em suas assinaturas do APSS.

