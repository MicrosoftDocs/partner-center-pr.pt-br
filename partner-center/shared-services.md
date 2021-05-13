---
title: Adicionar os Serviços Compartilhados com Parceiros do Azure
description: Use Serviços Compartilhados com Parceiros do Azure para comprar assinaturas do Azure para seu próprio uso e ter um método uniforme para comprar, acompanhar e gerenciar o Azure.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 11/11/2020
ms.openlocfilehash: 929907c7c6f238fb84a13622227534797f0ac949
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855328"
---
# <a name="add-azure-partner-shared-services-so-partners-can-buy-azure-subscriptions-for-their-own-use"></a>Adicione Serviços Compartilhados com Parceiros do Azure para que os parceiros possam comprar assinaturas do Azure para uso próprio

**Funções apropriadas:** administrador global | Agente administrador | Agente de vendas

Os Serviços Compartilhados do Parceiro Azure são um novo tipo de oferta para parceiros no programa CSP, permitindo que os parceiros adquiram assinaturas do Azure para uso próprio.  Ele gera a oportunidade para os parceiros usarem um método uniforme de compra, rastreamento e gerenciamento do Azure, além da capacidade de consolidar seus contratos de licenciamento e revenda do Azure com a Microsoft. Com o Serviços Compartilhados com Parceiros do Azure, os parceiros agora têm a mesma flexibilidade para usar assinaturas do Azure no CSP como fazem nos programas Microsoft Enterprise Agreement e Web Direct, abrindo cenários como: criar ambientes de desenvolvimento e teste, implantar cargas de trabalho internas e hospedar serviços compartilhados ou aplicativos multisatário.  

## <a name="create-the-shared-services-tenant"></a>Criar o locatário de serviços compartilhados

1. Vá para **Configurações Configurações** da conta Serviços  >  **compartilhados.**  >  

   :::image type="content" source="images/sharedservices2.png" alt-text="Configurações de conta > serviços compartilhados":::

2. Se você ainda não tiver um locatário de serviços compartilhados, clique em **Criar serviços compartilhados**.

   :::image type="content" source="images/sharedservices3.png" alt-text="Criar serviços compartilhados":::

3. Isso cria um locatário serviços compartilhados e compra a assinatura de Serviços Compartilhados do Azure CSP para serem usados para recursos compartilhados e carga de trabalho interna.

   :::image type="content" source="images/sharedservices5.png" alt-text="Criar o locatário e comprar a assinatura":::

## <a name="about-the-azure--internalshared-services-offer"></a>Sobre a oferta dos Serviços Compartilhados/Internos do Azure

- A Azure - Serviços Compartilhados/Internos assinatura é um novo tipo de oferta do Azure no CSP acessado por meio Partner Center que os parceiros usam para seu próprio uso do Azure.

- Serviços Compartilhados com Parceiros do Azure assinaturas são qualificadas e podem ser usadas para comprar RIs.

- A oferta Azure - Serviços Compartilhados/Internos só pode ser aplicada ao locatário de serviços compartilhados.

- O principal uso para a assinatura Azure - Serviços Compartilhados/Internos é para que você possa usar o Azure para suas próprias finalidades de desenvolvimento. O locatário compartilhado usado para provisionar essa oferta não pode ser usado para outros serviços, como licenças do Office 365 ou dynamics.

- Você pode cancelar a assinatura como qualquer outra assinatura. Vá para as **configurações Exibir tudo**  >  **Serviços**  >  **compartilhados.** Selecione a assinatura do Azure - Serviços Compartilhados/Internos e cancele-a.

## <a name="accessing-azure-partner-shared-services-consumption-details"></a>Acessando os detalhes de consumo de Serviços Compartilhados do Parceiro Azure

Você encontrará o consumo do Azure em sua fatura do CSP e no arquivo de reconciliação. Ele será incluído como parte do item de linha do Microsoft Azure na fatura. As informações detalhadas de consumo estarão disponíveis no arquivo de reconciliação registrado em relação ao locatário que foi criado para esta oferta.

## <a name="azure-partner-shared-services-pricing"></a>Preços dos Serviços Compartilhados do Parceiro Azure

Para ver o novo arquivo de preços para Serviços Compartilhados com Parceiros do Azure, acesse Vender Preços e ofertas e selecione a  >   lista de preços do mês atual. Nas próximas semanas, também será lançada uma API de tabela de tarifas específica.

## <a name="marketplace-offers-and-azure-partner-shared-services"></a>Ofertas e Serviços Compartilhados com Parceiros do Azure

A partir de 1º de março de 2019, o Serviços Compartilhados com Parceiros do Azure (APSS) não dá mais suporte a ofertas do Marketplace.

|**Suporte do Marketplace**   |**APSS com suporte antes de 1º de março de 2019**|**Após 1º de março de 2019**|
|---------------------------|:----------------------------|:-------------------|
|Traga sua própria licença (BYOL) e serviços gratuitos   | Sim   | Não|
|Outras ofertas do marketplace de terceiros   | Não   |Não|

Os parceiros que têm BYOL ou serviços gratuitos implantados usando o APSS não serão afetados; no entanto, após 1º de março de 2019, eles não poderão comprar novos byol ou serviços gratuitos.

Para aproveitar o catálogo completo de ofertas do Marketplace disponíveis (não apenas BYOL e serviços gratuitos), recomendamos que os parceiros CSP implantem serviços compartilhados usando assinaturas diretas da Web do Azure.  Os parceiros do CSP que implantaram byOL de terceiros e recursos de serviço gratuitos do Marketplace anteriormente e desejam continuar usando-os e implantar mais ofertas de terceiros são incentivados a migrar a assinatura do APSS para Migração direta da Web para [Assinaturas existentes do Azure.](/azure/cloud-solution-provider/migration/migration#migrating-existing-azure-subscriptions)

Os parceiros, que planejam continuar usando a assinatura do APSS após 1º de março de 2019 e desejam implantar novos serviços [BYOL](https://azuremarketplace.microsoft.com/marketplace/apps?filters=byol) de terceiros ou serviços gratuitos, podem seguir as instruções dos ISVs para implantá-los em suas assinaturas do APSS.

## <a name="next-steps"></a>Próximas etapas

- [Vender assinaturas de software por meio do CSP](csp-software-subscriptions.md)