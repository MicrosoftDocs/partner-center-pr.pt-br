---
title: Comunicados de abril de 2021
description: Comunicados de abril de 2021 sobre o Microsoft Partner Center, incluindo novas funcionalidades, promoções, ofertas, mercados ou alterações nas ofertas anteriores.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: brentserbus
ms.author: brserbus
ms.custom:
- announcement
- references_regions
ms.localizationpriority: high
ms.date: 04/29/2021
ms.openlocfilehash: d26d1af994ae9a3f951ee9428ee6fd092b2c91d8
ms.sourcegitcommit: 6c20c3cc4a226cada70c56df295966696affcec8
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/30/2021
ms.locfileid: "108328042"
---
# <a name="april-2021-announcements"></a><span data-ttu-id="759dc-103">Comunicados de abril de 2021</span><span class="sxs-lookup"><span data-stu-id="759dc-103">April 2021 announcements</span></span>

<span data-ttu-id="759dc-104">Esta página apresenta os comunicados de abril de 2021 sobre o Microsoft Partner Center.</span><span class="sxs-lookup"><span data-stu-id="759dc-104">This page provides the announcements for Microsoft Partner Center for April 2021.</span></span>

## <a name="readiness-updated-csp-customer-address-validation-api-going-live-in-june-testing-capability-now-available"></a><a name="10"></a><span data-ttu-id="759dc-105">Preparação: atualização da API de validação de endereço do cliente do CSP entrará em vigor em junho; funcionalidade de teste disponível</span><span class="sxs-lookup"><span data-stu-id="759dc-105">Readiness: Updated CSP customer address validation API going live in June; testing capability now available</span></span>

### <a name="categories"></a><span data-ttu-id="759dc-106">Categorias</span><span class="sxs-lookup"><span data-stu-id="759dc-106">Categories</span></span>

- <span data-ttu-id="759dc-107">Data: 30/04/2021</span><span class="sxs-lookup"><span data-stu-id="759dc-107">Date: 2021-04-30</span></span>
- <span data-ttu-id="759dc-108">Preparação</span><span class="sxs-lookup"><span data-stu-id="759dc-108">Readiness</span></span>

### <a name="summary"></a><span data-ttu-id="759dc-109">Resumo</span><span class="sxs-lookup"><span data-stu-id="759dc-109">Summary</span></span>

<span data-ttu-id="759dc-110">Para ajudar parceiros e clientes a conduzir os negócios com confiança, convidaremos os parceiros a testar as alterações na API de Validação de Endereço em todos os países do mundo.</span><span class="sxs-lookup"><span data-stu-id="759dc-110">To help partners and customers run their business based on trust, we’ll be inviting partners to test changes to the Validate Address API for all countries worldwide.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="759dc-111">Público-alvo afetado</span><span class="sxs-lookup"><span data-stu-id="759dc-111">Impacted audience</span></span>

<span data-ttu-id="759dc-112">Parceiros de cobrança direta e provedores indiretos do CSP que criam ou atualizam detalhes de endereços de clientes</span><span class="sxs-lookup"><span data-stu-id="759dc-112">CSP direct bill partners and indirect providers who create new or update existing customers’ address details</span></span>

### <a name="details"></a><span data-ttu-id="759dc-113">Detalhes</span><span class="sxs-lookup"><span data-stu-id="759dc-113">Details</span></span>

<span data-ttu-id="759dc-114">O trabalho da Microsoft é baseado em confiança.</span><span class="sxs-lookup"><span data-stu-id="759dc-114">Microsoft runs on trust.</span></span> <span data-ttu-id="759dc-115">Temos o compromisso de fornecer um método de validação de endereço do cliente que esteja em conformidade e que seja seguro e protegido para realizar transações de assinatura de clientes no programa CSP.</span><span class="sxs-lookup"><span data-stu-id="759dc-115">We’re committed to providing a compliant, safe, and secure method of customer address validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="759dc-116">Em 31 de março de 2021, introduzimos alterações na API de Validação de Endereço.</span><span class="sxs-lookup"><span data-stu-id="759dc-116">As of March 31, 2021, we have introduced changes to the Validate Address API.</span></span> <span data-ttu-id="759dc-117">Convidamos os parceiros a testar a API antes de seu lançamento no final de junho de 2021.</span><span class="sxs-lookup"><span data-stu-id="759dc-117">We invite partners to test the API prior to the  go-live at the end of June 2021.</span></span> 

<span data-ttu-id="759dc-118">Observe que essas alterações afetam somente a API de Validação de Endereço.</span><span class="sxs-lookup"><span data-stu-id="759dc-118">Note that these changes affect the Validate Address API only.</span></span> <span data-ttu-id="759dc-119">As APIs de Criação de Cliente e de Atualização de Perfil de Cobrança não são afetadas.</span><span class="sxs-lookup"><span data-stu-id="759dc-119">Create Customer and Update Billing Profile APIs aren’t affected.</span></span> <span data-ttu-id="759dc-120">Embora no momento o endereço sugerido não precise ser usado com a API de Criação de Cliente, é altamente recomendável.</span><span class="sxs-lookup"><span data-stu-id="759dc-120">Although the suggested address doesn’t currently have to be used with the Create Customer API, it’s highly recommended.</span></span>

<span data-ttu-id="759dc-121">A resposta retornará uma das seguintes mensagens de status:</span><span class="sxs-lookup"><span data-stu-id="759dc-121">The response will return one of the following status messages:</span></span>

| <span data-ttu-id="759dc-122">Status</span><span class="sxs-lookup"><span data-stu-id="759dc-122">Status</span></span>     | <span data-ttu-id="759dc-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="759dc-123">Description</span></span> |    <span data-ttu-id="759dc-124">O número de endereços sugeridos retornados</span><span class="sxs-lookup"><span data-stu-id="759dc-124">Number of suggested addresses returned</span></span> |
|-------|---------------|-------------------|
|<span data-ttu-id="759dc-125">Destino de entrega verificado</span><span class="sxs-lookup"><span data-stu-id="759dc-125">Verified shippable</span></span> | <span data-ttu-id="759dc-126">O endereço foi verificado e pode ser usado para entregas.</span><span class="sxs-lookup"><span data-stu-id="759dc-126">Address is verified and can be shipped to.</span></span> | <span data-ttu-id="759dc-127">Único</span><span class="sxs-lookup"><span data-stu-id="759dc-127">Single</span></span> |
|<span data-ttu-id="759dc-128">Verificado</span><span class="sxs-lookup"><span data-stu-id="759dc-128">Verified</span></span> | <span data-ttu-id="759dc-129">O endereço foi verificado.</span><span class="sxs-lookup"><span data-stu-id="759dc-129">Address is verified.</span></span> | <span data-ttu-id="759dc-130">Único</span><span class="sxs-lookup"><span data-stu-id="759dc-130">Single</span></span> |
|<span data-ttu-id="759dc-131">Interação necessária</span><span class="sxs-lookup"><span data-stu-id="759dc-131">Interaction required</span></span> | <span data-ttu-id="759dc-132">O endereço sugerido foi alterado significativamente e precisa de confirmação do usuário.</span><span class="sxs-lookup"><span data-stu-id="759dc-132">Suggested address has been changed significantly and needs user confirmation.</span></span> | <span data-ttu-id="759dc-133">Single</span><span class="sxs-lookup"><span data-stu-id="759dc-133">Single</span></span> |
|<span data-ttu-id="759dc-134">Rua parcial</span><span class="sxs-lookup"><span data-stu-id="759dc-134">Street partial</span></span> | <span data-ttu-id="759dc-135">A rua que consta no endereço é parcial e precisa de mais informações.</span><span class="sxs-lookup"><span data-stu-id="759dc-135">The given street in the address is partial and needs more info.</span></span> | <span data-ttu-id="759dc-136">Múltiplo – máximo de três</span><span class="sxs-lookup"><span data-stu-id="759dc-136">Multiple—maximum of three</span></span> |
|<span data-ttu-id="759dc-137">Local parcial</span><span class="sxs-lookup"><span data-stu-id="759dc-137">Premises partial</span></span> | <span data-ttu-id="759dc-138">O local determinado (número do prédio, número do conjunto, entre outros) é parcial e precisa de mais informações.</span><span class="sxs-lookup"><span data-stu-id="759dc-138">The given premises (building number, suite number, and others) are partial and need more info.</span></span> | <span data-ttu-id="759dc-139">Múltiplo – máximo de três</span><span class="sxs-lookup"><span data-stu-id="759dc-139">Multiple—maximum of three</span></span> |
|<span data-ttu-id="759dc-140">Vários</span><span class="sxs-lookup"><span data-stu-id="759dc-140">Multiple</span></span> | <span data-ttu-id="759dc-141">Há vários campos parciais no endereço (pode incluir rua parcial e local parcial).</span><span class="sxs-lookup"><span data-stu-id="759dc-141">There are multiple fields that are partial in the address (potentially also including street partial and premises partial).</span></span> | <span data-ttu-id="759dc-142">Múltiplo – máximo de três</span><span class="sxs-lookup"><span data-stu-id="759dc-142">Multiple—maximum of three</span></span> |
|<span data-ttu-id="759dc-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="759dc-143">None</span></span> | <span data-ttu-id="759dc-144">O endereço está incorreto.</span><span class="sxs-lookup"><span data-stu-id="759dc-144">Address is incorrect.</span></span> | <span data-ttu-id="759dc-145">Nenhum</span><span class="sxs-lookup"><span data-stu-id="759dc-145">None</span></span> |
|<span data-ttu-id="759dc-146">Não validado.</span><span class="sxs-lookup"><span data-stu-id="759dc-146">Not validated</span></span> | <span data-ttu-id="759dc-147">Não foi possível enviar o endereço pelo processo de validação.</span><span class="sxs-lookup"><span data-stu-id="759dc-147">Address was not able to be sent through the validation process.</span></span> | <span data-ttu-id="759dc-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="759dc-148">None</span></span> |

<span data-ttu-id="759dc-149">Os códigos postais dos EUA retornam mais quatro dígitos e um hífen, por exemplo, 12345-6789.</span><span class="sxs-lookup"><span data-stu-id="759dc-149">US post codes will return an additional four digits + hyphen, for example, 12345-6789.</span></span>

### <a name="next-steps"></a><span data-ttu-id="759dc-150">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="759dc-150">Next steps</span></span>

- <span data-ttu-id="759dc-151">Examine a documentação técnica e as perguntas frequentes na [coleção de parceiros dedicada](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) para obter diretrizes mais detalhadas.</span><span class="sxs-lookup"><span data-stu-id="759dc-151">Review the technical documentation and frequently asked questions in the [dedicated partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>
- <span data-ttu-id="759dc-152">Prepare-se para incorporar as alterações usando a experiência do usuário da Web e a API do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="759dc-152">Prepare to incorporate the changes using the Partner Center API and web user experience.</span></span> 
- <span data-ttu-id="759dc-153">Informe a ID de locatário de sua área restrita ao especialista (Ali Khaki) para participar do teste da versão de pré-lançamento e começar a se preparar para a atualização.</span><span class="sxs-lookup"><span data-stu-id="759dc-153">Share your sandbox tenant ID with the subject matter expert (Ali Khaki) to be included in the test flight, so that you can begin preparing for the update.</span></span> 
- <span data-ttu-id="759dc-154">Se estiver usando uma solução de CPV (fornecedor de painel de controle), consulte seu CPV.</span><span class="sxs-lookup"><span data-stu-id="759dc-154">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="759dc-155">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="759dc-155">Questions?</span></span>

<span data-ttu-id="759dc-156">Se precisar de suporte para suas operações com a Microsoft, entre em contato com o grupo do Yammer de suporte ao parceiro ou abra uma [solicitação de serviço](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span><span class="sxs-lookup"><span data-stu-id="759dc-156">If you need support for your operations with Microsoft, reach out to your partner support Yammer group or open a [service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

_______________
## <a name="new-location-for-partner-center-api-swagger-documentation"></a><a name="9"></a><span data-ttu-id="759dc-157">Novo local para a documentação do Swagger da API do Partner Center</span><span class="sxs-lookup"><span data-stu-id="759dc-157">New location for Partner Center API Swagger documentation</span></span>

### <a name="categories"></a><span data-ttu-id="759dc-158">Categorias</span><span class="sxs-lookup"><span data-stu-id="759dc-158">Categories</span></span>

- <span data-ttu-id="759dc-159">Data: 26/04/2021</span><span class="sxs-lookup"><span data-stu-id="759dc-159">Date: 2021-04-26</span></span>
- <span data-ttu-id="759dc-160">Funcionalidades</span><span class="sxs-lookup"><span data-stu-id="759dc-160">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="759dc-161">Resumo</span><span class="sxs-lookup"><span data-stu-id="759dc-161">Summary</span></span>

<span data-ttu-id="759dc-162">Os documentos do Swagger da API do Partner Center foram migrados do [site anterior de documentação do Swagger](https://apidocs.microsoft.com/services/partnercenter) para um [novo site de documentação do Swagger](https://docs.microsoft.com/rest/api/partner-center-rest/).</span><span class="sxs-lookup"><span data-stu-id="759dc-162">Partner Center API Swagger documents have been migrated from the [previous Swagger Documentation site](https://apidocs.microsoft.com/services/partnercenter) to a [new Swagger Documentation site](https://docs.microsoft.com/rest/api/partner-center-rest/).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="759dc-163">Público-alvo afetado</span><span class="sxs-lookup"><span data-stu-id="759dc-163">Impacted audience</span></span>

<span data-ttu-id="759dc-164">Parceiros de cobrança direta e provedores indiretos que participam do programa CSP (Provedor de Soluções na Nuvem) que estão usando as APIs do Partner Center</span><span class="sxs-lookup"><span data-stu-id="759dc-164">Direct bill partners and Indirect Providers participating in the Cloud Solution Provider (CSP) program who are using the Partner Center APIs</span></span>

### <a name="details"></a><span data-ttu-id="759dc-165">Detalhes</span><span class="sxs-lookup"><span data-stu-id="759dc-165">Details</span></span>

<span data-ttu-id="759dc-166">Desde 26 de abril de 2021, a documentação do Swagger da API do Partner Center, incluindo o conteúdo relacionado à API REST, está em um [novo site](https://docs.microsoft.com/rest/api/partner-center-rest/).</span><span class="sxs-lookup"><span data-stu-id="759dc-166">As of April 26, 2021 the Partner Center API Swagger documentation, including Rest API content, is located on a [new site](https://docs.microsoft.com/rest/api/partner-center-rest/).</span></span> <span data-ttu-id="759dc-167">O site antigo ficará inacessível após algumas semanas.</span><span class="sxs-lookup"><span data-stu-id="759dc-167">The old site will be inaccessible after several weeks.</span></span>

### <a name="benefits"></a><span data-ttu-id="759dc-168">Benefícios</span><span class="sxs-lookup"><span data-stu-id="759dc-168">Benefits</span></span>

<span data-ttu-id="759dc-169">A documentação do Swagger da API do Partner Center fornecerá uma função **Experimente**.</span><span class="sxs-lookup"><span data-stu-id="759dc-169">The Partner Center API Swagger documentation will provide a **Try It** function.</span></span> <span data-ttu-id="759dc-170">Para usar essa função, você precisará de um token de portador, que pode ser gerado seguindo as etapas listadas em [Autenticação do Partner Center](https://docs.microsoft.com/partner-center/develop/partner-center-authentication#app--user-authentication).</span><span class="sxs-lookup"><span data-stu-id="759dc-170">To use this function, you’ll need to have a Bearer Token, which you can generate by following the steps listed in [Partner Center Authentication](https://docs.microsoft.com/partner-center/develop/partner-center-authentication#app--user-authentication).</span></span>

### <a name="next-steps"></a><span data-ttu-id="759dc-171">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="759dc-171">Next steps</span></span>

<span data-ttu-id="759dc-172">Compartilhe essas informações em sua organização para que a equipe correta possa examinar e atualizar os processos delas.</span><span class="sxs-lookup"><span data-stu-id="759dc-172">Share this information within your organization so that the appropriate team can review and update their processes.</span></span>

### <a name="questions"></a><span data-ttu-id="759dc-173">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="759dc-173">Questions?</span></span>

<span data-ttu-id="759dc-174">Caso tenha dúvidas sobre essas ofertas, confira as comunidades relevantes no Yammer.</span><span class="sxs-lookup"><span data-stu-id="759dc-174">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="cloud-solution-provider-csp-software-return-period-policy-and-download-link-expiry-notice"></a><a name="8"></a><span data-ttu-id="759dc-175">Política de período de devolução e notificação de expiração do link de download de software do CSP (Provedor de Soluções na Nuvem)</span><span class="sxs-lookup"><span data-stu-id="759dc-175">Cloud Solution Provider (CSP) software return period policy and download link expiry notice</span></span>

### <a name="categories"></a><span data-ttu-id="759dc-176">Categorias</span><span class="sxs-lookup"><span data-stu-id="759dc-176">Categories</span></span>

- <span data-ttu-id="759dc-177">Data: 21-04-2021</span><span class="sxs-lookup"><span data-stu-id="759dc-177">Date: 2021-04-21</span></span>
- <span data-ttu-id="759dc-178">Funcionalidades</span><span class="sxs-lookup"><span data-stu-id="759dc-178">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="759dc-179">Resumo</span><span class="sxs-lookup"><span data-stu-id="759dc-179">Summary</span></span>

<span data-ttu-id="759dc-180">Há alterações na política de período de devolução e na expiração do link de download de software do CSP.</span><span class="sxs-lookup"><span data-stu-id="759dc-180">There are changes to the CSP software return period policy and download link expiry.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="759dc-181">Público-alvo afetado</span><span class="sxs-lookup"><span data-stu-id="759dc-181">Impacted audience</span></span>

<span data-ttu-id="759dc-182">Parceiros que fazem transações de ofertas de software perpétuo ou de assinatura de software no CSP</span><span class="sxs-lookup"><span data-stu-id="759dc-182">Partners transacting perpetual software or software subscription offers in CSP</span></span>

### <a name="details"></a><span data-ttu-id="759dc-183">Detalhes</span><span class="sxs-lookup"><span data-stu-id="759dc-183">Details</span></span>

<span data-ttu-id="759dc-184">Observe as seguintes notificações importantes sobre compras de software perpétuo ou de assinatura de software por meio do Partner Center:</span><span class="sxs-lookup"><span data-stu-id="759dc-184">Note the following important notifications regarding perpetual software and software subscription purchases through Partner Center:</span></span>

#### <a name="software-return-period-policy"></a><span data-ttu-id="759dc-185">Política de período de devolução de software</span><span class="sxs-lookup"><span data-stu-id="759dc-185">Software return period policy</span></span>

<span data-ttu-id="759dc-186">A partir de 1º de junho de 2021, o período de devolução de ofertas de software no CSP, conforme o MPA (Contrato de Parceiro da Microsoft), será alterado de 60 dias para 30 dias após a data do pedido.</span><span class="sxs-lookup"><span data-stu-id="759dc-186">From June 1, 2021, the return period for software offers in CSP, as stated in the Microsoft Partner Agreement (MPA), will change from 60 days from order date to 30 days from order date.</span></span>

<span data-ttu-id="759dc-187">Depois que um pedido de uma oferta de software for enviado, os parceiros terão 30 dias após a data do pedido para enviar revisões dele:</span><span class="sxs-lookup"><span data-stu-id="759dc-187">After an order for a software offer is submitted, partners will have 30 days from the order date to submit any revisions to such order:</span></span>

- <span data-ttu-id="759dc-188">Para todas as licenças de software perpétuo devolvidas dentro do período de devolução de 30 dias, o parceiro receberá um crédito completo no valor do preço de compra pago.</span><span class="sxs-lookup"><span data-stu-id="759dc-188">Any perpetual software license returned within the 30-day return period will receive a full credit of the paid purchase price.</span></span>

- <span data-ttu-id="759dc-189">Para todos os produtos de assinatura de software devolvidos dentro do período de devolução de 30 dias, o parceiro receberá um crédito proporcional ao preço de compra pago.</span><span class="sxs-lookup"><span data-stu-id="759dc-189">Any software subscription product returned within the 30-day return period will receive a prorated credit of the paid purchase price.</span></span>

<span data-ttu-id="759dc-190">Esta mensagem é um acompanhamento das nossas comunicações por email enviadas em dezembro de 2020 e abril de 2021 a todos os parceiros CSP em relação ao período de devolução e outras atualizações do MPA.</span><span class="sxs-lookup"><span data-stu-id="759dc-190">This message is a follow-up to our email communications sent on December 2020 and April 2021 to all CSP partners regarding the return period and other updates to the MPA.</span></span> <span data-ttu-id="759dc-191">Confira estas notificações para obter detalhes completos sobre as alterações que afetam o MPA.</span><span class="sxs-lookup"><span data-stu-id="759dc-191">Refer to those notices for full details regarding changes affecting the MPA.</span></span>

#### <a name="software-download-link-expiry"></a><span data-ttu-id="759dc-192">Expiração do link de download de software</span><span class="sxs-lookup"><span data-stu-id="759dc-192">Software download link expiry</span></span>

<span data-ttu-id="759dc-193">A partir de 3 de junho de 2021, os links de download de software de compras de produtos de software perpétuos e de assinaturas de software por meio do Partner Center terão uma data de validade de cinco dias após o download inicial.</span><span class="sxs-lookup"><span data-stu-id="759dc-193">From June 3, 2021, the software download links for perpetual software and software subscription product purchases through Partner Center will have an expiration date of five days from the initial download.</span></span> <span data-ttu-id="759dc-194">O período de expiração será aplicado a todas as compras feitas em 3 de junho de 2021, bem como antes ou após essa data.</span><span class="sxs-lookup"><span data-stu-id="759dc-194">The expiry period will apply to all purchases before June 3, 2021, as well as on or after June 3, 2021.</span></span>

### <a name="next-steps"></a><span data-ttu-id="759dc-195">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="759dc-195">Next steps</span></span>

<span data-ttu-id="759dc-196">Examine as [Perguntas frequentes sobre o período de devolução e a expiração do link de download do CSP](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf) e informe todas as equipes apropriadas na sua organização sobre estas alterações:</span><span class="sxs-lookup"><span data-stu-id="759dc-196">Review the [CSP return period and download link expiry FAQ](https://partner.microsoft.com/resources/detail/csp-software-return-period-download-expiry-faq-pdf), and inform all appropriate teams within your organization of these changes:</span></span>

### <a name="questions"></a><span data-ttu-id="759dc-197">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="759dc-197">Questions?</span></span>

<span data-ttu-id="759dc-198">Caso tenha dúvidas sobre essas ofertas, confira as comunidades relevantes no Yammer.</span><span class="sxs-lookup"><span data-stu-id="759dc-198">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="open-licensing-program-transitioning-resellers-to-the-cloud-solution-provider-csp-program"></a><a name="7"></a><span data-ttu-id="759dc-199">Programa Licenciamento Open: transição de revendedores para o programa CSP (Provedor de Soluções na Nuvem)</span><span class="sxs-lookup"><span data-stu-id="759dc-199">Open Licensing program: Transitioning resellers to the Cloud Solution Provider (CSP) program</span></span>

### <a name="categories"></a><span data-ttu-id="759dc-200">Categorias</span><span class="sxs-lookup"><span data-stu-id="759dc-200">Categories</span></span>

- <span data-ttu-id="759dc-201">Data: 19/04/2021</span><span class="sxs-lookup"><span data-stu-id="759dc-201">Date: 2021-04-19</span></span>
- <span data-ttu-id="759dc-202">Amplie seus negócios</span><span class="sxs-lookup"><span data-stu-id="759dc-202">Grow Your Business</span></span>

### <a name="summary"></a><span data-ttu-id="759dc-203">Resumo</span><span class="sxs-lookup"><span data-stu-id="759dc-203">Summary</span></span>

<span data-ttu-id="759dc-204">Essa comunicação fornece detalhes sobre como se preparar para as alterações que serão disponibilizadas em breve para o programa Licenciamento Open.</span><span class="sxs-lookup"><span data-stu-id="759dc-204">This communication details how to prepare for the changes that are coming soon to the Open Licensing program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="759dc-205">Público-alvo afetado</span><span class="sxs-lookup"><span data-stu-id="759dc-205">Impacted audience</span></span>

<span data-ttu-id="759dc-206">Parceiros do Open License e CSP</span><span class="sxs-lookup"><span data-stu-id="759dc-206">CSP and Open License partners</span></span>

### <a name="details"></a><span data-ttu-id="759dc-207">Detalhes</span><span class="sxs-lookup"><span data-stu-id="759dc-207">Details</span></span>

<span data-ttu-id="759dc-208">Em 2020, a Microsoft [anunciou](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) que as licenças de software perpétuas estarão amplamente disponíveis para parceiros e clientes por meio do programa CSP (Provedor de Soluções na Nuvem).</span><span class="sxs-lookup"><span data-stu-id="759dc-208">In 2020, Microsoft [announced](https://blogs.partner.microsoft.com/mpn/general-availability-of-perpetual-software-licenses-in-the-cloud-solution-provider-program/) that perpetual software licenses will be broadly available to partners and customers through the Cloud Solution Provider (CSP) program.</span></span> <span data-ttu-id="759dc-209">O primeiro marco foi atingido em janeiro de 2021, quando as ofertas de software perpétuo comercial foram disponibilizadas.</span><span class="sxs-lookup"><span data-stu-id="759dc-209">The first milestone was reached in January 2021, when commercial perpetual software offers became available.</span></span> <span data-ttu-id="759dc-210">O próximo grande marco ocorrerá em julho de 2021, quando as ofertas do [setor público](https://aka.ms/openlicensepublicsector) forem disponibilizadas.</span><span class="sxs-lookup"><span data-stu-id="759dc-210">The next key milestone will happen in July 2021, when [public sector](https://aka.ms/openlicensepublicsector) offers become available.</span></span> <span data-ttu-id="759dc-211">Também [comunicamos](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) que, a partir de 1º de janeiro de 2022, nenhuma nova compra ou renovação de licença de software do Software Assurance ou de serviços online poderá ser feita por meio do programa Open License.</span><span class="sxs-lookup"><span data-stu-id="759dc-211">We also [communicated](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) that effective January 1, 2022, no new software license purchases or renewals of Software Assurance or online services can be made through the Open License program.</span></span>

<span data-ttu-id="759dc-212">A transição do software perpétuo para o programa CSP na nova experiência de comércio ajudará os parceiros a expandir as oportunidades para oferecer soluções e serviços gerenciados diversificados.</span><span class="sxs-lookup"><span data-stu-id="759dc-212">The transition of perpetual software to the CSP program in the new commerce experience will help partners to expand the opportunities to offer diverse solutions and managed services.</span></span> <span data-ttu-id="759dc-213">Isso também acelerará a transição dos clientes para a nuvem.</span><span class="sxs-lookup"><span data-stu-id="759dc-213">This will also accelerate customers’ transition to the cloud.</span></span>  <span data-ttu-id="759dc-214">Para ajudar a garantir uma transição estável para nossos parceiros e clientes, criamos estes ajustes e materiais para acelerar essa transformação digital:</span><span class="sxs-lookup"><span data-stu-id="759dc-214">To help ensure a smooth transition for both our partners and customers, we’ve made these adjustments and materials to accelerate this digital transformation:</span></span>

#### <a name="april-2021"></a><span data-ttu-id="759dc-215">Abril de 2021</span><span class="sxs-lookup"><span data-stu-id="759dc-215">April 2021</span></span>

<span data-ttu-id="759dc-216">[Agora disponíveis](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/): materiais de transição do Open License para o CSP para revendedores</span><span class="sxs-lookup"><span data-stu-id="759dc-216">[Now available](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/): Open License-to-CSP transition materials for resellers</span></span>

#### <a name="july-2021"></a><span data-ttu-id="759dc-217">Julho de 2021</span><span class="sxs-lookup"><span data-stu-id="759dc-217">July 2021</span></span>

##### <a name="csp"></a><span data-ttu-id="759dc-218">CSP</span><span class="sxs-lookup"><span data-stu-id="759dc-218">CSP</span></span>

- <span data-ttu-id="759dc-219">1º de julho: licenças de software perpétuas disponíveis para os clientes do setor público</span><span class="sxs-lookup"><span data-stu-id="759dc-219">July 1: Perpetual software licenses available to public sector customers</span></span>

- <span data-ttu-id="759dc-220">7 de julho: licenças de software perpétuas do Visual Studio Pro e do Get Genuine Windows Agreement disponíveis para todos os segmentos</span><span class="sxs-lookup"><span data-stu-id="759dc-220">July 7: Visual Studio Pro and Get Genuine Windows Agreement  perpetual software licenses available to all segments</span></span>

##### <a name="open-value"></a><span data-ttu-id="759dc-221">Open Value</span><span class="sxs-lookup"><span data-stu-id="759dc-221">Open Value</span></span>

- <span data-ttu-id="759dc-222">1º de julho: SKUs adicionais disponíveis no programa Open Value para educação e entidades sem fins lucrativos, fornecendo ofertas semelhantes ao programa Open License</span><span class="sxs-lookup"><span data-stu-id="759dc-222">July 1: Additional SKUs available in the Open Value program for education and nonprofit, providing similar offers to the Open License program</span></span>

##### <a name="open-license"></a><span data-ttu-id="759dc-223">Open License</span><span class="sxs-lookup"><span data-stu-id="759dc-223">Open License</span></span>

- <span data-ttu-id="759dc-224">1º de julho: a Microsoft não iniciará mais novas ofertas no programa Open License.</span><span class="sxs-lookup"><span data-stu-id="759dc-224">July 1: Microsoft will no longer launch new offers in the Open License program.</span></span>

#### <a name="january-2022"></a><span data-ttu-id="759dc-225">Janeiro de 2022</span><span class="sxs-lookup"><span data-stu-id="759dc-225">January 2022</span></span>

- <span data-ttu-id="759dc-226">1º de janeiro: nenhuma nova compra ou renovação poderá ser feita por meio do programa Open License</span><span class="sxs-lookup"><span data-stu-id="759dc-226">January 1: No new purchases or renewals can be made through the Open License program</span></span>

### <a name="next-steps"></a><span data-ttu-id="759dc-227">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="759dc-227">Next steps</span></span>

#### <a name="csp-indirect-providers"></a><span data-ttu-id="759dc-228">Provedores indiretos do CSP</span><span class="sxs-lookup"><span data-stu-id="759dc-228">CSP indirect providers</span></span>

<span data-ttu-id="759dc-229">Use os próximos meses para ajudar os revendedores do Open License a se orientarem no programa CSP, participando de eventos da comunidade de parceiros e usando os materiais de transição do Open License para o CSP para revendedores:</span><span class="sxs-lookup"><span data-stu-id="759dc-229">Use the coming months to help Open License resellers orient into the CSP program by attending partner community events and using the Open License-to-CSP transition materials for resellers:</span></span>

- <span data-ttu-id="759dc-230">[Materiais de transição do Open License para o CSP para revendedores](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/): apresentação de visão geral personalizável, modelo de email, guia de integração de revendedor indireto do CSP, entre outros, para ajudar você a incentivar a adoção dos revendedores em escala.</span><span class="sxs-lookup"><span data-stu-id="759dc-230">[Open License-to-CSP transition materials for resellers](https://partner.microsoft.com/resources/collection/reseller-open-license-to-csp-transition-materials#/)—Customizable overview presentation, email template, CSP indirect reseller onboarding guide, and more to help you drive the adoption for your resellers at scale.</span></span>

- <span data-ttu-id="759dc-231">[Eventos da comunidade de parceiros do CSP](https://globalpbocomm.eventbuilder.com/GlobalCSP) hospedados pelas Operações Comerciais da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="759dc-231">[CSP Partner Community Events](https://globalpbocomm.eventbuilder.com/GlobalCSP) hosted by Microsoft Business Operations.</span></span>  <span data-ttu-id="759dc-232">Participe das várias sessões para aprender os conceitos básicos do CSP ou manter-se atualizado e faça perguntas sobre o software no CSP (sessões de perguntas e respostas).</span><span class="sxs-lookup"><span data-stu-id="759dc-232">Join the various sessions to learn CSP basics (CSP Fundamentals) or stay up to date, and ask questions regarding Software in CSP (Q&A Sessions).</span></span>

- <span data-ttu-id="759dc-233">(Em breve) Sessão de treinamento voltada ao revendedor indireto do CSP hospedada pelas Operações Comerciais da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="759dc-233">(Coming soon) CSP indirect reseller–focused training session hosted by Microsoft Business Operations.</span></span>

#### <a name="open-license-resellers"></a><span data-ttu-id="759dc-234">Revendedores do Open License</span><span class="sxs-lookup"><span data-stu-id="759dc-234">Open License resellers</span></span>

- <span data-ttu-id="759dc-235">Se a sua organização não estiver registrada no programa CSP, entre em contato com seu distribuidor para obter informações sobre como começar.</span><span class="sxs-lookup"><span data-stu-id="759dc-235">If your organization isn’t currently enrolled in the CSP program, contact your distributor for information on how to get started.</span></span> <span data-ttu-id="759dc-236">Conecte-se com um provedor indireto [aqui](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider).</span><span class="sxs-lookup"><span data-stu-id="759dc-236">Connect with an indirect provider [here](https://partner.microsoft.com/membership/cloud-solution-provider/find-a-provider).</span></span>

- <span data-ttu-id="759dc-237">Se a sua organização já estiver registrada no programa CSP, saiba mais sobre o software perpétuo no CSP [aqui](https://partner.microsoft.com/resources/collection/software-in-csp).</span><span class="sxs-lookup"><span data-stu-id="759dc-237">If your organization is already enrolled in the CSP program, learn more about perpetual software in CSP [here](https://partner.microsoft.com/resources/collection/software-in-csp).</span></span>

### <a name="questions"></a><span data-ttu-id="759dc-238">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="759dc-238">Questions?</span></span>

<span data-ttu-id="759dc-239">Em caso de dúvidas adicionais sobre essas ofertas, confira as comunidades relevantes no Yammer.</span><span class="sxs-lookup"><span data-stu-id="759dc-239">For further questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="now-live-global-promo-readiness-guide"></a><a name="6"></a><span data-ttu-id="759dc-240">Já disponível: guia de preparação para promoções globais</span><span class="sxs-lookup"><span data-stu-id="759dc-240">Now live: Global promo readiness guide</span></span>

### <a name="categories"></a><span data-ttu-id="759dc-241">Categorias</span><span class="sxs-lookup"><span data-stu-id="759dc-241">Categories</span></span>

- <span data-ttu-id="759dc-242">Data: 16/04/2021</span><span class="sxs-lookup"><span data-stu-id="759dc-242">Date: 2021-04-16</span></span>
- <span data-ttu-id="759dc-243">Funcionalidades</span><span class="sxs-lookup"><span data-stu-id="759dc-243">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="759dc-244">Resumo</span><span class="sxs-lookup"><span data-stu-id="759dc-244">Summary</span></span>

<span data-ttu-id="759dc-245">A Preparação para Lançamento publicou um novo [guia de preparação para promoções globais](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) na galeria de recursos da Preparação para Operações.</span><span class="sxs-lookup"><span data-stu-id="759dc-245">Launch Readiness has published a new [global promo readiness guide](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) on the Operations Readiness resource gallery.</span></span> <span data-ttu-id="759dc-246">Esse guia fornece uma exibição consolidada de todas as [promoções globais](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/) ativas.</span><span class="sxs-lookup"><span data-stu-id="759dc-246">This guide provides a consolidated view of all active [global promotions](https://partner.microsoft.com/resources/collection/global-promo-readiness-guide-collection#/).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="759dc-247">Público-alvo afetado</span><span class="sxs-lookup"><span data-stu-id="759dc-247">Impacted audience</span></span>

<span data-ttu-id="759dc-248">Todos os parceiros do VL (licenciamento por volume), da DPL (lista de preços do Dynamics) e do CSP (Provedor de Soluções na Nuvem)</span><span class="sxs-lookup"><span data-stu-id="759dc-248">All Volume Licensing (VL), Dynamics Price List (DPL), and Cloud Solution Provider (CSP) partners</span></span>

### <a name="details"></a><span data-ttu-id="759dc-249">Detalhes</span><span class="sxs-lookup"><span data-stu-id="759dc-249">Details</span></span>

<span data-ttu-id="759dc-250">Os parceiros da Microsoft compartilharam conosco a necessidade de fornecer uma exibição consolidada de todas as promoções globais com detalhes de suporte.</span><span class="sxs-lookup"><span data-stu-id="759dc-250">Microsoft partners have shared with us the need to provide a consolidated view of all global promotions with supporting details.</span></span> <span data-ttu-id="759dc-251">Você deseja que esse guia consolidado ajude a usar as promoções, com a confiança de que todas as informações disponíveis estarão prontamente acessíveis em uma localização central e conveniente.</span><span class="sxs-lookup"><span data-stu-id="759dc-251">You wanted this consolidated guide to help you use promotions with the confidence that all the available information will be readily accessible in a central and convenient location.</span></span>

<span data-ttu-id="759dc-252">A partir de abril de 2021, a Microsoft atualizará esse guia mensalmente, e ele ficará disponível em uma coleção dedicada de guias de preparação para promoções globais na galeria de recursos da Preparação para Operações.</span><span class="sxs-lookup"><span data-stu-id="759dc-252">Beginning in April 2021, Microsoft will update this guide on a monthly basis, and it will be available in a dedicated Global Promo Readiness Guide collection in the Operations Readiness resource gallery.</span></span>

<span data-ttu-id="759dc-253">Os links para o guia também serão incluídos nas seguintes coleções:</span><span class="sxs-lookup"><span data-stu-id="759dc-253">Links to this guide will also be included in the following collections:</span></span>

- <span data-ttu-id="759dc-254">[Coleção de calendário de lançamento](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/), que fornece uma exibição centralizada das próximas alterações e dos próximos lançamentos.</span><span class="sxs-lookup"><span data-stu-id="759dc-254">[Launch calendar collection](https://partner.microsoft.com/resources/collection/csp-announcement-calendar#/), which provides a centralized view of upcoming changes and launches.</span></span>

- <span data-ttu-id="759dc-255">[Coleções da comunidade](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), que contêm materiais de suporte para nossas chamadas de parceiros mensais, destacando alterações futuras e tópicos oportunos de interesse operacional.</span><span class="sxs-lookup"><span data-stu-id="759dc-255">[Community collections](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), which contain supporting materials for our monthly partner calls, highlighting upcoming changes and timely topics of operational interest.</span></span>

- <span data-ttu-id="759dc-256">[Boletins informativos de parceiros](https://partner.microsoft.com/resources/collection/csp-monthly-update#/), como a Atualização Mensal do CSP</span><span class="sxs-lookup"><span data-stu-id="759dc-256">[Partner newsletters](https://partner.microsoft.com/resources/collection/csp-monthly-update#/), such as CSP Monthly Update</span></span>

<span data-ttu-id="759dc-257">Como lembrete mensal, também publicaremos um comunicado no Partner Center a cada nova edição do guia de preparação para promoções globais.</span><span class="sxs-lookup"><span data-stu-id="759dc-257">As a monthly reminder, we will also publish a Partner Center announcement with each new issue of the global promo readiness guide.</span></span>

### <a name="next-steps"></a><span data-ttu-id="759dc-258">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="759dc-258">Next steps</span></span>

<span data-ttu-id="759dc-259">No início de cada mês, você encontrará o último [guia de preparação para promoções globais](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) na [galeria de recursos da Preparação para Operações](https://partner.microsoft.com/resources).</span><span class="sxs-lookup"><span data-stu-id="759dc-259">At the start of each month, you will find the latest [global promo readiness guide](https://partner.microsoft.com/resources/detail/operations-promo-guide-pdf) in the [Operations Readiness resource gallery](https://partner.microsoft.com/resources).</span></span>

<span data-ttu-id="759dc-260">Compartilhe essas informações com os contatos apropriados nas suas organizações e conte-nos como o guia ajudou você por meio do botão “Esta página foi útil?”</span><span class="sxs-lookup"><span data-stu-id="759dc-260">Share this information with the appropriate contacts in your organizations and let us know how helpful the guide is through the “Was this page helpful?”</span></span> <span data-ttu-id="759dc-261">no final de cada página.</span><span class="sxs-lookup"><span data-stu-id="759dc-261">button at the end of each page.</span></span>

________________
## <a name="april-cloud-solution-provider-csp-community-update-and-reminders"></a><a name="5"></a><span data-ttu-id="759dc-262">Atualização de abril e lembretes da comunidade do CSP (Provedor de Soluções na Nuvem)</span><span class="sxs-lookup"><span data-stu-id="759dc-262">April Cloud Solution Provider (CSP) community update and reminders</span></span>

### <a name="categories"></a><span data-ttu-id="759dc-263">Categorias</span><span class="sxs-lookup"><span data-stu-id="759dc-263">Categories</span></span>

- <span data-ttu-id="759dc-264">Data: 16/04/2021</span><span class="sxs-lookup"><span data-stu-id="759dc-264">Date: 2021-04-16</span></span>
- <span data-ttu-id="759dc-265">Comunidade | Convites e lembretes</span><span class="sxs-lookup"><span data-stu-id="759dc-265">Community | Invites and reminders</span></span>

### <a name="summary"></a><span data-ttu-id="759dc-266">Resumo</span><span class="sxs-lookup"><span data-stu-id="759dc-266">Summary</span></span>

<span data-ttu-id="759dc-267">Os recursos da comunidade do CSP estão disponíveis sob demanda e são atualizados mensalmente para mantê-lo informado e preparado para as alterações no programa CSP.</span><span class="sxs-lookup"><span data-stu-id="759dc-267">CSP community resources are available on demand and updated monthly to keep you informed and prepared for change in the CSP program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="759dc-268">Público-alvo afetado</span><span class="sxs-lookup"><span data-stu-id="759dc-268">Impacted audience</span></span>

<span data-ttu-id="759dc-269">Provedores indiretos ou parceiros de cobrança direta do CSP</span><span class="sxs-lookup"><span data-stu-id="759dc-269">CSP direct bill partners and indirect providers</span></span>

### <a name="details"></a><span data-ttu-id="759dc-270">Detalhes</span><span class="sxs-lookup"><span data-stu-id="759dc-270">Details</span></span>

<span data-ttu-id="759dc-271">Neste mês, os recursos incluem os seguintes tópicos principais:</span><span class="sxs-lookup"><span data-stu-id="759dc-271">This month, the resources include the following key topics:</span></span>

- [<span data-ttu-id="759dc-272">Atualização da evolução do programa CSP e alterações no programa Open License</span><span class="sxs-lookup"><span data-stu-id="759dc-272">Update to CSP program evolution and Open License program changes</span></span>](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/)

- [<span data-ttu-id="759dc-273">Alterações nos requisitos de integração do cliente CSP em algumas regiões</span><span class="sxs-lookup"><span data-stu-id="759dc-273">Changes to CSP customer onboarding requirements in certain regions</span></span>](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/)

- [<span data-ttu-id="759dc-274">Novo formato para a nova fatura de PDF de comércio no programa CSP</span><span class="sxs-lookup"><span data-stu-id="759dc-274">New format for the new commerce PDF invoice in the CSP program</span></span>](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/)

<span data-ttu-id="759dc-275">Na [coleção de comunidades do CSP](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), você encontrará:</span><span class="sxs-lookup"><span data-stu-id="759dc-275">Within the [CSP community collection](https://partner.microsoft.com/resources/collection/april-2021-csp-partner-community-content#/), you’ll find:</span></span>

- <span data-ttu-id="759dc-276">O [boletim informativo da Atualização Mensal do CSP](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global) para download, que agrega os comunicados, as atualizações, os eventos e os lembretes recentes do CSP em um documento de fácil leitura.</span><span class="sxs-lookup"><span data-stu-id="759dc-276">The downloadable [CSP Monthly Update newsletter](https://partner.microsoft.com/resources/detail/csp-monthly-update-april-2021-global), which aggregates recent CSP announcements, updates, events, and reminders in an easy-to-read document.</span></span>

- <span data-ttu-id="759dc-277">O [calendário de comunicados do CSP](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021), que fornece uma exibição de linha do tempo das alterações futuras que afetarão o programa.</span><span class="sxs-lookup"><span data-stu-id="759dc-277">The [CSP Announcement Calendar](https://partner.microsoft.com/resources/detail/csp-announcement-calendar-april-2021), which provides a timeline view of upcoming changes affecting the program.</span></span>

- <span data-ttu-id="759dc-278">O novo [calendário de lançamento de produtos](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf), no qual você poderá ver os lançamentos e as ofertas de produtos futuros.</span><span class="sxs-lookup"><span data-stu-id="759dc-278">The new [product launch calendar](https://partner.microsoft.com/resources/detail/product-launch-calendar-april-pdf), where you can view upcoming product launches and offers.</span></span>

- <span data-ttu-id="759dc-279">[Recursos de atualização de lançamentos do CSP](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/), com um conteúdo de fácil consumo sobre as principais alterações operacionais.</span><span class="sxs-lookup"><span data-stu-id="759dc-279">[CSP launch update resources](https://partner.microsoft.com/resources/collection/april-2021-csp-launch-topics-collection#/) with easy-to-consume content on key operational changes.</span></span>

- <span data-ttu-id="759dc-280">[Lembretes](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf) sobre os principais tópicos do CSP que geraram interesse e dúvidas.</span><span class="sxs-lookup"><span data-stu-id="759dc-280">[Refreshers and reminders](https://partner.microsoft.com/resources/detail/csp-april-2021-refreshers-and-reminders-pdf) on key CSP topics receiving interest and queries.</span></span>

#### <a name="csp-community-call-qas"></a><span data-ttu-id="759dc-281">Sessões de perguntas e respostas da Chamada da Comunidade do CSP</span><span class="sxs-lookup"><span data-stu-id="759dc-281">CSP Community Call Q&As</span></span>

<span data-ttu-id="759dc-282">As sessões de perguntas e respostas da Chamada da Comunidade estão disponíveis para ajudar você com dúvidas relacionadas às alterações futuras.</span><span class="sxs-lookup"><span data-stu-id="759dc-282">Community Call Q&As are available to help you with questions related to upcoming changes.</span></span> <span data-ttu-id="759dc-283">Registre-se agora mesmo nas sessões de perguntas e respostas da Chamada da Comunidade do CSP, que serão realizadas em abril, maio e junho.</span><span class="sxs-lookup"><span data-stu-id="759dc-283">Register now for CSP Community Call Q&As that are taking place in April, May, and June.</span></span> <span data-ttu-id="759dc-284">Elas terão como foco os mais recentes lançamentos e lembretes importantes.</span><span class="sxs-lookup"><span data-stu-id="759dc-284">These will focus on the latest launches, important refreshers, and reminders.</span></span>

<span data-ttu-id="759dc-285">[Registre-se aqui](https://globalpbocomm.eventbuilder.com/GlobalCSP).</span><span class="sxs-lookup"><span data-stu-id="759dc-285">[Register here](https://globalpbocomm.eventbuilder.com/GlobalCSP).</span></span>

### <a name="next-steps"></a><span data-ttu-id="759dc-286">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="759dc-286">Next steps</span></span>

<span data-ttu-id="759dc-287">Examine os recursos da comunidade e registre-se na sessão de perguntas e respostas da Chamada da Comunidade.</span><span class="sxs-lookup"><span data-stu-id="759dc-287">Review the community resources and register for the Community Call Q&A.</span></span>

<span data-ttu-id="759dc-288">Para garantir que você obtenha o máximo da sessão de perguntas e respostas da Chamada da Comunidade, examine o conteúdo da comunidade sob demanda e envie suas perguntas em até 48 horas antes da chamada.</span><span class="sxs-lookup"><span data-stu-id="759dc-288">To ensure that you get the most from the Community Call Q&A, review the on-demand community content and submit your questions up to 48 hours before the call.</span></span>

### <a name="questions"></a><span data-ttu-id="759dc-289">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="759dc-289">Questions?</span></span>

<span data-ttu-id="759dc-290">A sessão mensal de perguntas e respostas da Chamada da Comunidade do CSP é o melhor lugar para solucionar dúvidas relacionadas às alterações no programa CSP.</span><span class="sxs-lookup"><span data-stu-id="759dc-290">The monthly CSP Community Call Q&A is the best place for questions related to changes in the CSP program.</span></span> <span data-ttu-id="759dc-291">Todos os meses, examine o material e envie suas perguntas com antecedência para que possamos utilizar a sessão para os tópicos mais importantes para você.</span><span class="sxs-lookup"><span data-stu-id="759dc-291">Each month, review the material and submit your questions in advance so that we can spend the session on the topics that are most important to you.</span></span>

<span data-ttu-id="759dc-292">Para obter mais informações, entre em contato com o [Suporte](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp).</span><span class="sxs-lookup"><span data-stu-id="759dc-292">For more information, contact [Support](https://partner.microsoft.com/dashboard/support/csp/servicerequests/create?category=csp).</span></span>

________________
## <a name="reminder-deprecation-of-get-qualification-on-may-4-2021"></a><a name="4"></a><span data-ttu-id="759dc-293">Lembrete: preterimento da qualificação GET em 4 de maio de 2021</span><span class="sxs-lookup"><span data-stu-id="759dc-293">Reminder: Deprecation of GET qualification on May 4, 2021</span></span>

### <a name="categories"></a><span data-ttu-id="759dc-294">Categorias</span><span class="sxs-lookup"><span data-stu-id="759dc-294">Categories</span></span>

- <span data-ttu-id="759dc-295">Data: 09/04/2021</span><span class="sxs-lookup"><span data-stu-id="759dc-295">Date: 2021-04-09</span></span>
- <span data-ttu-id="759dc-296">Capacidades</span><span class="sxs-lookup"><span data-stu-id="759dc-296">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="759dc-297">Público-alvo afetado</span><span class="sxs-lookup"><span data-stu-id="759dc-297">Impacted audience</span></span>

<span data-ttu-id="759dc-298">Parceiros que vendem ofertas Acadêmicas, Sem Fins Lucrativos e GCC (Nuvem da Comunidade Governamental) por meio do programa Provedor de Soluções na Nuvem usando a API do Partner Center</span><span class="sxs-lookup"><span data-stu-id="759dc-298">Partners selling Academic, Nonprofit, and Government Community Cloud (GCC) offers through the Cloud Solution Provider program using the Partner Center API</span></span>

### <a name="details"></a><span data-ttu-id="759dc-299">Detalhes</span><span class="sxs-lookup"><span data-stu-id="759dc-299">Details</span></span>

<span data-ttu-id="759dc-300">Este comunicado é um acompanhamento dos [aprimoramentos lançados em dezembro](https://docs.microsoft.com/partner-center/announcements/2020-december#1) do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="759dc-300">This announcement is a follow-up to the Partner Center [enhancements released in December](https://docs.microsoft.com/partner-center/announcements/2020-december#1).</span></span> <span data-ttu-id="759dc-301">Como parte dessa versão, as novas APIs de Qualificações GET e POST foram implantadas e, como resultado, a qualificação GET será desativada até 4 de maio de 2021.</span><span class="sxs-lookup"><span data-stu-id="759dc-301">As part of that release, new GET and POST Qualifications APIs were deployed and, as a result, the existing GET qualification will be retired by May 4, 2021.</span></span> <span data-ttu-id="759dc-302">Até lá, você precisará ter feito a transição para usar as novas APIs POST do Partner Center na compra de ofertas de Educação e a nova API de qualificações GET para comprar ofertas Sem Fins Lucrativos e GCC pré-qualificadas.</span><span class="sxs-lookup"><span data-stu-id="759dc-302">By that time, you’ll need to have transitioned to using the new POST Partner Center APIs in purchase Education offers, and the new GET qualifications API to purchase prequalified Nonprofit and GCC offers.</span></span>

### <a name="next-steps"></a><span data-ttu-id="759dc-303">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="759dc-303">Next steps</span></span>

- <span data-ttu-id="759dc-304">Atualize para as novas APIs a fim de realizar uma transição bem-sucedida e em tempo hábil.</span><span class="sxs-lookup"><span data-stu-id="759dc-304">Update to the new APIs for a successful and timely transition.</span></span>

- <span data-ttu-id="759dc-305">Examine as novas alterações da API do Partner Center e o Guia nos recursos de Preparação de Operações: [aprimoramentos do processo de validação do cliente de Educação do Partner Center](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/).</span><span class="sxs-lookup"><span data-stu-id="759dc-305">Review the new Partner Center API changes and Guide in the Operations Readiness resources: [Partner Center Education customer validation process enhancements](https://partner.microsoft.com/resources/collection/partner-center-edu-validation-enhancements#/).</span></span>

- <span data-ttu-id="759dc-306">Compartilhe essas informações com as equipes apropriadas da sua organização e com seus revendedores para ajudá-los a se preparar para essas mudanças.</span><span class="sxs-lookup"><span data-stu-id="759dc-306">Share this information with the appropriate teams within your organization and with your resellers to help them prepare for these changes.</span></span>

### <a name="questions"></a><span data-ttu-id="759dc-307">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="759dc-307">Questions?</span></span>

<span data-ttu-id="759dc-308">Em caso de perguntas relacionadas a essa notificação, entre em contato com o [suporte do Partner Center](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals).</span><span class="sxs-lookup"><span data-stu-id="759dc-308">For any questions related to this notification, contact [Partner Center support](https://partner.microsoft.com/dashboard/support/referrals/servicerequests?category=referrals).</span></span>

### <a name="change-log"></a><span data-ttu-id="759dc-309">Log de alterações</span><span class="sxs-lookup"><span data-stu-id="759dc-309">Change log</span></span>

- <span data-ttu-id="759dc-310">Abril: lembrete do preterimento futuro da qualificação GET</span><span class="sxs-lookup"><span data-stu-id="759dc-310">April: Reminder of upcoming deprecation of GET qualification</span></span> 
- <span data-ttu-id="759dc-311">Fevereiro: atualização das linhas do tempo de reprovação das qualificações GET e PUT</span><span class="sxs-lookup"><span data-stu-id="759dc-311">February: Updated timelines for deprecation of GET & PUT qualifications</span></span>
- <span data-ttu-id="759dc-312">Janeiro: lembrete das reprovações futuras das qualificações GET e PUT</span><span class="sxs-lookup"><span data-stu-id="759dc-312">January: Reminder of upcoming deprecations of GET & PUT qualifications</span></span>

________________
## <a name="new-format-for-the-new-commerce-pdf-invoice-in-csp"></a><a name="3"></a><span data-ttu-id="759dc-313">Novo formato para a nova fatura de PDF de comércio no CSP</span><span class="sxs-lookup"><span data-stu-id="759dc-313">New format for the new commerce PDF invoice in CSP</span></span>

### <a name="categories"></a><span data-ttu-id="759dc-314">Categorias</span><span class="sxs-lookup"><span data-stu-id="759dc-314">Categories</span></span>

- <span data-ttu-id="759dc-315">Data: 05/04/2021</span><span class="sxs-lookup"><span data-stu-id="759dc-315">Date: 2021-04-05</span></span>
- <span data-ttu-id="759dc-316">Funcionalidades</span><span class="sxs-lookup"><span data-stu-id="759dc-316">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="759dc-317">Resumo</span><span class="sxs-lookup"><span data-stu-id="759dc-317">Summary</span></span>

<span data-ttu-id="759dc-318">A Microsoft está lançando um novo formato para a nova fatura de PDF de comércio no programa CSP (Provedor de Soluções na Nuvem) para exibir os detalhes de cobrança por detalhes do produto, em vez da descrição da SKU.</span><span class="sxs-lookup"><span data-stu-id="759dc-318">Microsoft is introducing a new format for the new commerce PDF invoice in the Cloud Solution Provider (CSP) program to display billing details by product detail instead of SKU description.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="759dc-319">Público-alvo afetado</span><span class="sxs-lookup"><span data-stu-id="759dc-319">Impacted audience</span></span>

<span data-ttu-id="759dc-320">Parceiros que fazem transações por meio do programa CSP</span><span class="sxs-lookup"><span data-stu-id="759dc-320">Partners transacting through the CSP program</span></span>

### <a name="details"></a><span data-ttu-id="759dc-321">Detalhes</span><span class="sxs-lookup"><span data-stu-id="759dc-321">Details</span></span>

<span data-ttu-id="759dc-322">A partir de maio de 2021, a Microsoft lançará um novo formato para a nova fatura de PDF de comércio no programa CSP para exibir os detalhes de cobrança por detalhes do produto, em vez da descrição da SKU.</span><span class="sxs-lookup"><span data-stu-id="759dc-322">Starting May 2021, Microsoft is introducing a new format for the new commerce PDF invoice in the CSP program to display billing details by product detail instead of SKU description.</span></span> <span data-ttu-id="759dc-323">Com a atualização, agregaremos os itens de linha por tipo de produto e exibiremos cada produto em uma linha individual.</span><span class="sxs-lookup"><span data-stu-id="759dc-323">With this new update, we will be aggregating the line items by product type while displaying every product on an individual line.</span></span>

<span data-ttu-id="759dc-324">A alteração entrará em vigor na fatura dos parceiros de maio, referente ao período de cobrança entre 1º de abril de 2021 e 30 de abril de 2021.</span><span class="sxs-lookup"><span data-stu-id="759dc-324">Partners will notice this change coming into effect in their May invoice for the billing period between April 1, 2021 and April 30, 2021.</span></span> <span data-ttu-id="759dc-325">As ofertas afetadas são a Instância Reservada do Microsoft Azure, as assinaturas do Azure (plano do Azure) e o Marketplace.</span><span class="sxs-lookup"><span data-stu-id="759dc-325">The affected offers are Microsoft Azure Reserved Instance, Azure subscriptions (Azure plan), and Marketplace.</span></span>

<span data-ttu-id="759dc-326">As solicitações de nova cobrança de crédito realizadas após a atualização do formato da fatura serão geradas no novo formato.</span><span class="sxs-lookup"><span data-stu-id="759dc-326">Any credit-rebill requests made after the invoice format has been updated will be generated in the new format.</span></span>

#### <a name="partner-benefits"></a><span data-ttu-id="759dc-327">Benefícios do parceiro</span><span class="sxs-lookup"><span data-stu-id="759dc-327">Partner benefits</span></span>

<span data-ttu-id="759dc-328">A atualização oferecerá os seguintes aprimoramentos para o faturamento dos parceiros:</span><span class="sxs-lookup"><span data-stu-id="759dc-328">This update will offer the following improvements to the invoicing experience for partners:</span></span>

- <span data-ttu-id="759dc-329">Redução do tamanho da fatura sem omitir dados essenciais</span><span class="sxs-lookup"><span data-stu-id="759dc-329">Reduced invoice size while retaining critical data</span></span>

- <span data-ttu-id="759dc-330">Alinhamento do formato com os padrões do setor para faturas compactas e fáceis de entender</span><span class="sxs-lookup"><span data-stu-id="759dc-330">Alignment of the format to the industry standards for compact and user-friendly invoices</span></span> 

<span data-ttu-id="759dc-331">Os seguintes elementos não serão afetados:</span><span class="sxs-lookup"><span data-stu-id="759dc-331">The following elements will not be affected:</span></span>

- <span data-ttu-id="759dc-332">Página de resumo de cobrança no PDF da fatura</span><span class="sxs-lookup"><span data-stu-id="759dc-332">Billing summary page on the invoice PDF</span></span>

- <span data-ttu-id="759dc-333">APIs de faturamento atuais</span><span class="sxs-lookup"><span data-stu-id="759dc-333">Existing invoicing APIs</span></span>

- <span data-ttu-id="759dc-334">Arquivos de reconciliação (usados para recuperar dados granulares)</span><span class="sxs-lookup"><span data-stu-id="759dc-334">Reconciliation files (Recon files can be used for retrieving granular data.)</span></span> 

- <span data-ttu-id="759dc-335">Faturas de encargos com base em uso e licença</span><span class="sxs-lookup"><span data-stu-id="759dc-335">Usage and license-based charges invoices</span></span>

### <a name="next-steps"></a><span data-ttu-id="759dc-336">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="759dc-336">Next steps</span></span>

<span data-ttu-id="759dc-337">Examine as informações sobre o tópico na [galeria de recursos de preparação de Operações](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/) no site de parceiros da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="759dc-337">Review the information about this topic in the [Operations Readiness resource gallery](https://partner.microsoft.com/resources/collection/introducing-new-format-for-the-new-commerce-invoice-in-csp#/) on the Microsoft partner website.</span></span> <span data-ttu-id="759dc-338">Para mais informações sobre tópicos relacionados a cobrança e imposto, incluindo recursos de cobrança, faturas, cobrança do CSP e impostos, visite a [seção Cobrança](https://docs.microsoft.com/partner-center/billing) do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="759dc-338">For more information about billing and tax topics including billing resources, invoices, CSP billing, and taxes, visit the [Billing section](https://docs.microsoft.com/partner-center/billing) in Partner Center.</span></span>

________________
## <a name="changes-to-the-cloud-solution-provider-csp-customer-onboarding-requirements"></a><a name="2"></a><span data-ttu-id="759dc-339">Alterações nos requisitos de integração do cliente do CSP (Provedor de Soluções na Nuvem)</span><span class="sxs-lookup"><span data-stu-id="759dc-339">Changes to the Cloud Solution Provider (CSP) customer onboarding requirements</span></span>

### <a name="categories"></a><span data-ttu-id="759dc-340">Categorias</span><span class="sxs-lookup"><span data-stu-id="759dc-340">Categories</span></span>

- <span data-ttu-id="759dc-341">Data: 02/04/2021</span><span class="sxs-lookup"><span data-stu-id="759dc-341">Date: 2021-04-02</span></span>
- <span data-ttu-id="759dc-342">Ofertas/mercados</span><span class="sxs-lookup"><span data-stu-id="759dc-342">Offers/Markets</span></span>

### <a name="summary"></a><span data-ttu-id="759dc-343">Resumo</span><span class="sxs-lookup"><span data-stu-id="759dc-343">Summary</span></span>

<span data-ttu-id="759dc-344">Como parte do nosso compromisso de ajudar parceiros e clientes a administrar os negócios com base na confiança, solicitaremos informações adicionais do cliente a partir do dia 25 de março de 2021.</span><span class="sxs-lookup"><span data-stu-id="759dc-344">As part of our commitment to help partners and customers run their business based on trust, we will request additional customer information, effective March 25, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="759dc-345">Público-alvo afetado</span><span class="sxs-lookup"><span data-stu-id="759dc-345">Impacted audience</span></span>

<span data-ttu-id="759dc-346">Provedores indiretos e parceiros de cobrança direta do CSP que têm clientes novos ou existentes nos países/regiões listados na próxima seção</span><span class="sxs-lookup"><span data-stu-id="759dc-346">CSP direct bill partners and indirect providers who have new or existing customers in the countries listed in the next section</span></span>

### <a name="details"></a><span data-ttu-id="759dc-347">Detalhes</span><span class="sxs-lookup"><span data-stu-id="759dc-347">Details</span></span>

<span data-ttu-id="759dc-348">O trabalho da Microsoft é baseado em confiança.</span><span class="sxs-lookup"><span data-stu-id="759dc-348">Microsoft runs on trust.</span></span> <span data-ttu-id="759dc-349">Temos o compromisso de fornecer um método de validação do cliente que esteja em conformidade e que seja seguro e protegido para realizar transações de assinatura de clientes no programa CSP.</span><span class="sxs-lookup"><span data-stu-id="759dc-349">We’re committed to providing a compliant, safe, and secure method of customer validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="759dc-350">Em 25 de março de 2021, apresentaremos os aprimoramentos da IU (interface do usuário) e da API do Partner Center que afetarão os parceiros que atendem a estes dois critérios:</span><span class="sxs-lookup"><span data-stu-id="759dc-350">On March 25, 2021, we will be introducing Partner Center API and user interface (UI) enhancements that will affect partners who meet both of the following criteria:</span></span>

- <span data-ttu-id="759dc-351">O parceiro tem um relacionamento de cobrança direta com a Microsoft (o que significa que ele é um parceiro de cobrança direta ou um provedor indireto).</span><span class="sxs-lookup"><span data-stu-id="759dc-351">The partner has a direct billing relationship with Microsoft (which means that the partner is either a direct bill partner or an indirect provider).</span></span>

- <span data-ttu-id="759dc-352">O parceiro faz negócios com clientes novos ou existentes nos seguintes países/regiões:</span><span class="sxs-lookup"><span data-stu-id="759dc-352">The partner does business with new or existing customers in the following countries:</span></span>

    - <span data-ttu-id="759dc-353">Tailândia</span><span class="sxs-lookup"><span data-stu-id="759dc-353">Thailand</span></span>
    - <span data-ttu-id="759dc-354">Vietnã</span><span class="sxs-lookup"><span data-stu-id="759dc-354">Vietnam</span></span>
    - <span data-ttu-id="759dc-355">Turquia</span><span class="sxs-lookup"><span data-stu-id="759dc-355">Turkey</span></span>
    - <span data-ttu-id="759dc-356">Polônia</span><span class="sxs-lookup"><span data-stu-id="759dc-356">Poland</span></span>
    - <span data-ttu-id="759dc-357">África do Sul</span><span class="sxs-lookup"><span data-stu-id="759dc-357">South Africa</span></span>
    - <span data-ttu-id="759dc-358">Índia</span><span class="sxs-lookup"><span data-stu-id="759dc-358">India</span></span>
    - <span data-ttu-id="759dc-359">Brasil</span><span class="sxs-lookup"><span data-stu-id="759dc-359">Brazil</span></span>
    - <span data-ttu-id="759dc-360">Iraque</span><span class="sxs-lookup"><span data-stu-id="759dc-360">Iraq</span></span>
    - <span data-ttu-id="759dc-361">Myanmar</span><span class="sxs-lookup"><span data-stu-id="759dc-361">Myanmar</span></span>
    - <span data-ttu-id="759dc-362">Sudão do Sul</span><span class="sxs-lookup"><span data-stu-id="759dc-362">South Sudan</span></span>
    - <span data-ttu-id="759dc-363">Arábia Saudita</span><span class="sxs-lookup"><span data-stu-id="759dc-363">Saudi Arabia</span></span>
    - <span data-ttu-id="759dc-364">Emirados Árabes Unidos</span><span class="sxs-lookup"><span data-stu-id="759dc-364">United Arab Emirates</span></span>
    - <span data-ttu-id="759dc-365">Venezuela</span><span class="sxs-lookup"><span data-stu-id="759dc-365">Venezuela</span></span>

<span data-ttu-id="759dc-366">Os parceiros que atendem aos critérios precisarão enviar a ID de registro da empresa do cliente (também conhecido como o INN da organização do cliente) e o número de telefone na próxima atualização ou na criação de uma assinatura para esse cliente.</span><span class="sxs-lookup"><span data-stu-id="759dc-366">Partners who meet the criteria will have to submit a customer's company registration ID (also known as the customer's organization INN) and phone number when they next update or create a subscription for that customer.</span></span> <span data-ttu-id="759dc-367">Esses parceiros também podem inserir um segundo nome opcional para o cliente.</span><span class="sxs-lookup"><span data-stu-id="759dc-367">These partners can also enter an optional middle name for the customer.</span></span>

<span data-ttu-id="759dc-368">Observe que, ao adicionar a ID de registro da sua empresa, você deve usar o número de identificação de contribuinte da sua empresa e não a ID pessoal do cliente.</span><span class="sxs-lookup"><span data-stu-id="759dc-368">Note that when you add your company registration ID you should use your business tax ID and not the customer personal ID.</span></span>

<span data-ttu-id="759dc-369">Os parceiros que fazem negócios com clientes novos ou existentes nos países/regiões a seguir já foram integrados a uma versão anterior em novembro de 2020.</span><span class="sxs-lookup"><span data-stu-id="759dc-369">Partners who do business with new or existing customers in the following countries have already been onboarded with a previous release in November 2020.</span></span>

- <span data-ttu-id="759dc-370">Armênia</span><span class="sxs-lookup"><span data-stu-id="759dc-370">Armenia</span></span>
- <span data-ttu-id="759dc-371">Azerbaijão</span><span class="sxs-lookup"><span data-stu-id="759dc-371">Azerbaijan</span></span>
- <span data-ttu-id="759dc-372">Bielorrússia</span><span class="sxs-lookup"><span data-stu-id="759dc-372">Belarus</span></span>
- <span data-ttu-id="759dc-373">Hungria</span><span class="sxs-lookup"><span data-stu-id="759dc-373">Hungary</span></span>
- <span data-ttu-id="759dc-374">Cazaquistão</span><span class="sxs-lookup"><span data-stu-id="759dc-374">Kazakhstan</span></span>
- <span data-ttu-id="759dc-375">Quirguistão</span><span class="sxs-lookup"><span data-stu-id="759dc-375">Kyrgyzstan</span></span>
- <span data-ttu-id="759dc-376">Moldova</span><span class="sxs-lookup"><span data-stu-id="759dc-376">Moldova</span></span>
- <span data-ttu-id="759dc-377">Rússia</span><span class="sxs-lookup"><span data-stu-id="759dc-377">Russia</span></span>
- <span data-ttu-id="759dc-378">Tadjiquistão</span><span class="sxs-lookup"><span data-stu-id="759dc-378">Tajikistan</span></span>
- <span data-ttu-id="759dc-379">Ucrânia</span><span class="sxs-lookup"><span data-stu-id="759dc-379">Ukraine</span></span>
- <span data-ttu-id="759dc-380">Uzbequistão</span><span class="sxs-lookup"><span data-stu-id="759dc-380">Uzbekistan</span></span>

<span data-ttu-id="759dc-381">No fim de março de 2021, os parceiros com clientes no restante do mundo poderão inserir a ID de registro da empresa, o número de telefone e o segundo nome dos clientes como detalhes opcionais.</span><span class="sxs-lookup"><span data-stu-id="759dc-381">Partners with customers in the rest of the world will have the ability at the end of March 2021 to enter the company registration ID, phone number, and middle name for customers as optional details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="759dc-382">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="759dc-382">Next steps</span></span>

- <span data-ttu-id="759dc-383">Examine a documentação técnica e as perguntas frequentes na [coleção de parceiros](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) dedicada para obter diretrizes mais detalhadas.</span><span class="sxs-lookup"><span data-stu-id="759dc-383">Review the technical documentation and frequently asked questions in the dedicated [partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>
- <span data-ttu-id="759dc-384">Prepare-se para incorporar as alterações usando a experiência do usuário da Web e a API do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="759dc-384">Prepare to incorporate the changes using Partner Center API and web user experience.</span></span> <span data-ttu-id="759dc-385">A API e os SDKs estarão disponíveis para teste.</span><span class="sxs-lookup"><span data-stu-id="759dc-385">API/SDKs will be available for testing.</span></span>
- <span data-ttu-id="759dc-386">Lembre-se de enviar os dados adicionais ao integrar novos clientes ou modificar detalhes dos clientes existentes.</span><span class="sxs-lookup"><span data-stu-id="759dc-386">Make sure to submit the additional data when onboarding new customers or modifying existing customer details.</span></span>
- <span data-ttu-id="759dc-387">Se estiver usando uma solução de CPV (fornecedor de painel de controle), consulte seu CPV.</span><span class="sxs-lookup"><span data-stu-id="759dc-387">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="759dc-388">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="759dc-388">Questions?</span></span>

<span data-ttu-id="759dc-389">Entre em contato com seu consultor fiscal ou o escritório fiscal local em caso de dúvidas relacionadas à ID de registro da empresa (também chamada de INN ou TIN).</span><span class="sxs-lookup"><span data-stu-id="759dc-389">Contact your tax advisor or local tax office if you have any questions related to the company registration ID (also called INN or TIN).</span></span> <span data-ttu-id="759dc-390">A Microsoft não pode fornecer diretrizes sobre questões fiscais.</span><span class="sxs-lookup"><span data-stu-id="759dc-390">Microsoft cannot provide guidance on tax matters.</span></span>

<span data-ttu-id="759dc-391">Caso precise de suporte para suas operações com a Microsoft, abra uma [solicitação de serviço](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span><span class="sxs-lookup"><span data-stu-id="759dc-391">If you need support with your operations with Microsoft, open a [service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

## <a name="view-this-months-product-launches-and-offers"></a><a name="1"></a><span data-ttu-id="759dc-392">Ver lançamentos e ofertas do produto neste mês</span><span class="sxs-lookup"><span data-stu-id="759dc-392">View this month’s product launches and offers</span></span>

### <a name="categories"></a><span data-ttu-id="759dc-393">Categorias</span><span class="sxs-lookup"><span data-stu-id="759dc-393">Categories</span></span>

- <span data-ttu-id="759dc-394">Data: 01/04/2021</span><span class="sxs-lookup"><span data-stu-id="759dc-394">Date: 2021-04-01</span></span>
- <span data-ttu-id="759dc-395">Funcionalidades</span><span class="sxs-lookup"><span data-stu-id="759dc-395">Capabilities</span></span>
 
### <a name="summary"></a><span data-ttu-id="759dc-396">Resumo</span><span class="sxs-lookup"><span data-stu-id="759dc-396">Summary</span></span>

<span data-ttu-id="759dc-397">O calendário de lançamento de produtos de abril de 2021 agora está publicado.</span><span class="sxs-lookup"><span data-stu-id="759dc-397">The April 2021 product launch calendar is now published.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="759dc-398">Público-alvo afetado</span><span class="sxs-lookup"><span data-stu-id="759dc-398">Impacted audience</span></span>

<span data-ttu-id="759dc-399">Todos os parceiros que fazem transações pelo programa CSP (Provedor de Soluções na Nuvem)</span><span class="sxs-lookup"><span data-stu-id="759dc-399">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="759dc-400">Detalhes</span><span class="sxs-lookup"><span data-stu-id="759dc-400">Details</span></span>

<span data-ttu-id="759dc-401">O [calendário de lançamento de produtos](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) de abril de 2021 está disponível agora na galeria de recursos de preparação de Operações.</span><span class="sxs-lookup"><span data-stu-id="759dc-401">The April 2021 [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) is now available in the Operations readiness resource gallery.</span></span> <span data-ttu-id="759dc-402">Veja os próximos lançamentos de produtos e ofertas aqui.</span><span class="sxs-lookup"><span data-stu-id="759dc-402">View the upcoming product launches and offers here.</span></span>

### <a name="next-steps"></a><span data-ttu-id="759dc-403">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="759dc-403">Next steps</span></span>

<span data-ttu-id="759dc-404">Examine o [calendário de lançamento de produtos](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) e repasse as informações aos stakeholders apropriados na sua organização.</span><span class="sxs-lookup"><span data-stu-id="759dc-404">Review the [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), and share the information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="759dc-405">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="759dc-405">Questions?</span></span>

<span data-ttu-id="759dc-406">Em caso de dúvidas adicionais sobre essas ofertas, confira as comunidades relevantes no Yammer.</span><span class="sxs-lookup"><span data-stu-id="759dc-406">For any further questions about these offers, check your relevant Yammer communities.</span></span>
