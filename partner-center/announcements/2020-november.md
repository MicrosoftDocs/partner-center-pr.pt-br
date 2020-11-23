---
title: Comunicados de novembro de 2020
description: Comunicados de novembro de 2020 sobre o Microsoft Partner Center, incluindo novas funcionalidades, promoções, ofertas, mercados ou alterações nas ofertas existentes.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom: announcement
ms.localizationpriority: high
ms.date: 11/02/2020
ms.openlocfilehash: 88d216f9e55b98f3c4818dd718c68f843c4098f0
ms.sourcegitcommit: 6ed7268356445939db8613f2af96016707c55d64
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/17/2020
ms.locfileid: "94691292"
---
# <a name="november-2020-announcements"></a>Comunicados de novembro de 2020

Esta página detalha os comunicados de novembro de 2020 sobre o Microsoft Partner Center.

Comunicados de 2020: [Abril](2020-april.md) | [Maio](2020-may.md) | [Junho](2020-june.md) | [Julho](2020-july.md) | [Agosto](2020-august.md) | [Setembro](2020-september.md) | [Outubro](2020-October.md) | Novembro

______________
## <a name="euefta-change-of-partner-billing-currency-for-new-commerce-offers"></a><a name="10"></a>Alteração da moeda de cobrança do parceiro da EU/EFTA para novas ofertas de comércio.  

### <a name="categories"></a>Categorias
- Data 2020-11-17
- Funcionalidades

### <a name="impacted-audience"></a>Público-alvo afetado  

Parceiros que fazem transações pelo programa de Provedor de Soluções na Nuvem na região EU/EFTA 

### <a name="summary"></a>Resumo 

Na região EU (União Europeia)/EFTA (Associação Europeia de Livre Comércio), todas as novas ofertas de comércio no programa Provedor de Soluções na Nuvem usarão o local de cobrança do parceiro, em vez do local de cobrança do cliente. Isso significa que os parceiros serão cobrados pela Microsoft com base na moeda do local em que eles estão, não na moeda do local dos clientes. Isso será feito em duas fases: 

- **Fase 1: novos clientes comprando uma nova oferta de comércio no CSP**

A partir de janeiro de 2021, os parceiros cujos novos clientes comprarem novas ofertas de comércio serão cobrados por essas compras na moeda do local do parceiro. Parceiros com clientes existentes que já compraram novas ofertas de comércio no CSP continuarão sendo cobrados na moeda do local de cobrança do cliente durante essa fase. 

 

- **Fase 2: clientes existentes que compraram uma nova oferta de comércio no CSP antes de janeiro de 2021** 

Após a Fase 1 e durante o ano de 2021, a Microsoft fará a transição da cobrança de novas ofertas de comércio para parceiros com clientes existentes, que compraram uma nova oferta de comércio no CSP antes de janeiro de 2021. Essa transição será da moeda do local do cliente para a moeda do local do parceiro. Os parceiros serão notificados com antecedência antes que essa alteração seja implementada.  

>[Observação] Essa alteração afetará apenas a moeda de cobrança do parceiro, e não o preço de novas ofertas de comércio no CSP. 

As novas ofertas de comércio no escopo para essa alteração são: Assinaturas do Azure que fazem parte de um plano do Azure, reservas do Azure, assinaturas de servidor, software perpétuo e compras do marketplace comercial da Microsoft no programa do Provedor de Soluções na Nuvem.

### <a name="partner-benefits"></a>Benefícios do parceiro  

- Essa atualização reduzirá a complexidade e a sobrecarga com o faturamento em várias moedas na região EU/EFTA para a nova experiência de comércio.  

- Os parceiros receberão uma fatura consolidada em uma moeda e não receberão mais uma fatura para cada moeda do local do cliente. 

- Os pagamentos de incentivos estarão na mesma moeda que a moeda da fatura do parceiro.

- Os parceiros perceberão que a cobrança ficou menos complexa devido ao faturamento em várias moedas; isso vai liberar tempo e recursos associados atualmente à reconciliação de contas. 

- Para parceiros que ainda não adotaram novas ofertas de comércio, essa alteração se alinha com o modelo de cobrança de parceiro anterior, permitindo que os parceiros façam uma transição mais fácil para a nova experiência de comércio no CSP. 

### <a name="resources"></a>Recursos 

Examine as informações sobre esse tópico na [Galeria de Operações](https://partner.microsoft.com/resources/collection/eu-efta-changes-collection#/ no site de parceiros da Microsoft.  

## <a name="api-throttling-to-partners-calling-partner-center-apis"></a><a name="9"></a>Limitação de API para parceiros que chamam as APIs do Partner Center

### <a name="categories"></a>Categorias

- Data 2020-11-17
- Capacidades

### <a name="summary"></a>Resumo

A Microsoft está introduzindo a limitação de API a parceiros que chamam APIs do Partner Center para oferecer um desempenho mais consistente dentro de um determinado período de tempo.

### <a name="impacted-audience"></a>Público-alvo afetado

Parceiros que fazem transações pelo programa de Provedor de Soluções na Nuvem

### <a name="details"></a>Detalhes

A Microsoft está implementando a limitação de API no primeiro trimestre de 2021 para possibilitar um desempenho mais consistente dentro de um período de tempo para parceiros que chamam as APIs do Partner Center. A limitação restringe o número de solicitações a um serviço dentro de um determinado período de tempo para evitar o uso excessivo de recursos. Quando um limite for excedido, o Partner Center limitará solicitações adicionais desse cliente durante um período de tempo.  

### <a name="partner-benefits"></a>Benefícios do parceiro 

O Partner Center foi criado para lidar com um alto volume de solicitações, mas se um número excessivo delas for realizado por alguns parceiros, a limitação ajudará a manter o desempenho ideal e a confiabilidade para todos os parceiros. Isso garante um tempo de inatividade mínimo. Reduzindo o alto volume de solicitações, podemos garantir um desempenho consistente para todos os parceiros. 


### <a name="apis-to-be-throttled"></a>APIs a serem limitadas

|**Operação**|**Documentação do Partner Center**|
|-------------------------|----------------------------------|
|{baseURL}/v1/customers/{ID_do_cliente}/subscriptions|[Obter as assinaturas de um cliente](https://docs.microsoft.com/partner-center/develop/get-all-of-a-customer-s-subscriptions)|  
|{baseURL}/v1/customers/{ID_do_cliente}/subscriptions/{ID_da_assinatura}|[Obter uma assinatura por ID](https://docs.microsoft.com/partner-center/develop/get-a-subscription-by-id) | 
|{baseURL}/v1/customers/{ID_do_cliente}/orders||[Obter todos os pedidos de um cliente](https://docs.microsoft.com/artner-center/develop/get-all-of-a-customer-s-orders)|  
|{baseURL}/v1/customers/{ID_do_cliente}/orders/{ID_do_pedido}|[Obter uma ordem por ID](https://docs.microsoft.com/partner-center/develop/get-an-order-by-id)|  
|{baseURL}/v1/customers/{ID_do_cliente}/orders/{ID_do_pedido}/provisioningstatus|[Obter o status de provisionamento da assinatura](https://docs.microsoft.com/partner-center/develop/get-subscription-provisioning-status)|  
|{baseURL}/v1/customers/{ID_do_cliente}/subscriptions/{ID_da_assinatura}|[Gerenciar pedidos e uma assinatura](https://docs.microsoft.com/partner-center/develop/manage-orders#manage-a-subscription)| 
|{baseURL}/v1/customers/{ID_do_cliente}/subscriptions/{ID_da_assinatura}/addons|[Obter uma lista de complementos de uma assinatura](https://docs.microsoft.com/partner-center/develop/get-a-list-of-add-ons-for-a-subscription)| 
|{baseURL}/v1/customers/{ID_do_cliente}/subscriptions/{ID_da_assinatura}/azureEntitlements|[Obter uma lista de direitos do Azure para uma assinatura](https://docs.microsoft.com/partner-center/develop/get-a-list-of-azure-entitlements-for-subscription)|  
|{baseURL}/v1/customers/{ID_do_cliente}/subscriptions/{ID_da_assinatura}/registrationstatus|[Obter o status de registro de assinatura](https://docs.microsoft.com/partner-center/develop/get-subscription-registration-status)| 
|{baseURL}/v1/customers/{ID-do-locatário-do-cliente}/transfers|[Obter todas as transferências de um cliente](https://docs.microsoft.com/partner-center/develop/get-subscription-registration-status)| 
|{baseURL}/v1/productUpgrades/{ID-da-atualização}/status|[Obter o status de atualização do produto](https://docs.microsoft.com/partner-center/develop/get-all-of-a-customer-s-transfers)| 
|{baseURL}/v1/customers/{ID-do-cliente}/subscriptions/{ID-da-assinatura}/conversions|[Obter uma lista de ofertas de conversão de avaliação](https://docs.microsoft.com/partner-center/develop/get-all-of-a-customer-s-transfers) 
  

O objetivo deste comunicado é fazer os parceiros conhecerem antecipadamente as alterações futuras, permitindo, assim, que eles se preparem. É altamente recomendável que os parceiros se familiarizem com essas APIs e considerem o uso da API do log de atividades para ter mais eficiência e evitar a limitação. Para obter mais informações sobre esse recurso, veja os detalhes em [Diretrizes de limitação de API](https://docs.microsoft.com/partner-center/develop/api-throttling-guidance). 

### <a name="next-steps"></a>Próximas etapas

Examine as [Diretrizes de limitação de API](https://docs.microsoft.com/partner-center/develop/api-throttling-guidance) e execute as etapas necessárias. 



## <a name="409-errors-due-to-duplicate-mca-requests"></a><a name="8"></a>409 erros devido a solicitações de MCA duplicadas

### <a name="categories"></a>Categorias

- Data 2020-11-16
- Funcionalidades

### <a name="context"></a>Contexto

- Em fevereiro deste ano, foi solicitado que os parceiros assinassem o MCuA (Contrato de Cliente da Microsoft). Ele era uma migração do antigo MCA (Contrato do Microsoft Cloud). 
- Como parte dessa mudança, foi solicitado que os parceiros incluíssem o parâmetro Type do contrato conforme documentado [aqui](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-agreement).

### <a name="what-happened-next"></a>O que aconteceu depois:

- Nem todos os parceiros incluíram a solicitação de parâmetro na implementação. A Microsoft retornou o MCA a esses parceiros.
- Em seguida, o parceiro reenviaria a solicitação de assinatura ao cliente e reenviaria o MCA à Microsoft. 
- A duplicação afetou a capacidade da Microsoft de fornecer o serviço aos parceiros.
- Em setembro de 2020, enviamos uma notificação aos parceiros, por meio do Yammer em vários fóruns, solicitando que eles corrigissem o parâmetro. A Microsoft não poderia mais aceitar as duplicatas e eles receberiam erros 409.

>[Observação] Isso NÃO era um novo contrato/uma alteração de API para os parceiros.

- Em outubro, trabalhamos em conjunto com os parceiros que tiveram a maioria das solicitações duplicadas a fim de corrigir o problema.
- Atualmente, estamos lembrando os parceiros e enviando emails pessoais para os 10 principais infratores para que eles examinem as solicitações e entrem em contato conosco para podermos ajudá-los a testar e a resolver o problema.
- Em 10 de novembro de 2020, paramos de aceitar duplicatas, e os parceiros que não tinham corrigido os parâmetros receberam erros 409.
- Desde então, revertemos a alteração de não aceitar duplicatas. 
- No entanto, em 14 de janeiro de 2021, não aceitaremos mais duplicatas. Isso permite que os parceiros tenham mais tempo para fazer os ajustes da parte deles. Já recebemos uma notificação de um parceiro de que ele planejava implantar uma atualização em 16/11, na qual trabalhamos em conjunto com ele.
- Pedimos que os parceiros entrem em contato conosco para podermos ajudá-los a fazer o teste adicionando os locatários deles a um pacote de pré-lançamento com as alterações. Assim, eles poderão garantir que a atualização da solução deles funcione conforme o esperado.



## <a name="testing-available-partner-center-api-updates-and-user-interface-ui-enhancements-for-the-education-customer-validation-process"></a><a name="7"></a>Testes disponíveis: atualizações de API do Partner Center e aprimoramentos da IU (interface do usuário) para obter o processo de validação do cliente de Educação

### <a name="categories"></a>Categorias

- Data 2020-11-10
- Funcionalidades | Escala e Eficiência da Unidade

### <a name="impacted-audience"></a>Público-alvo afetado

Os parceiros que vendem ofertas Acadêmicas por meio do programa CSP (Provedor de Soluções na Nuvem).

### <a name="summary"></a>Resumo

Os testes já estão disponíveis para atualizações de API do Partner Center e aprimoramentos da interface do usuário para obter o processo de validação do cliente de Educação.

### <a name="details"></a>Detalhes

O trabalho da Microsoft é baseado em confiança. Temos o compromisso de fornecer um método de validação do cliente que esteja em conformidade e que seja seguro e protegido para obter negociações de ofertas Acadêmicas no programa CSP. Como parte disso, estamos introduzindo a API do Partner Center e os aprimoramentos de interface do usuário no segundo trimestre deste ano fiscal (FY21 Q2). Esses aprimoramentos aumentarão a clareza e a visibilidade sobre o processo de validação do cliente, bem como a capacidade de inserir dados mais precisos, o que levará ao sucesso na validação do cliente.

**Aprimoramentos do Partner Center**

- Novas APIs de Qualificações GET e POST para dar suporte à entrada de dados precisos e aprimorar o processo de validação do cliente de Educação da Microsoft.

- Aprimoramentos na interface do usuário para dar suporte à entrada de dados precisos e aprimorar o processo de validação do cliente de Educação realizado pela Microsoft.

Testes.

Para obter uma maior compreensão sobre as APIs e a entrada de dados necessárias para obter êxito na validação do cliente, os parceiros poderão testar esses aprimoramentos de outubro de 2020. Forneceremos mais detalhes em breve sobre como e quando participar. As APIs existentes do Partner Center serão desativadas antes do fim do segundo trimestre do ano fiscal de 2021. Nesse momento, você precisará fazer a transição para as novas APIs do Partner Center.

   - Testes disponíveis: as datas para teste de parceiro são de 2 de outubro a 2 de dezembro de 2020. Os parceiros que desejam participar deverão baixar o guia de testes do cliente de Educação do Partner Center para saber como se preparar, como se inscrever e o que esperar durante a fase de testes.

**Clientes de biblioteca e museu**

Além desses aprimoramentos, estamos empolgados em anunciar que, no segundo trimestre do ano fiscal de 2021, habilitaremos ofertas com preços Acadêmicos para clientes de Biblioteca e Museu, expandindo os clientes de Educação com os quais você pode realizar transações de ofertas CSP.

A Microsoft reserva a si o direito de examinar o status de qualquer cliente ou cliente proposto como um usuário de Educação qualificado. Para obter detalhes completos, veja os [Requisitos de Usuário para obter uma Educação Acadêmica Qualificada](https://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=7).

## <a name="next-steps"></a>Próximas etapas

Examine as novas alterações na interface do usuário e na API do Partner Center, além do Guia de Testes na [coleção de conteúdo de aprimoramentos do processo de validação do cliente de Educação do Partner Center](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/)

• Inscreva-se para participar de testes. Confira [Guia de Testes](https://partner.microsoft.com/resources/detail/partner-center-edu-testing-guide-pdf) para obter detalhes. 

• Verifique se sua organização está familiarizada com os [Requisitos de Usuário para obter uma Educação Acadêmica Qualificada](https://www.microsoftvolumelicensing.com/DocumentSearch.aspx?Mode=3&DocumentTypeId=7). 

• Compartilhe essas informações com as equipes apropriadas em sua organização, juntamente com seus revendedores para ajudá-los a se preparar para essas alterações.



## <a name="expanding-commercial-licensing-partner-content-on-the-operations-readiness-gallery"></a><a name="6"></a>Como expandir o conteúdo do parceiro de licenciamento comercial na Galeria de Preparação de Operações

### <a name="categories"></a>Categorias

- Data: 2020-11-5
- Capacidades

### <a name="summary"></a>Resumo

Desde 5 de novembro de 2020, o conteúdo do parceiro de licenciamento comercial do Partner University também está disponível na Galeria de Preparação de Operações.

### <a name="impacted-audience"></a>Público-alvo afetado

Parceiros comerciais

### <a name="details"></a>Detalhes

Desde 5 de novembro de 2020, o conteúdo do parceiro de licenciamento comercial do Partner University também está disponível na Galeria de Preparação de Operações. Isso consolida o conteúdo de lançamento do parceiro de licenciamento comercial e operacional já existente na Galeria de Preparação de Operações com nosso conteúdo permanente do parceiro de licenciamento comercial do Partner University. Portanto, isso fornecerá aos parceiros uma experiência de preparação mais direta. As seguintes coleções foram adicionadas à Galeria de Preparação de Operações:

- [Microsoft Azure – Ofertas e Licenciamento](https://partner.microsoft.com/resources/collection/microsoft-azure-offers-and-licensing#/)
- [Licenciamento comercial – Chamada de destaque do CSP](https://partner.microsoft.com/resources/collection/commercial-licensing-csp-spotlight-call#/)
- [Licenciamento comercial – Chamada de atualizações de licenciamento](https://partner.microsoft.com/resources/collection/commercial-licensing-licensing-updates-call#/)

### <a name="next-steps"></a>Próximas etapas

Compartilhe essas informações com todos os contatos adequados na sua organização.

________________

## <a name="microsoft-teams-rooms-premium-sku-launch"></a><a name="5"></a>Lançamento do SKU Premium das Salas do Microsoft Teams

### <a name="categories"></a>Categorias

- Data: 2020-11-3
- Ofertas/mercados

### <a name="summary"></a>Resumo

O SKU Premium das Salas do Microsoft Teams para o Microsoft Teams por meio do programa CSP (Provedor de Soluções na Nuvem) já está disponível.

### <a name="impacted-audience"></a>Público-alvo afetado

Todos os parceiros que fazem transações pelo programa CSP (Provedor de Soluções na Nuvem)

### <a name="details"></a>Detalhes

O novo SKU Premium das Salas do Microsoft Teams para as Salas do Microsoft Teams já está disponível para seus clientes que adquirem o CSP com você, por US$ 50 por dispositivo por mês. O SKU Premium das Salas do Microsoft Teams é uma alternativa ao SKU Standard das Salas do Microsoft Teams (chamada anteriormente de licença de Sala de Reunião). Esse SKU inclui tudo que faz parte da oferta Standard, como as licenças necessárias para o Microsoft Teams, o Skype for Business Online e o gerenciamento do Intune. A oferta também habilita o Sistema Telefônico, necessário para integração de PSTN (Rede Telefônica Pública Comutada), e a Audioconferência quando disponível. 

Com a oferta Premium, os clientes têm acesso aos recém-lançados Serviços Gerenciados das Salas do Microsoft Teams, nos quais especialistas cuidam do gerenciamento e das operações das salas de reunião em nome do cliente. Esse serviço de monitoramento e gerenciamento de TI baseado em nuvem mantém os dispositivos de Salas do Microsoft Teams e os periféricos delas atualizados e seguros. Eles também são monitorados e gerenciados proativamente, mantendo um ambiente otimizado para uma excelente experiência na sala.

#### <a name="released-at-launch"></a>Liberado no lançamento

   |****|**Salas do Microsoft Teams Standard – US$ 15 por dispositivo por mês**|**Salas do Microsoft Teams Premium – US$ 50 por dispositivo por mês**|
   |-------------------|:------|:------|
   |Skype for Business|Yes| |
   |Microsoft Teams|Sim|Sim|
   |Sistema de Telefonia|Sim|Sim|
   |Audioconferência|Sim|Sim|
   |Microsoft Intune|Sim|Sim|
   | |Salas do Microsoft Teams Standard – US$ 15 por dispositivo por mês|Salas do Microsoft Teams Premium – US$ 50 por dispositivo por mês|
   |Serviços Gerenciados das Salas do Microsoft Teams| |Yes|
   |Disponibilidade mundial|Yes|Mercados selecionados|

#### <a name="microsoft-teams-rooms-managed-services"></a>Serviços Gerenciados das Salas do Microsoft Teams

- Gerenciamento proativo: gerenciamento ininterrupto de seus sistemas de salas, incluindo aplicação de patches, gerenciamento de configuração e muito mais.
•   Monitoramento e análise da causa raiz em tempo real: Monitoramento e detecção, com resposta de gerenciamento de incidentes orquestrada controlada pela Microsoft em coordenação com o cliente, quando necessário. O aplicativo móvel permite que você receba alertas em qualquer lugar.
- Atualizações gerenciadas: Gerenciamento e fornecimento de atualizações de aplicativos, KB do Windows e firmware.
- Proteção contra ameaças à segurança: proteção contra ameaças por meio da Proteção Avançada contra Ameaças do Microsoft Defender.
- Atendimento ao cliente: suporte ininterrupto por meio de tíquetes em nosso centro de operações de serviços dedicado, com correção de incidente assistida para casos não automatizados. Controle de acesso baseado em função granular.
- Insights e recomendações: Insights agregados entre clientes e relatórios sobre a integridade da sala, o estoque, o uso, as reuniões online e as tendências de incidentes.

#### <a name="offer-details"></a>Detalhes da oferta

   |**Nome da oferta**|**ID da oferta**|**ID do material**|
   |-------------------|:------|:------|
   |Salas do Teams Premium|5db9aa31-f039-4740-b122-a33514e4c492|6XB-00007|
   |Salas do Teams Premium (EUA e CAN)|03070f91-cc77-4c2e-b269-4a214b3698ab|6XB-00008|
   |Salas do Teams Premium para docentes|d0c9a9a9-c9b6-41d7-9148-b60115c36c95|6Y5-00005|

### <a name="next-steps"></a>Próximas etapas

- Familiarize-se com a nova oferta e a disponibilidade geográfica dela. Acesse as [perguntas frequentes]().
- Familiarize-se com a nova oferta e a disponibilidade geográfica dela. 
- Saiba mais sobre as Salas da Microsoft e as ofertas relacionadas em [Salas do Microsoft Teams](https://rooms.microsoft.com/).
- Use o [Guia do Parceiro do Teams](https://aka.ms/teamscallingmeetingsguide) para desenvolver sua prática com as Salas de Reunião do Teams e criar uma oferta pronta para venda conjunta.
- Analise as [Perguntas frequentes sobre as Salas do Microsoft Teams](https://aka.ms/PartnerMTRFAQ) para saber mais sobre a solução e os serviços do produto. 
- Compartilhe essas informações com todos os contatos adequados em sua organização e entenda as oportunidades de venda adicional e cruzada.

________________

## <a name="new-microsoft-teams-advanced-communications-skus-for-government-community-cloud-gcc-coming-soon"></a><a name="4"></a>Novas SKUs de Comunicações Avançadas do Microsoft Teams para a GCC (Nuvem da Comunidade Governamental) estarão disponíveis em breve

### <a name="categories"></a>Categorias

- Data: 2/11/2020
- Ofertas/mercados

### <a name="summary"></a>Resumo

O novo SKU do complemento Comunicações Avançadas para o Microsoft Teams no GCC estarão disponíveis em 1º de dezembro de 2020.

### <a name="impacted-audience"></a>Público-alvo afetado

Todos os parceiros que fazem transações pelo programa CSP (Provedor de Soluções na Nuvem)

### <a name="details"></a>Detalhes

O novo complemento Comunicações Avançadas para o Microsoft Teams no GCC já está disponível pelo valor de US$ 12 por usuário/mês. Os SKUs do complemento podem ser comprados adicionalmente a qualquer outro pacote do Microsoft 365 que contenha o Microsoft Teams. O complemento Comunicações Avançadas fornece um novo conjunto de funcionalidades para grandes reuniões, políticas de comunicação, integrações e ferramentas avançadas para o gerenciamento de TI. 

#### <a name="offer-details"></a>Detalhes da oferta

   |**Nome da oferta**|**ID da oferta**|**ID do material**|
   |-------------------|:------|:------|
   |Comunicações Avançadas para GCC|56fe76f5-f4ba-4fac-9561-d0daf59b01a1|7FB-00003|

#### <a name="frequently-asked-questions"></a>Perguntas frequentes 

**O que é o recurso Comunicações Avançadas?** Esse novo complemento do Microsoft Teams permite que os clientes aprimorem ainda mais a experiência de comunicação. Ele pode ser adquirido adicionalmente a qualquer SKU do Microsoft 365 no qual os clientes estejam inscritos.

**Quanto custa?** O ERP comercial custa US$ 12 por usuário/por mês.

**Quais clientes podem comprar o complemento?** Os clientes do GCC podem comprar o complemento.

**Como poderá ser adquirido?** O complemento pode ser adquirido por meio do Contrato Enterprise, da Assinatura do Contrato Enterprise, do Enrollment for Education Solutions, do CSP ou do Web Direct.

**Onde pode ser vendido?** Ele pode ser vendido em mercados dos EUA.

**Quais são os pré-requisitos?** Qualquer pacote do Microsoft 365 ou do Office 365 que inclua o Microsoft Teams pode ter esse complemento.

### <a name="next-steps"></a>Próximas etapas

Compartilhe essas informações com os contatos relevantes em sua organização e entenda as oportunidades de venda adicional e cruzada. Examine a seção de recursos do [Guia do parceiro do Teams](https://aka.ms/teamscallingmeetingsguide).

________________

## <a name="dynamics-365-recently-launched-and-upcoming-new-offers-and-products"></a><a name="3"></a>Dynamics 365: Ofertas e produtos lançados recentemente e futuros

### <a name="categories"></a>Categorias

- Data: 2/11/2020
- Ofertas/mercados

### <a name="impacted-audience"></a>Público-alvo afetado

Provedores diretos, provedores indiretos e revendedores indiretos

### <a name="details"></a>Detalhes

#### <a name="new-offers"></a>Novas ofertas

Em 1º de novembro de 2020, a Microsoft lançou as ofertas do Dynamics 365 Project Operations e removeu o Dynamics 365 PSA (Project Service Automation) para clientes comerciais. Essa comunicação fornece informações adicionais sobre o mapeamento de direitos de uso duplo desse lançamento e as novas ofertas inseridas do ISV (fornecedor independente de software).

#### <a name="project-operations-isv-embed-offers"></a>Ofertas inseridas do ISV do Project Operations

Em 1º de novembro de 2020, a Microsoft lançou três ofertas inseridas do ISV de 36 meses para o Dynamics 365 for Project Operations para clientes do CSP (Provedor de Soluções na Nuvem). Veja a guia Project Operations do documento do Excel [Ofertas do Dynamics CSP – novembro de 2020](https://partner.microsoft.com/resources/detail/dynamics-csp-offers-november-xls) para obter os detalhes do SKU.

#### <a name="project-operations-dual-use-rights-mapping"></a>Mapeamento de direitos de uso duplo do Project Operations

Você pode encontrar mais informações sobre o mapeamento de direitos de uso duplo local do Dynamics 365 das ofertas do Project Operations na seguinte tabela:

   |**Oferta do D365 Operations**|**Mapeamento de direitos de uso duplo local do D365**|
   |-------------------|:------|
   |Oferta do D365 Operations|Mapeamento de direitos de uso duplo local do D365|
   |D365 Project Operations|D365 for Operations, local (servidor do AX) que usa o SKU do Dyn365 Project Operations (109108477)|
   |D365 Project Operations Attach|D365 for Operations, local (servidor do AX) que usa o SKU do Dyn365 Project Operations (109108477)|
   |D365 Finance com Project Operations|D365 for Operations, local (servidor do AX) que usa o SKU do Dyn365 Project Operations (109108477)|
   |D365 Finance Attach com Project Operations|D365 for Operations, local (servidor do AX) que usa o SKU do Dyn365 Project Operations (109108477)|
   |D365 Unified Operations – Atividade com o Project Operations|D365 for Operations, local (servidor do AX) que usa o SKU do Dyn365 Project Operations (109108477)|

#### <a name="previously-announced"></a>Anunciado anteriormente

Em 1º de novembro de 2020, a Microsoft lançou as seguintes ofertas e produtos novos e atualizados do Dynamics 365 e da Power Platform para CSP:

- USL do Dynamics 365 Customer Voice 

Examine a guia Project Operations do documento do Excel [Ofertas do Dynamics CSP – novembro de 2020](https://partner.microsoft.com/resources/detail/dynamics-csp-offers-november-2020-xls) para obter os detalhes da ID da oferta.

Você pode encontrar mais recursos na home page do Microsoft Dynamics 365 Customer Voice.

### <a name="next-steps"></a>Próximas etapas

Compartilhe essas informações com as pessoas relevantes na sua organização.

________________

## <a name="introducing-microsoft-365-business-voice-for-nonprofit-organizations"></a><a name="2"></a>Apresentamos o Microsoft 365 Business Voice para organizações sem fins lucrativos

### <a name="categories"></a>Categorias

- Data: 2/11/2020
- Ofertas/mercados

### <a name="summary"></a>Resumo

Em 1º de novembro de 2020, a Microsoft apresentou novos SKUs para o Microsoft 365 Business Voice para organizações sem fins lucrativos.

### <a name="impacted-audience"></a>Público-alvo afetado

Provedores diretos, provedores indiretos e revendedores indiretos

### <a name="details"></a>Detalhes

Em 1º de novembro de 2020, a Microsoft apresentou novos SKUs para o Business Voice. O pacote completo está disponível no Canadá, no Reino Unido e nos Estados Unidos. O Business Voice sem Plano de Chamadas estará disponível em todos os outros mercados. 

O Microsoft 365 Business Voice é um sistema de telefonia baseado em nuvem e integrado ao Office 365 para empresas de pequeno e médio porte. Adicionar o Business Voice à assinatura do Office 365 de um cliente fornecerá uma solução completa de comunicação e colaboração com chamadas, chats e reuniões em um aplicativo, o Microsoft Teams.

Confira a lista de preços para obter mais detalhes.

O Microsoft 365 Business Voice pode ser adicionado às seguintes assinaturas para até 300 usuários:

- Office 365: Business Essentials, Business Premium, A1, E1, A3 e E3
- Microsoft 365: Business, A3 e E3


### <a name="next-steps"></a>Próximas etapas

- Familiarize-se e compartilhe as informações na lista de preços da versão prévia com todos os contatos apropriados da sua organização. 
- Examine todos os materiais de preparação na galeria de recursos Atualizações do Programa de Provedor de Soluções na Nuvem: [Apresentamos o Microsoft 365 Business Voice para pequenas e médias empresas](https://partner.microsoft.com/resources/collection/m365-voice-smb#/). 

________________

## <a name="cloud-solution-provider-csp-promo-for-microsoft-365-business-voice-is-now-available"></a><a name="1"></a>A promoção do CSP (Provedor de Soluções na Nuvem) para Microsoft 365 Business Voice já está disponível

### <a name="categories"></a>Categorias

- Data: 2/11/2020
- Ofertas/mercados

### <a name="summary"></a>Resumo

Preços com desconto disponíveis para as assinaturas que estão sendo renovadas e as novas do Microsoft 365 Business Voice com Plano de Chamadas e o Microsoft 365 Business Voice sem Plano de Chamadas.

### <a name="impacted-audience"></a>Público-alvo afetado

Todos os parceiros que fazem transações por meio do programa CSP

### <a name="details"></a>Detalhes

De 1º de novembro de 2020 até 30 de abril de 2021, as novas assinaturas e a renovação da assinatura do Microsoft 365 Business Voice com Plano de Chamadas e o Microsoft 365 Business Voice sem Plano de Chamadas estão sujeitas a preços com descontos. O Microsoft 365 Business Voice com Plano de Chamadas está sujeito a um desconto de 25% por 12 meses e o Microsoft 365 Business Voice sem Plano de Chamadas está sujeito a um desconto de 33% por 12 meses. 

#### <a name="offer-details"></a>Detalhes da oferta

   |**Nome da oferta**|**ID da oferta**|**ID do material**|
   |-------------------|:------|:------|
   |Promoção de adoção do Microsoft 365 Business Voice|e7d1d0fa-b769-45c7-aaea-c3e6f7402691|PZX-00006|
   |Promoção de adoção do Microsoft 365 Business Voice|ef3ff6bb-a288-4a56-9204-97b37ff9a0b8|PZW-00019|
   |Promoção de adoção do Microsoft 365 Business Voice (EUA)|4244aed3-90ae-4754-8dc8-37f2e8d84e85|PZW-00020|
   |Promoção de adoção do Microsoft 365 Business Voice (sem o plano de chamadas)|b71df433-6fd9-4549-886d-577f7aa06070|PZY-00019|
   |Promoção de adoção do Microsoft 365 Business Voice (sem o plano de chamadas)|4ba4d580-4902-42b0-8411-a27358dd5405|PZY-00016|
   |Promoção de adoção do Microsoft 365 Business Voice (sem o plano de chamadas)|bbfd896b-e3d4-45ba-9319-14104d400069|PZY-00018|
   |Microsoft 365 Business Voice (sem Plano de Chamadas) para a promoção de adoção dos EUA|9b05d0b7-cfb4-42f1-9cc3-f698dba2838e|PZY-00017|

Essas promoções afetarão os seguintes clientes:

- Novos locatários líquidos do cliente
- Os locatários existentes do cliente que não têm assinaturas ativas nem canceladas recentemente (nos últimos 30 dias) em uma licença do Business Voice ou de Audioconferência no CSP, no Web Direct ou em outro canal comercial da Microsoft

#### <a name="additional-resources"></a>Recursos adicionais

- Visite a [página do parceiro do Microsoft 365 Business Voice](https://www.microsoft.com/microsoft-365/partners/businessvoice) para saber mais sobre o Business Voice. 
- Saiba mais sobre essa promoção nas [Perguntas frequentes do parceiro](https://www.microsoft.com/microsoft-365/partners/resources/faq-business-voice-audio-conferencing-promo) relacionadas.

### <a name="next-steps"></a>Próximas etapas

- Familiarize-se com as oportunidades promocionais de reuniões e chamadas e compartilhe essas informações com todos os contatos apropriados na sua organização.
- Incorpore essas promoções nas suas estratégias de vendas do Microsoft 365.
- Promova a conscientização entre os clientes sobre o valor da adição do Business Voice ao Teams. 

________________
