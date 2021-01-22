---
title: Comunicados de janeiro de 2021
description: Comunicados de janeiro de 2021 sobre o Microsoft Partner Center, incluindo novas funcionalidades, promoções, ofertas, mercados ou alterações nas ofertas existentes.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 01/15/2021
ms.openlocfilehash: 9b972354fb21dbdfa4780717cee54bac14acdb0e
ms.sourcegitcommit: 9bcccaf8864d8ee3c93e67691f773463f162b5f0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/19/2021
ms.locfileid: "98571662"
---
# <a name="january-2021-announcements"></a>Comunicados de janeiro de 2021

Esta página fornece detalhes dos comunicados de janeiro de 2021 sobre o Microsoft Partner Center.

Comunicados de 2021: janeiro

Comunicados de 2020: [Maio](2020-may.md) | [Junho](2020-june.md) | [Julho](2020-july.md) | [Agosto](2020-august.md) | [Setembro](2020-september.md) | [Outubro](2020-October.md) | [Novembro](2020-november.md) | [Dezembro](2020-december.md)  

________________
## <a name="perpetual-software-now-generally-available-for-the-cloud-solution-provider-program"></a><a name="11"></a> Software perpétuo agora em disponibilidade geral no programa Provedor de Soluções na Nuvem

### <a name="categories"></a>Categorias

- Data: 19-01-2021
- Amplie seus negócios

### <a name="impacted-audience"></a>Público-alvo afetado

Todos os parceiros CSP

### <a name="details"></a>Detalhes

Conforme [anunciado](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) hoje, estamos animados para informar que as licenças perpétuas de softwares comerciais estão em disponibilidade geral para todos os parceiros CSP. A lista de preços de software perpétuo do CSP do Partner Center foi republicada e agora inclui produtos e geografias adicionais.

Observe também que, a partir de hoje, a funcionalidade de preenchimento de software e chave de licença do Partner Center foi desativada e os parceiros devem usar o Centro de Administração do Microsoft 365 para essa finalidade.
Veja abaixo mais detalhes e as próximas etapas.

### <a name="next-steps"></a>Próximas etapas

- Baixe a lista de preços de **Software perpétuo do CSP** na seção **Software** da página [Preços e Ofertas](https://partnercenter.microsoft.com/en-us/pcv/sales) do Partner Center. Uma lista dos produtos e geografias adicionados recentemente pode ser encontrada [aqui](https://partner.microsoft.com/resources/detail/software-in-csp-new-products-geos-pdf).
- Examine o [artigo de instruções para download de chaves de licença de produtos e software perpétuo no Centro de Administração do Microsoft 365](https://go.microsoft.com/fwlink/p/?linkid=2152525) e compartilhe com seus clientes quando eles estiverem prontos para baixar seus softwares e chaves de licença.
- Examine os materiais de preparação sobre [Software perpétuo no programa Provedor de Soluções na Nuvem](https://partner.microsoft.com/resources/collection/software-in-csp#/). Use este [mapa de preparação](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) para localizar de maneira rápida as informações corretas para sua função.

### <a name="questions"></a>Perguntas?

Em caso de dúvidas adicionais, confira as comunidades relevantes sobre o CSP no Yammer.

_____________
## <a name="reminder-introducingapithrottlingtopartners-calling-partner-centerapis"></a><a name="10"></a> Lembrete: introdução à limitação de API para parceiros que chamam as APIs do Partner Center 

### <a name="categories"></a>Categorias

- Data: 19-01-2021
- Amplie seus negócios

### <a name="summary"></a>Resumo

A Microsoft implementará a limitação de API para possibilitar um desempenho mais consistente dentro de um período de tempo para parceiros que chamam as APIs do Partner Center.

### <a name="impacted-audience"></a>Público-alvo afetado

Todos os parceiros que fazem transações pelo programa CSP (Provedor de Soluções na Nuvem)  

### <a name="details"></a>Detalhes

A partir de fevereiro de 2021, a Microsoft implementará a limitação de API para possibilitar um desempenho mais consistente dentro de um período de tempo para parceiros que chamam as APIs do Partner Center. A limitação restringe o número de solicitações para um serviço por um determinado período para evitar o uso excessivo de recursos. Quando um limite for excedido, o Partner Center limitará solicitações adicionais desse cliente durante um período de tempo.
  
**Benefícios do parceiro:** o Partner Center foi criado para lidar com um alto volume de solicitações, mas se um número excessivo delas for realizado por alguns parceiros, a limitação ajudará a manter o desempenho ideal e a confiabilidade para todos os parceiros.  

- A limitação garante um tempo de inatividade mínimo.
- A limitação reduz o número de solicitações de alto volume, ajudando a garantir um desempenho consistente para todos os parceiros.

**APIs a serem limitadas:**

| Operação | Documentação do Partner Center |
| ------ | ------- |
|{baseURL}/v1/customers/{ID_do_cliente}/subscriptions  | [Get-all-of-a-customer-s-subscriptions](/partner-center/develop/get-all-of-a-customer-s-subscriptions&data) |
|{baseURL}/v1/customers/{ID_do_cliente}/subscriptions/{ID_da_assinatura}  | [Obter uma assinatura por ID](/partner-center/develop/get-a-subscription-by-id) |
|{baseURL}/v1/customers/{ID_do_cliente}/orders  | [Obter todos os pedidos de clientes](/partner-center/develop/get-all-of-a-customer-s-orders) |
|{baseURL}/v1/customers/{ID_do_cliente}/orders/{ID_do_pedido}  | [Obter uma ordem por ID](/partner-center/develop/get-an-order-by-id) |
|{baseURL}/v1/customers/{ID_do_cliente}/orders/{ID_do_pedido}/provisioningstatus  | [Obter o status de provisionamento da assinatura](/partner-center/develop/get-subscription-provisioning-status) |
|{baseURL}/v1/customers/{ID_do_cliente}/subscriptions/{ID_da_assinatura}  | [Gerenciar pedidos e uma assinatura](/partner-center/develop/manage-orders#manage-a-subscription) |
|{baseURL}/v1/customers/{ID_do_cliente}/subscriptions/{ID_da_assinatura}/addons  | [Obter uma lista de complementos de uma assinatura](/partner-center/develop/get-a-list-of-add-ons-for-a-subscription) |
|{baseURL}/v1/customers/{ID_do_cliente}/subscriptions/{ID_da_assinatura}/azureEntitlements | [Obter uma lista de direitos do Azure para uma assinatura](/partner-center/develop/get-a-list-of-azure-entitlements-for-subscription) |
|{baseURL}/v1/customers/{ID_do_cliente}/subscriptions/{ID_da_assinatura}/registrationstatus  | [Obter o status de registro de assinatura](/partner-center/develop/get-subscription-registration-status) |
|{baseURL}/v1/customers/{ID-do-locatário-do-cliente}/transfers  | [Obter todas as transferências de um cliente](/partner-center/develop/get-all-of-a-customer-s-transfers) |
|{baseURL}/v1/productUpgrades/{ID-da-atualização}/status  | [Obter o status de atualização do produto](/partner-center/develop/get-product-upgrade-status) |
|{baseURL}/v1/customers/{ID-do-cliente}/subscriptions/{ID-da-assinatura}/conversions   | [Obter uma lista de ofertas de conversão de avaliação](/partner-center/develop/get-a-list-of-trial-conversion-offers) |
 
É altamente recomendável que os parceiros considerem o uso da API do log de atividades para ter mais eficiência e evitar a limitação. Para obter mais informações sobre esse recurso, confira os detalhes [aqui](/partner-center/develop/api-throttling-guidance).  

### <a name="next-steps"></a>Próximas etapas

Examine os [recursos](/partner-center/develop/api-throttling-guidance) sobre este tópico e execute as etapas necessárias.  

_____________

## <a name="security-compliance-and-identity-sci-launches-coming-on-february-1-2021"></a><a name="9"></a>As iniciações de SCI (Segurança, Conformidade e Identidade) chegam em 1º de fevereiro de 2021 

### <a name="categories"></a>Categorias

- Data: 15-01-2021
- Ofertas/mercados

### <a name="summary"></a>Resumo

Vários lançamentos do Microsoft 365 serão incluídos na versão prévia da lista de preços em janeiro e ficarão disponíveis a partir de 1º de fevereiro de 2021.

### <a name="impacted-audience"></a>Público-alvo afetado

Todos os parceiros que fazem transações pelo programa CSP (Provedor de Soluções na Nuvem)

### <a name="details"></a>Detalhes

#### <a name="microsoft-365-g5-compliance-component-skus-for-government"></a>[SKUs do componente de conformidade do Microsoft 365 G5 para o governo](/office365/servicedescriptions/microsoft-365-service-descriptions/microsoft-365-tenantlevel-services-licensing-guidance/microsoft-365-security-compliance-licensing-guidance)

Lançaremos três novas ofertas de componentes para os clientes GCC (Nuvem da Comunidade Governamental) e GCC High, que estarão disponíveis a partir de 1º de fevereiro de 2021. Essas SKUs serão equivalentes à Proteção e Governança de Informações do Microsoft 365 E5, ao Gerenciamento de Riscos Internos do M365 E5 e ao eDiscovery e Auditoria do Microsoft 365 E5, disponíveis atualmente na versão Comercial. 

   |**Nome da oferta**|**ID da oferta**|**ID do material**|
   |-------------------|:------|:------|
   |Governança e proteção de informações do Microsoft 365 E5 para GCC|9e5397ab-f309-4d90-97f3-6fb5d53074d6|8QL-00002|
   |Descoberta eletrônica e auditoria do Microsoft 365 E5 para GCC|5c9ef884-6307-47e7-a914-f5092feae51e|8RI-00002|
   |Gerenciamento de riscos para informações privilegiadas do Microsoft 365 E5 para GCC|11ccfdb3-80cb-4c80-8146-c9775045df17|8RF-00002|
   |DLP (complemento) e proteção de informações do Microsoft 365 E5 para GCC|911d3177-53a9-42ec-a0e9-3b73fce527f0|8QY-00002|

#### <a name="10-year-audit-log-retention-add-on"></a>[Complemento de retenção de logs de auditoria por 10 anos](/microsoft-365/compliance/)

Um complemento disponível com um pré-requisito do Microsoft 365 E5 permitirá que os clientes armazenem seus dados por 10 anos. 

   |**Nome da oferta**|**ID da oferta**|**ID do material**|
   |-------------------|:------|:------|
   |Complemento de retenção de logs de auditoria por 10 anos para EDU|879b5e1a-eaa2-4ea9-a628-0b429b2e8732|8LC-00002|
   |Complemento de retenção de logs de auditoria por 10 anos|e14ce8d1-09f4-42d2-9b5e-ee85f32e7be4|8LB-00003|
   
#### <a name="frontline-worker-add-ons"></a>Complementos para trabalhadores de linha de frente

A partir de 1º de fevereiro de 2021, os clientes podem comprar três novas ofertas programáticas de Segurança e Conformidade para trabalhadores de linha de frente como complementos para as [SKUs F1 e F3 do Microsoft 365](https://www.microsoft.com/microsoft-365/firstline-workers).

Essas ofertas programáticas substituirão a promoção de [Segurança e Conformidade](https://microsoft.sharepoint.com/teams/M365LicensingNews/SitePages/Security-and-Compliance-Promotion-for-Firstline-Workers-Update.aspx) atual que vai expirar em **28 de fevereiro de 2021**. Diferente da promoção atual, os complementos do F5 oferecem aos clientes mais previsibilidade à medida que a força de trabalho deles de linha de frente cresce.

   
   |**Nome da oferta**|**ID da oferta**|**ID do material**|
   |-------------------|:------|:------|
   |Segurança do Microsoft 365 F5|a8fba59e-1fc2-4658-8684-5f3d0c71c490|8RQ-00003|
   |Conformidade do Microsoft 365 F5|6dc6cb1d-7bcb-4234-80cc-9c7a9cded044|8RL-00003|
   |Segurança e Conformidade do Microsoft 365 F5|ad396924-ee4e-4059-b779-efe43dfa24d2|8RU-00003|
   
### <a name="next-steps"></a>Próximas etapas

Examine a versão prévia da lista de preços e compartilhe com os stakeholders apropriados em sua organização. Para saber mais, acesse [Segurança e Conformidade da Microsoft – Microsoft Tech Community](https://techcommunity.microsoft.com/t5/microsoft-security-and/ct-p/MicrosoftSecurityandCompliance).

### <a name="questions"></a>Perguntas?

Em caso de dúvidas adicionais sobre essas ofertas, confira as comunidades relevantes no Yammer. 

_____________ 

## <a name="docusign-migration-to-adobe-sign-for-partners-under-microsoft-partner-agreements-mpas"></a><a name="8"></a>Migração do DocuSign para o Adobe Sign para os parceiros com MPAs (Contratos de Parceiro da Microsoft) 

### <a name="categories"></a>Categorias

- Data: 15-01-2021
- Funcionalidades

### <a name="summary"></a>Resumo

A Microsoft fará a transição de todo o processamento de assinatura eletrônica do DocuSign para o Adobe Sign.

### <a name="impacted-audience"></a>Público-alvo afetado

Parceiros CSP (Provedor de Soluções na Nuvem) indiretos e diretos que têm um MPA. Parceiros na Ucrânia, na Rússia e no Cazaquistão precisarão assinar de maneira física ou eletrônica a cláusula adicional anualmente.

### <a name="details"></a>Detalhes

Em fevereiro de 2021, a Microsoft iniciará a transição de todo o processamento de assinatura eletrônica do DocuSign para o Adobe Sign para parceiros CSP. 

Você deverá esperar uma transição sem problemas. Após a migração, você receberá um email de adobesign@adobesign.com, em vez da DocuSign, sempre que sua assinatura eletrônica for necessária. Esse email fornecerá um link para a página da Web do Adobe Sign, em que você precisará assinar. Parceiros da Microsoft não precisarão assinar novamente contratos existentes, somente Contratos de Canal futuros. 

Veja um exemplo de um email de solicitação de assinatura do Adobe Sign na [galeria de recursos](https://partner.microsoft.com/resources/detail/adobe-sign-signature-request-email-pdf). 

**Para ter a melhor experiência, não deixe de fazer o seguinte:**

1. Adicione adobesign@adobesign.com à sua lista de remetentes seguros para evitar que emails dessa conta vão diretamente para a pasta de lixo eletrônico.
2. Trabalhe com seu departamento de TI para:
   - Atualizar o endereço de email adobesign@adobesign.com à lista de remetentes seguros para garantir que ele não seja incluído em nenhuma regra de phishing existente.
   - Atualizar as políticas de segurança existentes para garantir que todos os destinatários necessários possam assinar a documentação com sua licença empresarial do Adobe Sign.

O Adobe Sign é a ESS (Solução de Assinatura Eletrônica) preferencial da Microsoft. A transição para o Adobe Sign garantirá uma experiência de assinatura eletrônica segura e eficiente que oferecerá maior valor para nossos clientes e parceiros.

Para saber mais sobre como assinar documentos eletronicamente e sobre a delegação de assinatura eletrônica, confira os seguintes **tutoriais**: 
- [Assinar um documento eletronicamente | Tutoriais do Adobe Sign](https://helpx.adobe.com/sign/how-to/adobe-for-signers.html?playlist=/ccx/v1/collection/product/sign/segment/designer/explevel/beginner/applaunch/continuinged/collection.ccx.js&ref=helpx.adobe.com)
- [Delegar alguém para assinar um documento | Tutoriais do Adobe Sign](https://helpx.adobe.com/sign/how-to/use-the-delegator-role.html?playlist=/ccx/v1/collection/product/sign/segment/designer/explevel/beginner/applaunch/orientation/collection.ccx.js&ref=helpx.adobe.com)

### <a name="next-steps"></a>Próximas etapas

Compartilhe essas informações com os stakeholders apropriados da sua organização.

### <a name="questions"></a>Perguntas?

Em caso de dúvidas, entre em contato com o Centro de Operações Regionais usando a [CLT (Ferramenta de Log de Chamadas)](https://clt.partners.extranet.microsoft.com/CLT) ou no [Explore MS](https://www.explore.ms/). Siga o processo padrão da CLT para que possamos resolver sua consulta o mais rápido possível.

_____________ 

## <a name="commercial-pricing-update-for-norwegian-krone"></a><a name="7"></a>Atualização de preço comercial para coroa norueguesa 

### <a name="categories"></a>Categorias

- Data: 14-01-2021
- Ofertas/mercados

### <a name="impacted-audience"></a>Público-alvo afetado

Parceiros CSP que usam a coroa norueguesa.

### <a name="details"></a>Detalhes

A partir de 1º de março de 2021, os preços em coroas noruegueses para software comercial local e serviços online serão alterados a fim de realinhá-los aos níveis de preço predominantes na região.
O comunicado completo está disponível somente para parceiros da Microsoft. [Conecte-se para acessar o comunicado completo](https://partner.microsoft.com/resources/detail/pricing-update-norway-partners-pdf).

_____________ 

## <a name="commercial-pricing-update-for-the-indian-rupee"></a><a name="6"></a>Atualização de preços comerciais para INR 

### <a name="categories"></a>Categorias

- Data: 08/01/2021
- Ofertas/mercados

### <a name="impacted-audience"></a>Público-alvo afetado

Parceiros do CSP que atuam na Índia.

### <a name="details"></a>Detalhes 

A Microsoft está fazendo alterações na lista de preços em INR para alinhar os preços para software comercial e serviços online na Índia e na região asiática.

O comunicado completo só está disponível para os parceiros da Microsoft. [Faça logon para acessar o comunicado completo](https://partner.microsoft.com/resources/detail/price-update-indian-rupee.pdf).

________________

## <a name="calling-plan-and-phone-system-updates-for-february-1-20201"></a><a name="5"></a>Atualizações do Plano de Chamadas e do Sistema de Telefonia de 1º de fevereiro de 2021

### <a name="categories"></a>Categorias

- Data: 08/01/2021
- Ofertas/mercados

### <a name="summary"></a>Resumo

Uma oferta de complemento para Microsoft 365, que incluirá o Sistema de Telefonia, o Plano de Chamadas Nacionais e um Plano de Chamadas Nacionais independente, estará disponível em breve para países selecionados.

### <a name="impacted-audience"></a>Público-alvo afetado

Todos os parceiros que fazem transações pelo programa de CSP (Provedor de Soluções de Nuvem).

### <a name="details"></a>Detalhes 

A oferta no pacote do complemento para as ofertas do Microsoft 365 E1, E3 e E5 incluirá o Sistema de Telefonia e o Plano de Chamadas Nacionais. Além disso, uma nova oferta de Plano de Chamadas Nacionais independente estará disponível apenas para o E5. As novas ofertas estarão disponíveis somente para os clientes nos EUA, Porto Rico e Canadá. Para todos os outros países e regiões, os preços e SKUs independentes globais atuais continuam os mesmos. 

Essas ofertas estarão disponíveis para clientes comerciais, estudantes, docentes, de Nuvem da Comunidade Governamental (GCC) e de organizações sem fins lucrativos nos EUA, Porto Rico e Canadá. Os planos de chamadas não estão disponíveis em nenhum dos outros territórios dos EUA.

   |**Nome da oferta**|**ID da oferta**|**ID do material**|
   |-------------------|:------|:------|
   |Microsoft Teams Calling Essentials para EUA e Canadá|1ee81de6-4d8b-4cf1-b926-2fd2a774a4ca|8N2-00010|
   |Microsoft Teams Calling Essentials para EUA e Canadá (preços para equipes de organizações sem fins lucrativos)|0c2ece0d-39b7-40ec-8c08-87c2b6c75d62|8N2-00011|
   |Microsoft Teams Calling Essentials para EUA e Canadá para docentes|b8baa3b8-8cc2-4f26-a212-7fbeb28e7895|8N3-00003|
   |Microsoft Teams Calling Essentials para EUA e Canadá para estudantes|26956da8-eeb5-44e3-aa79-d36e0e42b930|8N3-00004|
   |Microsoft Teams Calling Essentials para EUA e Canadá para GCC|7a2e2d5a-41b5-4b20-a0d1-0d06d34b5fe1|8N4-00002|
   |Plano de Chamadas Nacionais do Microsoft 365 para os EUA e Canadá|60d2919e-427a-46c9-bd03-89cbad27d53f|TK2-00050|
   |Plano de Chamadas Nacionais do Microsoft 365 para docentes dos EUA e Canadá|602e7548-375b-4e01-bf79-a9a8b8ff16d4|LM7-00006|
   |Plano de Chamadas Nacionais do Microsoft 365 para estudantes dos EUA e Canadá|1f4b4375-3185-40cf-b044-117fe3b102c6|LM7-00007|
   |Plano de Chamadas Nacionais do Microsoft 365 para GCC dos EUA e Canadá|594ed84e-ddf8-4e40-9726-76c04bd29e3b|LM9-00023|

### <a name="next-steps"></a>Próximas etapas

- Compartilhe essas informações com os contatos relevantes em sua organização e entenda as oportunidades de venda adicional e cruzada. 
- Examine a seção de recursos do [Guia do parceiro do Teams](https://aka.ms/teamscallingmeetingsguide).

_____________ 

## <a name="license-base-price-list-updates-for-january-2021"></a><a name="4"></a>Atualizações da lista de preços baseada em licenças de janeiro de 2021 

### <a name="categories"></a>Categorias

- Data: 08/01/2021
- Ofertas/mercados

### <a name="summary"></a>Resumo

As listas de preços de janeiro e fevereiro para ofertas baseadas em licença foram atualizadas para corrigir determinados preços de lista incorretos.

### <a name="impacted-audience"></a>Público-alvo afetado

Todos os parceiros que fazem transações pelo programa de CSP (Provedor de Soluções de Nuvem).

### <a name="details"></a>Detalhes 

As listas de preços com base em licenças para janeiro e fevereiro de 2021 incluíam alguns preços de lista incorretos. As ofertas e as moedas afetadas estão abaixo. O preço correto foi atualizado e disponibilizado a partir de 7 de janeiro de 2021 14h PST (Horário Padrão do Pacífico). 

   |**Nome da oferta**|**ID da oferta**|**ID do material**|
   |-------------------|:------|:------|
   |Microsoft 365 E3|2b3b8d2d-10aa-4be4-b5fd-7f2feb0c3091|AAA-35638| 
   |Microsoft 365 Business Basic|bd938f12-058f-4927-bba3-ae36b1d2501c|AAA-10624|

Moedas afetadas: 

- Os problemas de preço do Microsoft 365 E3 eram limitados apenas a estas moedas: JPY (iene (Japão)), GBP (libra esterlina), EUR (União Europeia), AUD (dólar australiano). 
- Os problemas de preço do Microsoft 365 Business eram limitados apenas ao US$ (dólar americano). 

Os parceiros devem fazer referência às listas de preços prévias de janeiro e fevereiro disponíveis para encontrar os preços corretos. 

### <a name="next-steps"></a>Próximas etapas

- Os parceiros devem baixar os arquivos de lista de preços mais recentes do Partner Center para obter os preços corrigidos de janeiro e fevereiro. 
- Os administradores globais de locatários afetados que compraram assinaturas entre 1º e 6 de janeiro serão notificados por meio de um email do Partner Center antes do fim de janeiro com mais detalhes. 

_____________ 

## <a name="euefta-change-of-partner-billing-currency-for-new-commerce-offers"></a><a name="3"></a> Alteração da moeda de cobrança do parceiro da EU/EFTA para novas ofertas de comércio

### <a name="categories"></a>Categorias

- Data: 07/01/2021
- Capacidades

### <a name="impacted-audience"></a>Público-alvo afetado

- Todos os parceiros que fazem transações pelo programa de Provedor de Soluções na Nuvem na região EU/EFTA 

### <a name="details"></a>Detalhes

Na região EU (União Europeia)/EFTA (Associação Europeia de Livre Comércio), todas as novas ofertas de comércio no programa Provedor de Soluções na Nuvem usarão o local de cobrança do parceiro, em vez do local de cobrança do cliente. Dessa forma, os parceiros serão cobrados pela Microsoft com base na moeda do local em que eles estão, não na moeda do local dos clientes. Essas alterações serão feitas em duas fases:

**Fase 1:**

- novo cliente comprando uma nova oferta de comércio no CSP

- Primeira compra de novas ofertas de comércio de clientes existentes – locatário criado antes de 11 de maio de 2020

A partir de 28 de janeiro de 2021, parceiros que têm novos clientes de rede comprando uma nova oferta de comércio, ou clientes existentes com locatários criados antes de 11 de maio de 2020 fazendo sua primeira compra de novas ofertas de comércio, serão cobrados pelas compras na moeda do local do parceiro.  

Parceiros com clientes existentes que já compraram novas ofertas de comércio no CSP continuarão sendo cobrados na moeda do local de cobrança do cliente durante essa fase. Além disso, os parceiros com clientes existentes fazendo a primeira compra de uma nova oferta de comércio, cujos locatários foram criados em 11 de maio de 2020 ou após essa data, continuarão sendo cobrados na moeda do cliente.

**Fase 2:**

- clientes existentes que já compraram uma nova oferta de comércio no CSP antes da Fase 1
- Primeira compra de novas ofertas de comércio de clientes existentes – locatário criado em 11 de maio de 2020 ou após essa data

Após a Fase 1 e durante o ano de 2021, a Microsoft fará a transição da cobrança de novas ofertas de comércio para parceiros com clientes existentes, que compraram uma nova oferta de comércio no CSP antes da Fase 1, assim como clientes que tiveram seus locatários criados em 11 de maio de 2020 ou após essa data, da moeda do local do cliente para a moeda do local do parceiro. Os parceiros serão notificados com bastante antecedência antes que essa alteração seja implementada.

Após a Fase 2, os parceiros na região da UE/EFTA serão cobrados na moeda do local do parceiro para todos os clientes e todas as compras do CSP.

>[!NOTE]
>Essa alteração afetará apenas a moeda de cobrança do parceiro e não o preço de novas ofertas de comércio no CSP. As novas ofertas de comércio no escopo para essa alteração são: Assinaturas do Azure que fazem parte de um plano do Azure, reservas do Azure, assinaturas de servidor, software perpétuo e compras do marketplace comercial da Microsoft no programa do Provedor de Soluções na Nuvem.


### <a name="partner-benefits"></a>Benefícios do parceiro

Essa atualização reduzirá a complexidade e a sobrecarga com o faturamento em várias moedas na região EU/EFTA para a nova experiência de comércio.

- Os parceiros receberão uma fatura consolidada em uma moeda e não receberão mais uma fatura para cada moeda do local do cliente
- Os pagamentos de incentivos estarão na mesma moeda que a moeda da fatura do parceiro
- Os parceiros perceberão que a cobrança ficou menos complexa devido ao faturamento em várias moedas; isso vai liberar tempo e recursos associados atualmente à reconciliação de contas
- Para parceiros que ainda não adotaram novas ofertas de comércio, essa alteração se alinha com o modelo de cobrança de parceiro anterior, permitindo que os parceiros façam uma transição mais fácil para a nova experiência de comércio no CSP

### <a name="next-steps"></a>Próximas etapas

Examine as informações sobre esse tópico na [Galeria de Operações](https://partner.microsoft.com/resources/collection/eu-efta-changes-collection#/) (entrada necessária) no site de parceiros da Microsoft.  

### <a name="questions"></a>Perguntas?

Para fazer perguntas relacionadas a esta notificação, entre em contato com o [suporte do Partner Center](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals) (entrada necessária).

### <a name="change-log"></a>Log de alterações

- 17 de novembro de 2020: Publicação original
- 7 de janeiro de 2021: Cenário adicional incluído para a Fase 1 e a Fase 2


________________
## <a name="deprecation-and-retirement-of-existing-get-and-put-qualification-apis-for-the-education-customer-validation-process-by-the-end-of-february-2021"></a><a name="2"></a>Reprovação e desativação das APIs de Qualificação GET e PUT existentes para o processo de validação do cliente de Educação até o fim de fevereiro de 2021

### <a name="impacted-audience"></a>Público-alvo afetado

Parceiros que vendem ofertas Acadêmicas por meio do programa Provedor de Soluções na Nuvem usando a API do Partner Center

### <a name="details"></a>Detalhes 

Este é um acompanhamento dos aprimoramentos de API lançados em dezembro de 2020. Em dezembro de 2020, novas APIs de Qualificações GET e POST foram lançadas e, como resultado, as APIs de Qualificação GET e PUT antigas serão desativadas até o final de fevereiro de 2021. Nessa data, você precisará usar as novas APIs GET e POST do Partner Center para comprar ofertas de Educação. 

### <a name="next-steps"></a>Próximas etapas

- Se você ainda não fez isso, faça a atualização para as novas APIs a fim de realizar uma transição bem-sucedida e em tempo hábil.
- Examine as novas alterações da API do Partner Center e o [Guia nos recursos de Preparação de Operações:  aprimoramentos do processo de validação do cliente de Educação do Partner Center](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/).
- Compartilhe essas informações com as equipes apropriadas da sua organização e com seus revendedores para ajudá-los a se preparar para essas alterações.

_____________

## <a name="dynamics-365-offers-for-february-2021"></a><a name="1"></a>Ofertas do Dynamics 365 para fevereiro de 2021

### <a name="categories"></a>Categorias

- Data: 04/01/2021
- Ofertas

### <a name="summary"></a>Resumo

As novas alterações da oferta do Dynamics 365 serão iniciadas em fevereiro de 2021.

### <a name="impacted-audience"></a>Público-alvo afetado

Parceiros que participam dos programas de incentivo de revendedor indireto, provedor indireto e parceiro de cobrança direta do CSP (Provedor de Soluções na Nuvem)

### <a name="details"></a>Detalhes

A Microsoft está anunciando novas alterações da oferta do Dynamics 365, que serão iniciadas em fevereiro de 2021 para:

- Resposta Adicional da Opinião do Cliente para o Dynamics 365
- Fim da Vida Útil do Dynamics 365 Customer Service Insights
- Alteração das IDs da Oferta de Migração do Dynamics 365 Cloud AX

**Resposta Adicional da Opinião do Cliente para o Dynamics 365**

Em 1º de fevereiro de 2021, a Microsoft criará uma oferta de "Resposta Adicional" com direito a mil respostas para substituir a oferta existente de duas mil respostas de pesquisa, cujo fim da venda será em 1º de fevereiro de 2021.

Confira a guia "Resposta Adicional da Opinião do Cliente" no [documento do Excel Ofertas do Dynamics CSP – Fevereiro de 2021](https://partner.microsoft.com/resources/detail/dynamics-csp-offers-february-2021-xls) para obter os detalhes do SKU. Acesse a [home page da Opinião do Cliente para o Microsoft Dynamics 365](https://dynamics.microsoft.com/en-us/customer-voice/overview/) para obter mais informações.

**Fim da Vida Útil do Dynamics 365 Customer Service Insights**

Em 1º de fevereiro de 2021, os seguintes produtos serão alterados para o fim da vida útil:

- Dynamics 365 Customer Service Insights (incluindo "Casos Adicionais")
- Agente Virtual do Dynamics 365 para Serviço de Atendimento ao Consumidor

A experiência autônoma do "Customer Service Insights" está migrando para o "Dynamics 365 Customer Service", no qual os clientes podem encontrar as mesmas funcionalidades profundamente incorporadas às experiências de serviço de atendimento ao consumidor.  

Confira a guia "Customer Service Insights" no [documento do Excel Ofertas do Dynamics CSP – Fevereiro de 2021](https://partner.microsoft.com/resources/detail/dynamics-csp-offers-february-2021-xls) para obter os detalhes do SKU. Acesse a [home page do Microsoft Dynamics Customer Service](https://dynamics.microsoft.com/customer-service/overview/) para obter mais informações.

**IDs da oferta de migração do Dynamics 365 Cloud AX**

Esses SKUs foram removidos da lista final de preços de 1º de janeiro de 2021 e não estarão disponíveis para pedidos no momento. 

   |**Nome da oferta**|**ID da oferta**|
   |-------------------|:------|
   |Programa de Migração do Dynamics 365 Finance for AX|7fbd1115-a4c1-4cf9-b881-40c4187ca581|
   |Programa de Migração do Dynamics 365 Supply Chain Management for AX|a3c62c0e-4f8a-4fc9-a47e-dec3310529d0|
   |Programa de Migração do Dynamics 365 Commerce for AX|97e98de6-24a8-4282-bad6-9d1a874e90a4|
   |Anexo do Dynamics 365 Finance à Oferta Base Qualificada do Dynamics 365 para o Programa de Migração do AX|69d789e8-1e93-4dee-86b2-3ddfb03c08b9|
   |Anexo do Dynamics 365 Supply Chain Management à Oferta Base Qualificada do Dynamics 365 para o Programa de Migração do AX|c897adce-2964-4d24-abc3-7f7ad4b6a80d|
   |Anexo do Dynamics 365 Commerce à Oferta Base Qualificada do Dynamics 365 para o Programa de Migração do AX|ba1fe561-cfda-405a-a25d-ecda3bd3cba7|
   |Dynamics 365 Operations – Atividade para o Programa de Migração do AX|177e954e-1fff-4941-8967-55a47e36e1ce|
   |Dynamics 365 Operations – Dispositivo para o Programa de Migração do AX|8c8b7c8f-cb3a-4737-8319-1752938c7be3|
   |Membros da Equipe do Dynamics 365 para o Programa de Migração do AX|1eb3ad0b-9de3-419d-8bfe-0d61bdd945b2|

### <a name="next-steps"></a>Próximas etapas

Examine os recursos relacionados a este tópico e compartilhe-os com os stakeholders apropriados da sua organização. 

### <a name="questions"></a>Perguntas?

Em caso de dúvidas adicionais sobre essas ofertas, confira as comunidades relevantes no Yammer.

________________
