---
title: Usar Partner Center Analytics para Power BI
ms.topic: article
ms.date: 05/19/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como exibir seus dados empresariais usando o aplicativo Análise do Partner Center para Power BI (para parceiros diretos no programa Provedor de Soluções na Nuvem (CSP).
fwlink: https://go.microsoft.com/fwlink/?linkid=852581
author: v-sumukh
ms.author: v-sumukh
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 95eb018a3284d2de98c0ce6a9cd0ce6299d5571a
ms.sourcegitcommit: 4118de5cf55d1bd618ecca13c1b2ec59d80f43db
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2021
ms.locfileid: "112564974"
---
# <a name="view-your-business-data-with-the-partner-center-analytics-app-for-microsoft-power-bi"></a>Visualize seus dados de negócio com o aplicativo de análise do Partner Center para Microsoft Power BI



**Funções apropriadas**: Administrador global | Administrador de gerenciamento de usuários | Agente de vendas | Agente administrativo

## <a name="view-your-business-data"></a>Visualize seus dados de negócio

Obter uma representação visual dos dados de negócios com o aplicativo Partner Center Analytics para Microsoft Power BI, incluindo:

- Crescimento de sua base de clientes, assinaturas e licenças

- O uso de produtos do Office 365, Microsoft Dynamics e Microsoft Azure

- As unidades de consumo diário de cada recurso limitado em cada assinatura do Azure nos últimos 60 dias

- Custo estimado (com base na tabela de tarifas mais recente)

- Capacidade de exportar conjuntos de dados e criar relatórios personalizados, incluindo por cliente.

### <a name="about-the-partner-center-analytics-app-preview-release"></a>Sobre a versão de visualização do aplicativo de análises do Partner Center

- Este aplicativo é destinado somente a parceiros diretos no programa Provedor de Soluções na Nuvem (CSP). Outros parceiros no CSP (revendedores indiretos, por exemplo) não poderão se conectar.

- Todos os custos estimados são pré-taxados na cobrança/ dados da fatura, e não são vinculados legalmente. Os Custos estimados destinam-se a ser usados somente para percepções.

- As informações do cliente são baseadas em assinaturas. Todos os clientes para os que você criou contas recentemente, mas que ainda não têm assinaturas, não estão incluídos em contagens.

- Os custos estimados baseiam-se na tabela de taxa mais recente, que baseia-se nos preços CSP.

- Os dias são dias calendários.

### <a name="business-insights-report"></a>Relatório de ideias de negócios

- **Locatários do** cliente: número de locatários Azure Active Directory (Azure AD) distintos de clientes que compraram assinaturas

- **Novo (últimos 30 dias)**: Novos clientes comprando pelo menos uma assinatura nos últimos 30 dias

- **Variação (últimos 30 dias)**: clientes sem assinaturas "ativas", "em carência" ou "desabilitadas"

- **Novo (últimas 24 horas)**: Novos clientes comprando pelo menos uma assinatura nos últimas 24 horas

- **Custo mensal estimado nos últimos 12 meses**: Tendência mês a mês do valor pré-taxado em dólar estimado para a fatura agregado mensalmente durante o período dos últimos 12 meses

- **Custo mensal por produto estimado nos últimos 12 meses**: Produtos vendidos classificados pelo valor pré-taxado em dólar estimado para a fatura agregado mensalmente durante o período dos últimos 12 meses. Esse status indica os principais produtos que trazem a maior parte da receita.

- **Clientes nos últimos 12 meses**: Tendência mês a mês de novos clientes e clientes de variação agregados mensalmente durante o período de últimos 12 meses

- **Custo mensal por cliente estimado nos últimos 12 meses**: Clientes classificados pelo valor pré-taxado em dólar estimado para a fatura agregado mensalmente durante o período dos últimos 12 meses. Esse status indica os principais clientes que trazem a maior parte da receita.

- **Contagem de cliente por produto**: Produtos vendidos classificados por clientes associados. Esse status indica os principais produtos vendidos para a maioria dos clientes.

### <a name="subscription-insights-report"></a>Relatório de ideias de assinatura

- **Status da assinatura:**

- Ativo: assinaturas que pertencem ao estado "ativo" ou "em carência"

  - Suspenso: assinaturas que pertencem ao estado "desabilitado"

  - Des provisionado: assinaturas que pertencem ao status "des provisionado" ou "expirado"

- **Status de expiração**:

  - Expirado: Assinaturas que já expiraram (onde a data de término da assinatura está no passado)

  - Expiram após 30 dias: Assinaturas que expirarão após 30 dias (onde data de término da assinatura é depois dos próximos 30 dias)

  - Expiram em 30 dias: Assinaturas que expirarão nos próximos 30 dias (onde data de término da assinatura é entre hoje e os próximos 30 dias)

- **Total de assinaturas:** assinaturas no status "ativo", "em carência" ou "desabilitado"

- **Novo (últimos 30 dias)**: Novas assinaturas compradas por clientes nos últimos 30 dias

- **Novo (últimas 24 horas)**: Novas assinaturas compradas por clientes nas últimas 24 horas

- **Expira em 30 dias**: Assinaturas que expirarão nos próximos 30 dias

- **Variação (últimos 30 dias)**: assinaturas que foram des provisionadas ou suspensas (desabilitadas) nos últimos 30 dias

- **Distribuição por tipos de assinatura:**% de distribuição do total de assinaturas por tipo de assinatura baseado em licença e com base no uso

- **Contagem de assinatura ativa por produto**: Produtos vendidos classificados por contagem de assinaturas ativas

- **Assinaturas nos últimos 12 meses**: Tendência mês a mês de novas assinaturas e assinaturas com rotatividade agregadas mensalmente durante o período de últimos 12 meses

- **Detalhes da assinatura do** cliente: exibição detalhada dos clientes, assinaturas e ofertas

### <a name="license-insights-report"></a>Relatório de ideias de licença:

- **Total de licenças:** número total de licenças agregadas em todas as assinaturas baseadas em licença

- **Novo (últimos 30 dias)**: Adição de licenças nos últimos 30 dias

- **Rotatividade (últimos 30 dias)**: Redução de licenças nos últimos 30 dias

- **Novo (últimas 24 horas)**: Adição de licenças nas últimas 24 horas

- **Licenças nos últimos 90 dias**: Tendência mês a mês de adições e reduções de licença agregadas mensalmente durante o período dos últimos 90 dias

- **Contagem de licença ativa por produto**: Produtos vendidos classificados por contagem de licenças ativas

- **Contagem de licenças ativas por cliente:** clientes classificaram por contagem de licenças ativas

- Detalhes do evento de licença do cliente nos últimos **90** dias: exibição detalhada dos clientes, assinaturas e eventos de assinatura, incluindo data do evento, nome do evento, quantidade e alteração na quantidade.

### <a name="licenses-usage-report"></a>Relatório de uso de licenças:

- **Licenças atribuídas por produto**: Produtos vendidos classificados por contagem de atribuição

- **Licenças em uso por produto**: Produtos vendidos classificados por contagem de uso de licença

- **Distribuição de cliente de licenças atribuídas**: distribuição % do total de clientes desfeitos em classificações de faixas de 20% por % de atribuição de licença

- **Distribuição de cliente de licenças em uso**: distribuição % do total de clientes desfeitos em classificações de faixas de 20% por % de uso de licença

- **Licenças atribuídas pelo cliente**: Visualização detalhada de licenças vendidas e licenças atribuídas por cliente e produto

- **Licenças em uso por cliente**: Visualização detalhada de licenças em uso por cliente e produto

### <a name="azure-insights-report"></a>Relatório de ideias do Azure:

- Clientes baseados em uso nos últimos **12** meses: tendência mês a mês de novos clientes baseados em uso e clientes baseados em uso rotativos agregados mensalmente ao longo do período dos últimos 12 meses

- Assinaturas baseadas em uso nos últimos **12** meses: tendência mensal de novas assinaturas baseadas em uso e assinaturas baseadas em uso rotativas agregadas mensalmente durante o período dos últimos 12 meses

- Custo estimado de uso pelo cliente nos últimos **60** dias: clientes baseados em uso classificaram pelo valor estimado em dinheiro da fatura pré-fiscal agregada ao longo do período dos últimos 60 dias. Esse status indica os principais clientes baseados em uso que trazem a maior parte da receita

- Custo estimado de uso por categoria nos últimos **60** dias: categorias de medidores de assinaturas baseadas em uso, classificação pelo valor estimado em dinheiro da fatura pré-fiscal agregada ao longo do período dos últimos 60 dias.

- Custo estimado de uso por assinatura nos últimos **60** dias: assinaturas baseadas em uso pelo valor estimado em dinheiro da fatura pré-fiscal agregada ao longo do período dos últimos 60 dias.

- **Custos estimados de uso de cliente por orçamento de gastos**: Clientes classificados por percentual de seu orçamento de gastos com uso atual excedendo o limite (100%).

### <a name="azure-resource-usage-report"></a>Relatório de uso de recurso Azure:

- **Uso de recursos do Azure** por dia para o período selecionado: unidades de consumo diário para cada recurso limitado em cada assinatura baseada em uso para o período selecionado nos últimos 60 dias.

- Custo de uso estimado dos recursos do **Azure** para o período selecionado: custo estimado com base no cartão de taxa mais recente para cada recurso limitado em cada assinatura baseada em uso para o período selecionado nos últimos 60 dias. 

## <a name="next-steps"></a>Próximas etapas

- [Visão geral do aplicativo de análise do Partner Center para Power BI](power-bi-app-for-direct-partners.md)

- [Instalar e visualizar o aplicativo Análise do Partner Center para Microsoft Power BI](power-bi-app-for-direct-partners-install.md)
