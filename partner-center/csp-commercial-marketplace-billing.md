---
title: Cobrança de produtos do Marketplace comercial
ms.topic: article
ms.date: 05/12/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como a cobrança funciona para produtos SaaS de ISV ou assinaturas adquiridas para clientes do Marketplace comercial no Partner Center.
author: LauraBrenner
ms.author: labrenne
keywords: assinaturas, produtos, compras, Marketplace, terceiros, ISV, cobrança, faturas, reconciliação, arquivo reconhecimento
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 9672850b699a2660f646ede5250e52298f5522cd
ms.sourcegitcommit: 093039319fab2a44ab147159bc4be832f1330d57
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/14/2020
ms.locfileid: "83394161"
---
# <a name="billing-for-commercial-marketplace-products-and-subscriptions-in-partner-center"></a>Cobrança de produtos e assinaturas do Marketplace comercial no Partner Center

**Aplica-se a**

- Partner Center
- Parceiros no programa CSP

**Funções apropriadas**

- Administrador global
- Administrador de cobrança

Como um parceiro no programa CSP, você pode usar o Partner Center para comprar produtos SaaS baseados em licença de editores ISV no mercado comercial. Depois de fazer isso, você pode acessar uma fatura para esses tipos de compras. O período de cobrança começa no primeiro dia do mês do calendário e termina no último dia do mês do calendário. As notas fiscais são disponibilizadas no oitavo dia do mês seguinte.

Você pode acessar as faturas no [painel](https://partner.microsoft.com/dashboard/) do Partner Center ou usando as [APIs do Partner Center](https://docs.microsoft.com/partner-center/develop/).

Os parceiros no programa CSP são cobrados pelas soluções do ISV Commercial Marketplace adquiridas para um cliente quando compram esses produtos da central de parceiros ou da portal do Azure (usando o locatário do Azure do cliente antes, adquirido pelo CSP).

>[!NOTE]
>Se os clientes usam seu próprio locatário do Azure AD (não adquirido de um parceiro no programa CSP), os clientes também podem optar por comprar sua própria solução de SaaS de ISV diretamente do ([Microsoft AppSource](https://appsource.microsoft.com/) ou [do Azure Marketplace](https://azuremarketplace.microsoft.com/)). Se fizerem isso, eles receberão sua própria conta diretamente da Microsoft. Da mesma forma, se um parceiro no programa CSP vender uma assinatura do Azure ou o novo plano do Azure para o cliente e conceder ao cliente (ou revendedor indireto) o [acesso baseado em função](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles) a esse locatário (atribuindo qualquer função ao cliente além do **leitor**), esse cliente (ou revendedor indireto) também poderá adquirir ofertas do Marketplace comercial sem aprovação prévia ou notificação ao parceiro CSP Nesses casos, a Microsoft não notificará diretamente os parceiros no programa CSP sobre as compras feitas por seus clientes. No entanto, a Microsoft oferece um mecanismo de [Azure monitor](https://docs.microsoft.com/azure/azure-monitor/platform/alerts-activity-log) opcional que você pode usar para definir alertas ou notificações sobre a atividade em uma assinatura do Azure.

## <a name="access-billing-information-for-commercial-marketplace-products"></a>Acessar informações de cobrança para produtos do Marketplace comercial

O administrador global ou de cobrança da sua empresa receberá um email quando a fatura estiver pronta para ser exibida. Para acessar a última nota fiscal e o arquivo de reconciliação para compras de produtos do Marketplace comercial:

1. Entre no [Painel](https://partner.microsoft.com/dashboard/) do Partner Center.

2. No menu do Partner Center, selecione **Cobrança**. 

    Você verá duas guias na parte superior da página de cobrança: compras **recorrentes** e **recorrentes e de uso único**. Cada guia permite que você acesse arquivos de reconhecimento (fatura e reconciliação) para diferentes produtos do Marketplace:

    - Guia **recorrente** : mostra a fatura e os arquivos de reconciliação para assinaturas relacionadas ao Office 365, Microsoft 365, Dynamics 365, Azure Active Directory, PowerBI Pro e Microsoft Azure.

    - Guia **compras recorrentes e de uso único** : mostra a fatura e os arquivos de reconciliação do plano do Azure, reservas do Azure, produtos de software e Marketplace comercial.
  
3. Selecione a guia **compras recorrentes e de uso único** . Se você comprou assinaturas de um cliente em uma moeda diferente, verá uma guia para cada moeda. Você pode fazer algumas coisas fr: om esta página:

    - Para ver a última nota fiscal e o arquivo de reconciliação, selecione **Nota Fiscal** ou **arquivo de reconciliação**. (Se desejar, você também pode acessar os dados de arquivo de nota fiscal e reconhecimento mais recentes usando as [APIs do Partner Center](https://docs.microsoft.com/partner-center/develop/).

    - Para ver os arquivos de notas fiscais e reconhecimento anteriores, expanda a linha de **histórico de cobrança** abaixo.

    - Para verificar o saldo da conta ou a cobrança estimada a qualquer momento com base na atividade da conta mais recente, selecione um link sob o título **estimativas** .  

    >[!NOTE]
    > Quando publicarmos sua fatura no oitavo dia do mês, ela incluirá impostos e quaisquer outros encargos e créditos aplicáveis. Isso significa que o valor final devido pode ser diferente do que você vê durante o período de cobrança.

## <a name="more-about-invoices-and-recon-files-for-commercial-marketplace-products"></a>Mais informações sobre notas fiscais e arquivos reconhecimento para produtos do Marketplace comercial

Esta seção oferece mais informações sobre faturas e arquivos de reconciliação para assinaturas SaaS do Marketplace comercial adquiridas para clientes de editores de ISVs de terceiros.

Quando você seleciona **compras recorrentes e de uso único** da opção de **cobrança** no menu do Partner Center, você tem acesso a faturas e a arquivos de reconciliação para encargos relacionados às compras da Microsoft (de terceiros) e ISV (terceiros). Essas compras podem estar associadas a:

- Assinaturas de SaaS (de editores da Microsoft ou ISV)

- Plano do Azure

- Reservas do Azure

- Outros softwares baseados em assinatura (de editores da Microsoft ou ISV)

Exemplos dessas compras podem incluir o software SUSE Linux (uma assinatura de software) ou uma assinatura de produto SaaS do Azure ISV.

>[!NOTE]
> Para obter mais informações sobre como ler arquivos de nota fiscal e reconhecimento, consulte também [visão geral da cobrança](billing.md).

### <a name="tips-on-reading-your-invoice"></a>Dicas sobre como ler sua fatura

Ao comprar um produto SaaS baseado em licença de um Publicador ISV de terceiros, você verá apenas os encargos da taxa de licença em sua fatura. Isso é verdadeiro mesmo quando o produto SaaS do ISV usa (ou consome) recursos de infraestrutura subjacentes do Azure. Isso ocorre porque os encargos de uso de infraestrutura do Azure do seu cliente para o produto SaaS de um ISV são cobrados diretamente para o ISV. (Os ISVs verão os encargos de consumo do Azure associados em seu próprio arquivo de reconciliação de faturas com classificação diária de uso do Azure.)

Sua fatura conterá várias páginas:

- **Página 1 da fatura:** Contém uma visão geral resumida dos detalhes de cobrança do parceiro do programa CSP. Isso inclui um resumo de encargos para o período de cobrança, um número de nota fiscal, termos de pagamento (líquido 60 dias) e métodos de pagamento de cobrança para pagar por fio ou por cheque.

- **Página 2 (e todas as páginas subsequentes) da fatura:** Detalhes de cobranças de compras de terceiros e compras de terceiros (baseadas em licença) de terceiros do Marketplace comercial. Você pode identificar compras baseadas em licença do ISV pela linha do **Publicador** abaixo de cada nome de produto. O arquivo de reconciliação associado oferece mais detalhes de cobrança para encargos específicos da fatura.

- **Página final da fatura:** Se você foi cobrado por produtos do Marketplace baseados em licença de um ISV, essa página final exibirá mais detalhes sobre o nome e o endereço do fornecedor ISV.

### <a name="tips-on-reading-your-reconciliation-file"></a>Dicas sobre como ler seu arquivo de reconciliação

O arquivo de reconciliação de **compras única e recorrente** contém várias colunas com detalhes adicionais que são mapeados para os encargos em sua fatura. A coluna **PublisherName** mostra se a compra é da Microsoft ou de um Publicador ISV de terceiros.

Alguns encargos em seu arquivo de reconciliação podem aparecer com um custo de $0. Isso pode ser devido a uma oferta de "avaliação gratuita" do ISV (geralmente 30 ou 60 dias) ou uma oferta traga sua própria licença.

No caso de ofertas de avaliação gratuitas do ISV:

- O período de avaliação gratuita aborda o custo do produto SaaS baseado em licença do ISV durante esse tempo. Você também não será cobrado pelo uso da infraestrutura do Azure associada do produto SaaS.  No entanto, se você estiver usando uma oferta de ISV baseada em uso, a avaliação gratuita não incluirá o custo de uso de infraestrutura subjacente do Azure. Nesse caso, os encargos de uso de infraestrutura do Azure serão exibidos em um arquivo de reconciliação do Azure separado.

- Quando você adquire e implanta um produto qualificado de avaliação gratuita de um ISV para seu cliente, o cliente é registrado automaticamente na avaliação gratuita pelo editor ISV. O período de avaliação gratuita termina automaticamente após o período definido pelo editor ISV. Depois que o período terminar, o cliente será cobrado. Isso significa que o arquivo de reconciliação pode mostrar duas linhas para um produto qualificado para avaliação: um que acompanha o período de avaliação e outro que acompanha a oferta paga (que exibirá um custo de $0 até o término do período de avaliação). Quando a avaliação terminar, a linha que mostra a oferta paga começará a mostrar os encargos. 

Para obter mais informações sobre o que cada coluna representa, consulte [usar seus arquivos de reconciliação](use-the-reconciliation-files.md). Consulte também [tipos de cobrança no Partner Center](billing-different-types.md)

## <a name="next-steps"></a>Próximas etapas

- [Gerenciar produtos do Marketplace comercial para clientes](csp-commercial-marketplace-manage.md)
- [Saiba mais sobre o suporte para produtos do Marketplace comercial](csp-commercial-marketplace-support.md)
