---
title: Comunicados de março de 2021
description: Comunicados de março de 2021 sobre o Microsoft Partner Center, incluindo novas funcionalidades, promoções, ofertas, mercados ou alterações nas ofertas existentes.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 03/22/2021
ms.openlocfilehash: a3172b78d41a966b52a824703a7f15f163467d63
ms.sourcegitcommit: 715368e56fe669d29c7981906e08bc8d7d5d62a4
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "104880728"
---
# <a name="march-2021-announcements"></a>Comunicados de março de 2021

Esta página apresenta os comunicados de março de 2021 sobre o Microsoft Partner Center.

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a>Correções feitas na lista de preços de software perpétuo de 1º de março de 2021

### <a name="categories"></a>Categorias

- Data: 23/03/2021
- Ofertas/mercados

### <a name="impacted-audience"></a>Público-alvo afetado

Provedores indiretos e parceiros de cobrança direta realizando transações de software perpétuo no programa do Provedor de Soluções na Nuvem 

### <a name="details"></a>Detalhes

A lista de preços para software perpétuo publicada em 1º de março de 2021 incluiu mercados que não deveriam estar lá. A lista de preços de software perpétuo foi atualizada em 17 de março de 2021 com as devidas correções. Tais correções aplicavam-se somente a:

- ID do produto: DF77X4D43RKT 
- Nome do produto: atualização do Windows 10 Home para Pro para Microsoft 365 Business
- Mercados removidos ou sem suporte: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG, NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM e ZW

Essas alterações se aplicam somente ao produto acima. Os demais produtos não tiveram correções. 

### <a name="next-steps-and-resources"></a>Próximas etapas e recursos

- Os parceiros que realizam transações com software perpétuo devem baixar a mais recente lista de preços de software perpétuo.
- Consulte os [códigos de país da região](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) para ver o mapeamento correto da abreviação dos países com apenas duas letras.
________________
## <a name="sdk-release-on-net-standard-v1170"></a><a name="13"></a> Lançamento do SDK no .NET Standard (v1.17.0)

### <a name="categories"></a>Categorias

- Data: 23/03/2021

- Capacidades
 
### <a name="impacted-audience"></a>Público-alvo afetado

Parceiros do programa CSP Direct Bill Partner e fornecedores do programa CSP Indirect Provider que estão usando o SDK do .NET do Partner Center.

### <a name="details"></a>Detalhes

Desde 23 de março de 2020, os parceiros já podem baixar a versão do [MicrosoftPartnerCenter.NETSDK (Galeria do NuGet | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), juntamente com as [amostras públicas atualizadas do GitHub](https://github.com/Microsoft/Partner-Center-DotNet-Samples) do SDK do Partner Center. Esta versão inclui atualizações para os seguintes métodos:

#### <a name="audit-updated-new-operation-types"></a>Auditoria atualizada: novos tipos de operação

Adicionados novos [tipos de operação](https://docs.microsoft.com/partner-center/develop/auditing-resources) para saber quando o cliente aprovou e terminou o DAP.

- DapAdminRelationshipApproved

- DapAdminRelationshipTerminated

#### <a name="audit-updated-new-resource-and-operation-types"></a>Auditoria atualizada: novos tipos de recurso e operação

Adição de novos [tipos de recursos e operação](https://docs.microsoft.com/partner-center/develop/auditing-resources) para dar suporte ao cenário de função de diretório do cliente.

- Novo tipo de recurso "CustomerDirectoryRole"

- Tipos de operação "AddUserMember" e "RemoveUserMember"

#### <a name="sdk-updates-to-customer-accounts"></a>Atualizações do SDK para contas de clientes

- Suporte para GET/customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus

- GET /customers/{customer-tenant-id}/qualifications

- POST /customers/{customer_id}/qualifications?code={validationCode}

#### <a name="additional-changes"></a>Alterações adicionais

As seguintes alterações são introduzidas como parte do Novo Comércio e atualmente estão disponíveis somente por convite para parceiros que fazem parte da visualização técnica da experiência de Novo Comércio M365/D365. Os parceiros que não fazem parte da visualização técnica do Novo Comércio não devem notar os impactos e devem ser compatíveis com versões anteriores.

- Alterações no catálogo:

  - GET /products/{product-id}/skus/{sku-id}

- Comprar e gerenciar:
  - GET /customers/{customerId}/subscriptions
  - GET /customers/{customerId}/subscriptions/{subscriptionId}
  - PATCH /customers/{customerId}/subscriptions/{subscriptionId}
  - GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities
  - GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions
  - POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions

### <a name="next-steps"></a>Próximas etapas

- Baixar a versão mais recente do [MicrosoftPartnerCenter.NETSDK (Galeria do NuGet | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)
- Baixe e examine as [amostras do GitHub](https://github.com/Microsoft/Partner-Center-DotNet-Samples)

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="12"></a>Oferta do marketplace comercial do CSP e incentivos do CSP no ano fiscal de 2021 para ofertas qualificadas

### <a name="categories"></a>Categorias

- Data: 18/03/2021
- Capacidades

### <a name="impacted-audience"></a>Público-alvo afetado

Provedores indiretos e parceiros de cobrança direta do programa Provedor de Soluções na Nuvem 

### <a name="details"></a>Detalhes

Provedores indiretos e parceiros de cobrança direta no programa de Provedor de Soluções na Nuvem podem vender ofertas de terceiros e receber um incentivo de reembolso para cada oferta de terceiros qualificada transacionada no Partner Center ou no portal do Azure. O incentivo será oferecido na forma de reembolso sobre as vendas cobradas de ofertas qualificadas e estará **disponível até 30 de junho de 2021**.  

Saiba mais abaixo sobre este incentivo para Ofertas do Marketplace Comercial dos CSP e entre em contato com seus clientes hoje mesmo para identificar as ofertas corretas a fim de habilitar o sucesso contínuo e transformação digital deles.

Firmamos parcerias com ISVs (fornecedores independentes de software) para trazer as soluções de IaaS e SaaS mais recentes ao mercado a fim de atender aos clientes da Microsoft. Os distribuidores ISV têm a opção de habilitar as vendas de suas ofertas por meio do canal Microsoft Partner. Nossas ofertas qualificadas para receber o incentivo se enquadram em duas categorias:

- Algumas ofertas SaaS e IaaS de terceiros com status incentivado de venda conjunta do Azure IP. 

- Aplicativos SaaS integrados com o Teams ou pelo menos dois aplicativos de produtividade do Microsoft 365, como PowerPoint, Word, Excel, Outlook ou SharePoint.

### <a name="next-steps-and-resources"></a>Próximas etapas e recursos

- Saiba mais sobre a conquista de [Incentivos de Parceiros](https://partner.microsoft.com/membership/partner-incentives) pela venda dos aplicativos do Marketplace qualificados para incentivos. Novas ofertas são adicionadas mensalmente.  
- [Recursos de incentivo para parceiro de cobrança direta do programa Provedor de Soluções na Nuvem](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [Recursos de incentivo para provedor indireto no programa Provedor de Soluções na Nuvem](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- Examine esta [apresentação](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) para saber mais sobre como vender os aplicativos do marketplace comercial. Confira os recursos adicionais [aqui](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/). 
- Explorar o catálogo do marketplace comercial no [Partner Center](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) ou no [portal do Azure](https://ms.portal.azure.com/#home)
- Usar [APIs](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) para integrar aplicativos ao marketplace da sua empresa
- Entre em contato com os ISVs com quem está interessado em fazer negócios
- Os provedores indiretos precisam se integrar usando APIs e orientar os revendedores sobre quais aplicativos vender

### <a name="questions"></a>Perguntas?  

Confira [este artigo](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) para obter uma visão geral do marketplace comercial no Partner Center.

Para obter assistência adicional, crie uma solicitação de suporte no Partner Center. Saiba mais em [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1).

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="11"></a>Atualizações de nomenclatura e pré-requisitos da oferta do Power BI Premium

### <a name="categories"></a>Categorias

- Data: 18/03/2021
- Funcionalidades

### <a name="summary"></a>Resumo

A lista de preços final de 1º de abril de 2021 será atualizada para esclarecer as informações de nomenclatura e/ou pré-requisitos das ofertas do Power BI Premium por usuário.

### <a name="impacted-audience"></a>Público-alvo afetado

Parceiros diretos e indiretos do programa CSP (Provedor de Soluções na Nuvem)

### <a name="details"></a>Detalhes

A lista de preços final de 1º de abril de 2021 será atualizada para esclarecer as informações de nomenclatura e/ou pré-requisitos das ofertas do Power BI Premium por usuário.

Até que a lista de preços final seja atualizada, use as informações desta seção para efetuar pedidos dos produtos corretos.

A seguir são mostrados os detalhes do SKU e dos pré-requisitos afetados.

| Nome de exibição da oferta na versão prévia da lista de preços de 1º de março |  Nome de exibição da oferta atualizada na lista de preços final de 1º de abril| ID da oferta |
| ------ | ----------- | ----------- |
| Complemento do Power BI Premium por Usuário (preço de equipe sem fins lucrativos)  |  Complemento do Power BI Premium por Usuário **(Office)** (preço para equipes de organizações sem fins lucrativos)   | 31c03289-47ab-4ab0-8df1-03742c127ac6   |

Os clientes precisam ter um dos seguintes pré-requisitos para adquirir essa oferta:

| Nome de exibição da oferta | ID da oferta |
| ------ | ----------- |
| Microsoft 365 E5 (preço para equipes de organizações sem fins lucrativos)  |  31bedf01-9e57-4ece-a53a-d3656a563931   |
|   Microsoft 365 E5 sem conferência de áudio (preço para equipes de organizações sem fins lucrativos)|  b456810a-c414-4e07-98fc-ef74e8175a09|
|   Office 365 E5 (preço para equipes de organizações sem fins lucrativos)| ce139fe5-8bd5-47ed-a5be-07c286f8b9e    |
|   Office 365 E5 (preço para equipes de organizações sem fins lucrativos) Avaliação|  2f192efe-608a-4c9c-9d19-2b0b70b0962e|
|   Office 365 E5 sem conferência de áudio (preço para equipes de organizações sem fins lucrativos)|  c3897426-9f49-4eaf-9b4d-7d9a1c72aef7|

A seguinte oferta do Power BI Premium tem um pré-requisito obrigatório para a compra:

| Nome de exibição da oferta | ID da oferta |
| ------ | ----------- |
|   Complemento do Power BI Premium por Usuário (preço de equipe sem fins lucrativos)|  ef0b895b-681b-4026-a5b1-dda182a57d40 |

Os clientes precisam ter este pré-requisito para adquirir essa oferta:

| Nome de exibição da oferta | ID da oferta |
| ------ |----------|
| Power BI Pro (preço para equipes de organizações sem fins lucrativos)  |   cabdfc93-5786-4224-bfd3-35d58f833b35 |

### <a name="next-steps"></a>Próximas etapas

Examine os recursos relacionados a esse tópico e compartilhe essas informações com os stakeholders apropriados da organização.  

### <a name="questions"></a>Perguntas?

Caso tenha dúvidas sobre essas ofertas, confira as comunidades relevantes no Yammer. 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="10"></a> Atualizações de preço de março para Microsoft 365 F3

### <a name="categories"></a>Categorias

- Data: 16/03/2021
- Ofertas/mercados

### <a name="summary"></a>Resumo

Os preços incorretos de março de 2021 para Microsoft 365 F3 em GBP (libras esterlinas) e EUR (euro) foram corrigidos.

### <a name="impacted-audience"></a>Público-alvo afetado

Parceiros que compraram o Microsoft 365 F3 em GBP ou EUR entre os dias 1º e 17 de março de 2021 por meio do programa CSP (Provedor de Soluções na Nuvem).

### <a name="details"></a>Detalhes

A Microsoft corrigiu os preços incorretos do Microsoft 365 F3. Os preços estavam incorretos apenas em GBP e EUR e somente nas ofertas adquiridas entre os dias 1º e 17 de março de 2021. As ofertas e as moedas afetadas estão listadas abaixo. 

| Nome da oferta | Moeda | ID da oferta | ID do material |
| ------ |----------- |----------- |----------- |
| Microsoft 365 F3 (caridade) | GBP | 57b722c2-c435-4bfb-9bc8-80509213a13a | AAD-11626 |
| Microsoft 365 F3 (comercial) | EUR| 3451a3b0-8cda-44a7-bad7-c30be81c4aaa | AAA-89898 |
 
As versões prévias das listas de preços baseadas em licença de março e abril foram atualizadas em 16 de março, às 17h, horário padrão do Pacífico.

### <a name="next-steps"></a>Próximas etapas

- Os parceiros devem baixar novamente as listas de preços atuais baseadas em licença, tanto da versão prévia de março quanto de abril, com essas correções de preços, se aplicável.  
- A Microsoft entrará em contato por email com os parceiros afetados nas próximas semanas para informar sobre o que fazer em seguida com relação à correção das transações afetadas.

### <a name="questions"></a>Perguntas?

Em caso de dúvidas adicionais, confira as comunidades relevantes sobre o CSP no Yammer.

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="9"></a> Atualizar a razão social de uma empresa por meio do Partner Center

### <a name="categories"></a>Categorias

- Data: 16/03/2021
- Conduza Eficiência e Escala

### <a name="summary"></a>Resumo

Desde março de 2021, os parceiros do MPN (Microsoft Partner Network) e os revendedores indiretos do CSP (Provedor de Soluções na Nuvem) podem atualizar a razão social da empresa por meio do Partner Center.

### <a name="impacted-audience"></a>Público-alvo afetado

Parceiros do MPN e revendedores indiretos do CSP (não aplicável a parceiros de cobrança direta do CSP)

### <a name="details"></a>Detalhes

Desde março de 2021, os parceiros do MPN e os revendedores indiretos do CSP podem atualizar a razão social da empresa por meio do Partner Center com conformidade e de maneira autônoma. Com esse novo recurso, os parceiros não precisarão mais enviar um tíquete de suporte do Partner Center para atualizar o nome da empresa. Isso economizará muito tempo para os parceiros na execução dessas atividades. 

Para saber mais, confira [Atualizar seu perfil comercial legal](../update-your-partner-profile.md#update-your-legal-business-profile).

>[!NOTE]
>Verifique se o nome da empresa no perfil comercial legal não tem erros de ortografia nem abreviações e se ele corresponde exatamente aos registros comerciais formais da empresa. Para mais informações sobre como atualizar o perfil da sua organização, veja [Verificar o perfil da organização](../update-your-partner-profile.md#update-your-legal-business-profile).

### <a name="next-steps"></a>Próximas etapas

Compartilhe essas informações em sua organização para que a equipe correta possa examinar e atualizar os processos delas.

### <a name="questions"></a>Perguntas?

Em caso de dúvidas adicionais, confira as comunidades relevantes sobre o CSP no Yammer.

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="8"></a> Atualização sobre a evolução do programa CSP (Provedor de Soluções na Nuvem) e as alterações do programa Open License

### <a name="categories"></a>Categorias

- Data: 15/03/2021
- Funcionalidades

### <a name="summary"></a>Resumo

Novas ofertas de software perpétuo para o setor público e comercial estão chegando ao programa CSP (Provedor de Soluções na Nuvem), juntamente com alterações no programa de Licenciamento Aberto.

### <a name="impacted-audience"></a>Público-alvo afetado

Distribuidores comerciais e revendedores gerenciados que fazem vendas usando o programa Open License e todos os parceiros CSP que realizam transações com software perpétuo

### <a name="details"></a>Detalhes

Em setembro de 2020, a Microsoft [anunciou](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) uma série de etapas em nosso percurso de transformação digital para expandir oportunidades para parceiros no programa CSP, incluindo a disponibilidade de software local para parceiros. Essas mudanças permitem que os parceiros expandam os negócios e ampliem o alcance deles aproveitando as licenças de software no CSP, preparando-os para ter sucesso no atual mundo que prioriza a nuvem. Elas também capacitam as transições dos clientes para a nuvem e dão aos parceiros a flexibilidade necessária para ambientes de nuvem híbrida.

Na continuação dessa transformação digital, estamos anunciando as seguintes mudanças:

- 1º de julho de 2021: não serão adicionados SKUs, produtos nem promoções à lista de preços do programa Open License.

- 7 de julho de 2021: duas ofertas comerciais, Get Genuine Windows e Visual Studio Professional, e ofertas para o setor público (governamental, educação e sem fins lucrativos – veja o [comunicado](./2020-december.md#9)) serão adicionadas à lista de preços do software perpétuo do CSP.  A lista de preços pode ser encontrada na seção Software da página [Vender > Preços e Ofertas](https://partnercenter.microsoft.com/pcv/sales) no Partner Center e será publicada novamente nessa data.

Para obter detalhes completos sobre a evolução do programa CSP e as mudanças no programa Open License, confira as **Próximas Etapas** abaixo.

### <a name="next-steps"></a>Próximas etapas:

- Evolução do programa CSP: examine os materiais de preparação sobre [Software perpétuo no programa Provedor de Soluções na Nuvem](https://partner.microsoft.com/resources/collection/software-in-csp#/). Use este [mapa de preparação](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) para localizar de maneira rápida as informações corretas para sua função.

- Mudanças no programa Open License: examine os materiais de preparação [Evolução do programa CSP e mudanças no programa Open License](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/). Use este [mapa de preparação](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) para localizar de maneira rápida as informações corretas para sua função.

### <a name="questions"></a>Perguntas

Em caso de dúvidas adicionais, confira as comunidades relevantes sobre o CSP no Yammer.

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="7"></a>Atualização sobre um comunicado anterior: Avaliações Premium e complemento do Gerenciador de Conformidade

### <a name="categories"></a>Categorias

- Data: 15/03/2021
- Amplie seu negócio

### <a name="summary"></a>Resumo

As ofertas de avaliação não deveriam ter sido listadas na lista de preço e serão removidas.

### <a name="impacted-audience"></a>Público-alvo afetado

Parceiros que fazem transações pelo programa Provedor de Soluções na Nuvem

### <a name="details"></a>Detalhes

As ofertas de avaliação não deveriam ter sido incluídas na lista de preços. Elas serão removidas da lista de preços de 1º de maio de 2021.

O comunicado original está [aqui](./2021-february.md#4).

### <a name="additional-resources"></a>Recursos adicionais

- [Segurança e conformidade do Microsoft 365 E5](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [Criar e gerenciar as avaliações no Gerenciador de Conformidade da Microsoft – Conformidade do Microsoft 365](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a>Próximas etapas

Examine os recursos relacionados a esse tópico e compartilhe essas informações com os stakeholders apropriados da organização.

### <a name="questions"></a>Perguntas?

Caso tenha dúvidas sobre essas ofertas, confira as comunidades relevantes no Yammer.

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="6"></a> Migrar suas soluções OCP (One Commercial Partner) GTM (go-to-market) para o marketplace comercial da Microsoft

### <a name="categories"></a>Categorias

- Data: 12/03/2021
- Funcionalidades

### <a name="summary"></a>Resumo

A partir de 29 de março de 2021, você começará a experimentar funcionalidades da OCP (One Commercial Partner) GTM (go-to-market) limitadas. Incentivamos você a migrar suas soluções para o marketplace comercial no Partner Center.

### <a name="impacted-audience"></a>Público-alvo afetado

Organizações que fazem vendas conjuntas com soluções OCP GTM

### <a name="details"></a>Detalhes

Em dezembro de 2020, iniciamos o percurso desde a ferramenta Microsoft OCP GTM até o marketplace comercial da Microsoft no Partner Center. Essa transição expande as funcionalidades do marketplace comercial em que você pode demonstrar suas soluções para milhões de clientes, compartilhar oportunidades de maneira bidirecional com outros vendedores parceiros e da Microsoft e vender soluções inovadoras em conjunto.

O próximo marco da transição ocorrerá em 29 de março de 2021. É quando você começará a experimentar funcionalidades da OCP GTM limitadas, com alguns campos se tornando somente leitura. Se, no momento, você estiver fazendo venda conjunta de soluções na OCP GTM, recomendamos que migre suas soluções para o marketplace comercial para aproveitar as funcionalidades dele e simplificar sua experiência de publicação. 

A migração para o marketplace comercial faz do Partner Center o principal destino para a experiência de publicação de venda conjunta. É lá que você pode continuar expandindo seus negócios conectando suas soluções com nossos clientes compartilhados por meio dos mesmos canais e de experiências no produto que usamos para produtos da Microsoft. [Saiba mais sobre o marketplace comercial](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).

### <a name="next-steps"></a>Próximas etapas

- Se você ainda não tiver migrado suas soluções, siga as instruções detalhadas no [guia de transição](/azure/marketplace/co-sell-solution-migration) ou veja o [tutorial de vídeo passo a passo](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) para concluir todas as atividades de migração e começar a publicar suas soluções no marketplace comercial.

- Caso tenha dúvidas sobre a experiência de funcionalidade limitada na OCP GTM, veja as [Perguntas frequentes sobre requisitos de venda conjunta para publicação no marketplace comercial da Microsoft](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf). (Confira a seção "Funcionalidades limitadas da OCP GTM a partir de 29 de março de 2021".)

### <a name="questions"></a>Perguntas?

Entre em contato com o [suporte](https://partner.microsoft.com/support/?stage=1) se você tiver dúvidas ou precisar de mais informações.

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a>Expandir a nova experiência de comércio no programa CSP (Provedor de Soluções na Nuvem) para Azure para a Rússia

### <a name="categories"></a>Categorias

- Data: 10/03/2021
- Capacidades

### <a name="impacted-audience"></a>Público-alvo afetado

Todos os parceiros na Rússia que fazem transações pelo programa CSP (Provedor de Soluções na Nuvem).

### <a name="details"></a>Detalhes

Desde 10 de março de 2021, estamos empolgados em anunciar a disponibilidade da **nova experiência de comércio no CSP para Azure na Rússia**. Essa experiência vai simplificar e aprimorar a maneira como os clientes compram e consomem os serviços do Azure. Ela também dará aos parceiros do programa CSP uma visão consistente do preço do Azure nos movimentos de vendas, o preço em dólares para consistência global, o alinhamento da data de cobrança e o acesso ao Gerenciamento de Custos do Azure.

### <a name="next-steps"></a>Próximas etapas

Há vários recursos disponíveis que apresentam a nova experiência de comércio do Azure e fornecem mais informações. Encontre as perguntas frequentes mais recentes, apresentações, vídeos e muito mais na [Galeria de Recursos de Atualizações do Programa CSP](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a>Cumprimento de chave de licença e download de software do Partner Center

### <a name="categories"></a>Categorias

- Data: 04/03/2021
- Funcionalidades

### <a name="summary"></a>Resumo

A capacidade de cumprimento de chave de licença e download de software do Partner Center foi restabelecida.

### <a name="impacted-audience"></a>Público-alvo afetado

Todos os parceiros CSP (Provedor de Soluções na Nuvem) que fazem a transação de pedidos de software de assinatura de servidor e perpétuas por meio do Partner Center

### <a name="details"></a>Detalhes

Em resposta aos comentários dos parceiros, estamos restabelecendo a capacidade de cumprimento do Partner Center para obter software e chaves de licença para pedidos de software de assinatura de servidor e perpétuas. Ela será restaurada para o estado anterior antes de ser removida em 19 de janeiro de 2021. Confira o [comunicado](2020-september.md#17).

Observe que as chaves de licença de software e os links de download são ativos de propriedade intelectual valiosos e muito procurados. Caso sejam vazados, poderão esgotar rapidamente os limites de ativação e causar uma experiência negativa para clientes e parceiros.

### <a name="next-steps"></a>Próximas etapas

Examine os seguintes recursos para obter instruções de uso e diretrizes importantes sobre a distribuição de chaves de software:

- [Vender software local por meio do programa CSP](../csp-on-premise-software.md)
- [Novo guia de operações de comércio do Partner Center](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (Confira a seção **Diretrizes sobre a distribuição de chaves de software**.)

### <a name="questions"></a>Perguntas?

Se tiver mais dúvidas sobre esse aviso, confira as comunidades relevantes no Yammer.

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a>Migre seus acordos do PSC (Partner Sales Connect) para o Partner Center

### <a name="categories"></a>Categorias

- Data: 04/03/2021
- Funcionalidades

### <a name="summary"></a>Resumo

O PSC (Partner Sales Connect) fará a migração para acesso somente leitura a partir de 31 de março de 2021. Portanto, incentivamos você a começar a migrar seus acordos do PSC para o Partner Center.

### <a name="impacted-audience"></a>Público-alvo afetado

Parceiros com acordos no PSC

### <a name="details"></a>Detalhes

Como parte do nosso compromisso com o crescimento compartilhado, a **venda conjunta com a Microsoft** é o caminho para você **ser descoberto, oferecer sua experiência e expandir a superfície do cliente** para que ele tenha resultados positivos. Com uma negociação média **3,5 vezes mais rápida** do que o normal, o gerenciamento de sua experiência de venda conjunta no Partner Center permite que você venda nos canais de clientes diretos, parceiros e vendedores da Microsoft e administre seu pipeline de referência em um lugar só.

O **PSC** fará a migração para o **acesso somente leitura** a partir de **31 de março de 2021**. Portanto, incentivamos você a começar a fazer a migração para o Partner Center e acessar estes aprimoramentos de funcionalidade: 

- **Encaminhamento mais preciso** dos acordos que você compartilha com a Microsoft para o vendedor certo, com base no tipo de assistência de que você precisa.
- **Validação da qualificação de acordos antecipados** para soluções qualificadas para incentivos e para atender aos critérios do programa ISV Connect, simplificando o processo de aprovação e o atestado de POE (comprovante de execução) final.
- **Experiência de usuário perfeita** para gerenciar todas as suas oportunidades de venda conjunta e leads qualificados por vendas em um lugar só.

Também adicionamos recentemente novos recursos ao Partner Center para ajudar você na sua migração:

- [Operações em massa para oportunidades de venda conjunta](../bulk-operations.md)
- [Recurso de migração de acordos](../psc-to-pc.md) (Confira a seção **Migração de acordos no PSC**.)

Usando a experiência de venda conjunta no Partner Center, suas equipes de vendas terão mais tempo para se concentrar em fomentar leads e oportunidades, fechar acordos e criar relações duradouras com o cliente.

### <a name="next-steps"></a>Próximas etapas

Use o [guia de transição](../psc-to-pc.md) do Partner Center para explicar as etapas para migrar seus acordos do PSC para o Partner Center.

### <a name="questions"></a>Perguntas?

Para outras perguntas, entre em contato com o [Suporte](https://partner.microsoft.com/support/?stage=1).

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a>Novos produtos e ofertas do Microsoft Dynamics 365 disponíveis em 1º de abril de 2021

### <a name="categories"></a>Categorias

- Data: 04/03/2021
- Funcionalidades

### <a name="summary"></a>Resumo

Em 1º de abril de 2021, a Microsoft iniciará vários novos produtos e ofertas para o programa CSP (Provedor de Soluções na Nuvem).

### <a name="impacted-audience"></a>Público-alvo afetado

Todos os parceiros que fazem transações pelo programa CSP (Provedor de Soluções na Nuvem)

### <a name="details"></a>Detalhes

Em 1º de abril de 2021, a Microsoft iniciará os seguintes novos produtos e oferecerá:

- Power BI Premium por Usuário
- Expansão geográfica e de segmento da USL do Marketing e Customer Voice

**Power BI Premium por Usuário**

A Microsoft apresentará as primeiras ofertas do Power BI Premium por usuário. No momento, o Power BI Premium é vendido apenas em um constructo de capacidade. O Power BI Premium por usuário fornece acesso a funcionalidades de BI (business intelligence empresarial) e análise. O licenciamento de estação individual flexível dele atende a empresas de pequeno e médio porte.

Examine os [detalhes de versão do Power BI](/power-platform-release-plan/2020wave2/power-bi/planned-features) para saber mais sobre esta oferta.


**Detalhes da oferta**

Observe que o nome da oferta difere ligeiramente da visualização da lista de preços.

| Nome da oferta | ID da oferta |
| ------ |----------- |
| Power BI Premium por Usuário | 9c810018-9356-4903-95ab-eeb956289290 | 
| Power BI Premium por Usuário para Docentes | 3affc44f-f372-4ad5-8657-aadd9574fce0 | 
| Power BI Premium por Usuário para Estudantes | 657eea87-d0b0-4c89-8c8e-9b04395bd940 | 
| Power BI Premium por Usuário (preço de equipe sem fins lucrativos) | 7a0a856c-059f-45dd-9d26-ae27992e706a | 
| Complemento do Power BI Premium por Usuário | 244ff87e-5925-44a0-bf31-cea189719b58 | 
| Complemento do Power BI Premium por Usuário para Docentes | 5da849bd-b8f7-4340-b4f4-3a9eaeb8987e | 
| Complemento do Power BI Premium por Usuário para Estudantes | cf62d70d-5af5-422a-bda8-97936402ac8e | 
| Complemento do Power BI Premium por Usuário (preço de equipe sem fins lucrativos) | 31c03289-47ab-4ab0-8df1-03742c127ac6 | 

**Expansão geográfica e de segmento da USL do Marketing e Customer Voice**

Como um acompanhamento para o lançamento de dezembro de 2020, as ofertas USL do Dynamics 365 Customer Voice e Marketing foram alteradas para adicionar novos países e mais SKUs educacionais e sem fins lucrativos.

| Nome da oferta | ID da oferta |
| ------ |----------- |
| USL do Dynamics 365 Customer Voice (preço de equipe sem fins lucrativos) | 7a8642a5-481e-4906-a642-b56dbeeb62a0 |
| USL do Dynamics 365 Customer Voice para Docentes | 85162d70-9676-4cf6-a4bc-a0d6672f2657 |

Acesse as seguintes páginas para saber mais sobre essas ofertas:

- [Página inicial do Dynamics 365 Customer Service Voice](https://dynamics.microsoft.com/customer-voice/overview/)
- [Página inicial do Dynamics 365 Marketing](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a>Próximas etapas

Examine os recursos sobre esse tópico e compartilhe essas informações com os stakeholders apropriados da organização.  

### <a name="questions"></a>Perguntas?

Caso tenha dúvidas sobre essas ofertas, confira as comunidades relevantes no Yammer. 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a> A Impressão Universal da Microsoft já está disponível em alguns pacotes

### <a name="categories"></a>Categorias

- Data: 03/03/2021
- Funcionalidades

### <a name="summary"></a>Resumo

A Impressão Universal da Microsoft está disponível para transações em pacotes do Microsoft 365 selecionados e como um complemento autônomo desde 1º de março de 2021.

### <a name="impacted-audience"></a>Público-alvo afetado

Todos os parceiros que fazem transações pelo programa CSP (Provedor de Soluções na Nuvem)

### <a name="details"></a>Detalhes

A [Impressão Universal](https://aka.ms/universalprint) é um serviço de impressão da Microsoft 365 que acaba com a necessidade de servidores de impressão locais e permite que dispositivos Windows imprimam em impressoras registradas no Azure. Ela está disponível para transações desde 1º de março de 2021.

Os trabalhadores se beneficiam da impressão sem driver, da descoberta simplificada de impressoras baseada em local e de uma experiência de impressão intuitiva, com nenhuma curva de aprendizado. Os dispositivos que ingressaram no Azure AD (Active Directory) usam credenciais do Azure AD existentes para imprimir com segurança. Os administradores gerenciam a impressão usando o portal do Azure e podem facilmente conectar impressoras com suporte nativo para Impressão Universal. A Impressão Universal pode ser implantada com impressoras não compatíveis usando o software do conector da Impressão Universal.

A Impressão Universal será acrescida ao Windows E3, A3, E5 e A5 e ao Microsoft 365 BP, F3, E3, A3, E5 e A5 no lançamento.  

**Detalhes da oferta**

Observe que o nome da oferta difere ligeiramente da visualização da lista de preços.

| Nome da oferta | ID da oferta | ID do material |
| ------ |----------- |----------- |  
| Complemento de volume da Impressão Universal (500 trabalhos) – Microsoft 365  | cb131356-45ee-4ae2-8537-873b706c8e75     | 9BI-00004   |
| Complemento de volume da Impressão Universal (500 trabalhos) para docentes – Microsoft 365   | 477bee81-9872-43d6-91d3-c72390bfcf49   | 9BK-00004   |
| Complemento de volume da Impressão Universal (500 trabalhos) – Windows    | d3ddc493-5741-4e0d-a02d-07edbb0bb72e   | 9BI-00002   |
| Complemento de volume da Impressão Universal (500 trabalhos) para docentes – Windows   |  d0862f05-80f5-4fd4-8432-fe72dd893cc7  | 9BK-00002   |

### <a name="next-steps"></a>Próximas etapas

Familiarize-se com a lista de preços e a [visão geral da Impressão Universal](/universal-print/fundamentals/universal-print-whatis). Compartilhe essas informações com todos os contatos adequados na sua organização.

### <a name="questions"></a>Perguntas?

Caso tenha dúvidas sobre essas ofertas, confira as comunidades relevantes no Yammer.
