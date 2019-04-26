---
title: Adicionar Serviços Compartilhados do Parceiro Azure | Partner Center
ms.topic: article
ms.date: 03/15/2019
description: Os Serviços Compartilhados do Parceiro Azure são um novo tipo de oferta para parceiros no programa CSP, permitindo que os parceiros adquiram assinaturas do Azure para uso próprio.
author: LauraBrenner
ms.author: labrenne
Keywords: Azure, serviços compartilhados, locatário
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: bfdb82d0698f2e0aba3f5284a53fe22010efc0da
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "62134921"
---
# <a name="add-azure-partner-shared-services"></a>Adicionar Serviços Compartilhados do Parceiro Azure

**Aplica-se a**

-  Partner Center

Os Serviços Compartilhados do Parceiro Azure são um novo tipo de oferta para parceiros no programa CSP, permitindo que os parceiros adquiram assinaturas do Azure para uso próprio.  Ele cria a oportunidade para parceiros ao usar um método uniforme para compra, acompanhamento e gerenciamento do Azure além da capacidade para consolidar seu Azure licenciamento e revenda contratos com a Microsoft. Com os Serviços Compartilhados do Parceiro Azure, agora os parceiros têm a mesma flexibilidade para usar assinaturas do Azure no CSP que eles têm nos programas Microsoft Enterprise Agreement e Web Direct, abrindo cenários como: criação de ambientes de desenvolvimento e teste, implantação de cargas de trabalho internas e hospedagem de serviços compartilhados ou aplicativos de multilocatários.  

## <a name="create-the-shared-services-tenant"></a>Criar o locatário de serviços compartilhados

1. Acesse **Configurações** > **Exibir todas as configurações** > **Serviços compartilhados**.

    ![**Configurações de conta**>**Serviços compartilhados**](images/sharedservices2.png)

2. Se você ainda não tiver um locatário de serviços compartilhados, clique em **Criar serviços compartilhados**.

    ![Criar serviços compartilhados](images/sharedservices3.png)

3. Isso cria um locatário serviços compartilhados e compra a assinatura de Serviços Compartilhados do Azure CSP para serem usados para recursos compartilhados e carga de trabalho interna.

    ![Criar o locatário e comprar a assinatura](images/sharedservices5.png)

## <a name="about-the-azure--internalshared-services-offer"></a>Sobre a oferta dos Serviços Compartilhados/Internos do Azure

- A assinatura do Azure – Serviços Compartilhados/Internos é um novo tipo de oferta do Azure no CSP acessada por meio do Partner Center que os parceiros obtém para seu próprio uso do Azure. 

- A oferta Azure - Serviços Compartilhados/Internos não está qualificada para descontos e incentivos.

- A oferta Azure - Serviços Compartilhados/Internos só pode ser aplicada ao locatário de serviços compartilhados.

- O uso principal da assinatura do Azure – Serviços Compartilhados/Internos é para que você possa usar o Azure para seus próprios fins de desenvolvimento. O locatário compartilhado que você usa para provisionar esta oferta não pode ser usado para outros serviços como o Office 365 ou estações do Dynamics. 

- Você pode cancelar a assinatura como qualquer outra assinatura. Acesse as **configurações** > **Exibir todas as configurações** > **Serviços compartilhados**. Selecione a assinatura do Azure - Serviços Compartilhados/Internos e cancele-a.

## <a name="accessing-azure-partner-shared-services-consumption-details"></a>Acessando os detalhes de consumo de Serviços Compartilhados do Parceiro Azure

Você encontrará o consumo do Azure em sua fatura do CSP e no arquivo de reconciliação. Ele será incluído como parte do item de linha do Microsoft Azure na fatura. As informações detalhadas de consumo estarão disponíveis no arquivo de reconciliação registrado em relação ao locatário que foi criado para esta oferta. 

## <a name="azure-partner-shared-services-pricing"></a>Preços dos Serviços Compartilhados do Parceiro Azure

Para ver o novo arquivo de definição de preços dos Serviços Compartilhados do Parceiro Azure, acesse **Vender** > **Preços e ofertas** e selecione a lista de preços do mês atual. Nas próximas semanas, também será lançada uma API de tabela de tarifas específica.

## <a name="marketplace-offers-and-azure-partner-shared-services"></a>As ofertas do Marketplace e serviços compartilhados do parceiro do Azure

A partir de 1º de março de 2019, o Azure Partner Shared Services (APSS) não oferece suporte a ofertas do Marketplace.   

|**Suporte do Marketplace**   |**APSS compatível antes de 1 de março de 2019**|**Após 1 de março de 2019**|
|---------------------------|:----------------------------|:-------------------|
|Traga sua própria licença (BYOL) e serviços gratuitos   | Sim   | Não|
|Outras ofertas do marketplace de terceiros   | Não   |Não|


Parceiros que tem BYOL ou livre serviços implantados usando APSS não serão afetados; No entanto após 1 de março de 2019 eles não poderão adquirir nova BYOL ou serviços gratuitos. 

Para tirar proveito de todo o catálogo de ofertas do Marketplace disponíveis (não apenas serviços gratuitos e BYOL) é recomendável que os parceiros CSP implantem serviços compartilhados usando assinaturas web direct do Azure.  Parceiros CSP que implantaram 3ª parte BYOL e liberam recursos do Marketplace do serviço anteriormente e deseja continuar a usá-los e implantar mais 3ª parte ofertas são incentivadas a migrar a assinatura APSS para diretos da web [migrando Assinaturas do Azure existentes](https://docs.microsoft.com/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions).

Parceiros que planejam continuar a usar assinatura APSS após 1º de março de 2019 e deseja implantar novo participante 3ª [serviços BYOL](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) ou serviços gratuitos, siga as instruções de ISVs para implantá-las em suas assinaturas APSS.

