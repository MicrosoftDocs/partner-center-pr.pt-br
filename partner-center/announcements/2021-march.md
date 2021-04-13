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
ms.date: 04/02/2021
ms.openlocfilehash: 12954a5f7eafb138794de879a41026ef54c65da7
ms.sourcegitcommit: c6c741475604b8daf386fb54bb2795a6445ac887
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/05/2021
ms.locfileid: "106374375"
---
# <a name="march-2021-announcements"></a><span data-ttu-id="a1e7d-103">Comunicados de março de 2021</span><span class="sxs-lookup"><span data-stu-id="a1e7d-103">March 2021 announcements</span></span>

<span data-ttu-id="a1e7d-104">Esta página apresenta os comunicados de março de 2021 sobre o Microsoft Partner Center.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-104">This page provides the announcements for Microsoft Partner Center for March 2021.</span></span>

________________
## <a name="updated-csp-customer-address-validation-api-now-available-for-testing"></a><a name="18"></a><span data-ttu-id="a1e7d-105">API de validação de endereço de cliente do CSP atualizada agora disponível para teste</span><span class="sxs-lookup"><span data-stu-id="a1e7d-105">Updated CSP customer address validation API now available for testing</span></span>

### <a name="categories"></a><span data-ttu-id="a1e7d-106">Categorias</span><span class="sxs-lookup"><span data-stu-id="a1e7d-106">Categories</span></span>

- <span data-ttu-id="a1e7d-107">Data: 31/03/2021</span><span class="sxs-lookup"><span data-stu-id="a1e7d-107">Date: 2021-03-31</span></span>
- <span data-ttu-id="a1e7d-108">Funcionalidades</span><span class="sxs-lookup"><span data-stu-id="a1e7d-108">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="a1e7d-109">Resumo</span><span class="sxs-lookup"><span data-stu-id="a1e7d-109">Summary</span></span>

<span data-ttu-id="a1e7d-110">Diante do nosso compromisso em ajudar os parceiros e os clientes a administrar os negócios com base na confiança, convidaremos parceiros em todo o mundo para testar as alterações na API ValidateAddress.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-110">As part of our commitment to help partners and customers run their business based on trust, we will be inviting partners worldwide to test the changes to the ValidateAddress API.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a1e7d-111">Público-alvo afetado</span><span class="sxs-lookup"><span data-stu-id="a1e7d-111">Impacted audience</span></span>

<span data-ttu-id="a1e7d-112">Todos os parceiros de cobrança direta e provedores indiretos do CSP que criam ou atualizam os endereços de clientes</span><span class="sxs-lookup"><span data-stu-id="a1e7d-112">All CSP direct bill partners and indirect providers who create new or update existing customer address details</span></span>

### <a name="details"></a><span data-ttu-id="a1e7d-113">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a1e7d-113">Details</span></span>

<span data-ttu-id="a1e7d-114">O trabalho da Microsoft é baseado em confiança.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-114">Microsoft runs on trust.</span></span> <span data-ttu-id="a1e7d-115">Temos o compromisso de oferecer um método seguro e em conformidade com os requisitos para o envio da validação de endereços de clientes para a comercialização de assinaturas no programa CSP.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-115">We’re committed to providing a compliant, safe, and secure method of submitting customer address validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="a1e7d-116">Hoje, dia 31 de março de 2021, lançamos alterações na API ValidateAddress que gostaríamos que você testasse antes que elas entrem em funcionamento em junho de 2021.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-116">Today, March 31, 2021, we have introduced changes to the ValidateAddress API that we’d like to invite you to test, prior to going live with the changes in June 2021.</span></span> 

<span data-ttu-id="a1e7d-117">As alterações afetam apenas a API ValidateAddress.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-117">Note that these changes affect the ValidateAddress API only.</span></span> <span data-ttu-id="a1e7d-118">As APIs CreateCustomer e UpdateBillingProfile não foram afetadas.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-118">CreateCustomer and UpdateBillingProfile APIs are not affected.</span></span>

<span data-ttu-id="a1e7d-119">A resposta retornará uma das seguintes mensagens de status:</span><span class="sxs-lookup"><span data-stu-id="a1e7d-119">The response will return one of the following status messages:</span></span>

| <span data-ttu-id="a1e7d-120">Status</span><span class="sxs-lookup"><span data-stu-id="a1e7d-120">Status</span></span> | <span data-ttu-id="a1e7d-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1e7d-121">Description</span></span> | <span data-ttu-id="a1e7d-122">O número de endereços sugeridos retornados</span><span class="sxs-lookup"><span data-stu-id="a1e7d-122">Number of suggested addresses returned</span></span> |
|----------|-------------|-------------------|
| <span data-ttu-id="a1e7d-123">VerifiedShippable</span><span class="sxs-lookup"><span data-stu-id="a1e7d-123">VerifiedShippable</span></span> | <span data-ttu-id="a1e7d-124">O endereço foi verificado e pode ser usado para entregas.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-124">Address is verified and can be shipped to.</span></span> | <span data-ttu-id="a1e7d-125">Único</span><span class="sxs-lookup"><span data-stu-id="a1e7d-125">Single</span></span> |
| <span data-ttu-id="a1e7d-126">Verificado</span><span class="sxs-lookup"><span data-stu-id="a1e7d-126">Verified</span></span> | <span data-ttu-id="a1e7d-127">O endereço foi verificado.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-127">Address is verified.</span></span> | <span data-ttu-id="a1e7d-128">Único</span><span class="sxs-lookup"><span data-stu-id="a1e7d-128">Single</span></span> |
| <span data-ttu-id="a1e7d-129">InteractionRequired</span><span class="sxs-lookup"><span data-stu-id="a1e7d-129">InteractionRequired</span></span> | <span data-ttu-id="a1e7d-130">Os endereços sugeridos foram alterados significativamente e precisam de confirmação do usuário.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-130">Suggested address(es) has been changed significantly and needs user confirmation.</span></span> | <span data-ttu-id="a1e7d-131">Único</span><span class="sxs-lookup"><span data-stu-id="a1e7d-131">Single</span></span> |
| <span data-ttu-id="a1e7d-132">StreetPartial</span><span class="sxs-lookup"><span data-stu-id="a1e7d-132">StreetPartial</span></span> | <span data-ttu-id="a1e7d-133">A rua que consta no endereço é parcial e precisa de mais informações.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-133">The given street in the address is partial and needs more info.</span></span> | <span data-ttu-id="a1e7d-134">Múltiplo – máximo de três</span><span class="sxs-lookup"><span data-stu-id="a1e7d-134">Multiple—maximum of three</span></span>|
| <span data-ttu-id="a1e7d-135">PremisesPartial</span><span class="sxs-lookup"><span data-stu-id="a1e7d-135">PremisesPartial</span></span> | <span data-ttu-id="a1e7d-136">O local determinado (número de edifício, número do conjunto etc.) é parcial e precisa de mais informações.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-136">The given premises (building number, suite number, etc.) is partial and needs more info.</span></span> | <span data-ttu-id="a1e7d-137">Múltiplo – máximo de três</span><span class="sxs-lookup"><span data-stu-id="a1e7d-137">Multiple—maximum of three</span></span> |
| <span data-ttu-id="a1e7d-138">Vários</span><span class="sxs-lookup"><span data-stu-id="a1e7d-138">Multiple</span></span> | <span data-ttu-id="a1e7d-139">Há vários campos parciais no endereço (pode incluir StreetPartial e PremisesPartial).</span><span class="sxs-lookup"><span data-stu-id="a1e7d-139">There are multiple fields that are partial in the address (potentially also including StreetPartial and PremisesPartial).</span></span> | <span data-ttu-id="a1e7d-140">Múltiplo – máximo de três</span><span class="sxs-lookup"><span data-stu-id="a1e7d-140">Multiple—maximum of three</span></span> |
| <span data-ttu-id="a1e7d-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a1e7d-141">None</span></span> | <span data-ttu-id="a1e7d-142">O endereço está incorreto.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-142">Address is incorrect.</span></span> | <span data-ttu-id="a1e7d-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a1e7d-143">None</span></span> |
| <span data-ttu-id="a1e7d-144">NotValidated</span><span class="sxs-lookup"><span data-stu-id="a1e7d-144">NotValidated</span></span> | <span data-ttu-id="a1e7d-145">Não foi possível enviar o endereço pelo processo de validação.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-145">Address was not able to be sent through the validation process.</span></span>  | <span data-ttu-id="a1e7d-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a1e7d-146">None</span></span> |

<span data-ttu-id="a1e7d-147">Depois que um endereço for enviado para validação por meio da API ValidateAddress, o seguinte esquema de resposta será retornado:</span><span class="sxs-lookup"><span data-stu-id="a1e7d-147">Once an address has been submitted to be validated via the ValidateAddress API, the following response schema will be returned:</span></span>

```csharp

// <summary>
/// Object represents the address validation response.
/// </summary>

public class AddressValidationResponse
{
   /// <summary>
   /// Gets or sets the original address
   /// </summary>
   /// <value>
   /// Original Address
   /// </value>
   public Address OriginalAddress { get; set; }

   /// <summary>
   /// Gets or sets the suggested addresses
   /// </summary>
   /// <value>
   /// Suggested Addresses
   /// </value>
   public List<Address> SuggestedAddresses { get; set; }

   /// <summary>
   /// Gets or sets the validation status
   /// </summary>
   /// <value>
   /// Status
   /// </value>
   public string Status { get; set; }

   /// <summary>
   /// Gets or sets the validation message
   /// </summary>
   /// <value>
   /// Validation Message
   /// </value>
   public string ValidationMessage { get; set; }
   ```

<span data-ttu-id="a1e7d-148">Observe este exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-148">Take a look at this sample response.</span></span> <span data-ttu-id="a1e7d-149">Para os EUA, a resposta retornará um sufixo adicional de quatro dígitos na linha de código postal se você inserir apenas cinco dígitos para o CEP.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-149">Note that for the US, the response will return an additional four-digit suffix for the postal code line if you only enter five digits for the zip code.</span></span>

```csharp

"suggested_address": {
    "Country": "US",
    "region": "WA",
    "city": "Redmond",
    "address_line1": "1 Microsoft Way",
    "postal_Code": "98052-8300"
},
"original_address": {
    "Country": "US",
    "region": "WA",
    "city": "Redmond",
    "address_line1": "1 Micro Way",
    "postal_Code": "98052"
},
"status":  "InteractionRequired",
"validation_message": "Address field invalid for property: ‘Street’"
}
```

### <a name="next-steps"></a><span data-ttu-id="a1e7d-150">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="a1e7d-150">Next steps</span></span>

- <span data-ttu-id="a1e7d-151">Informe sua ID de locatário de área restrita ao SME (especialista no assunto) Ali Khaki para participar do teste da versão de pré-lançamento e começar a preparar-se para a atualização.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-151">Share your sandbox tenant ID with our subject matter expert (SME), Ali Khaki, to be included in the test flight, so that you can begin preparing for the update.</span></span>

- <span data-ttu-id="a1e7d-152">Se estiver usando uma solução de CPV (fornecedor de painel de controle), consulte seu CPV.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-152">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="a1e7d-153">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="a1e7d-153">Questions?</span></span>

<span data-ttu-id="a1e7d-154">Se você tiver dúvidas ou precisar de suporte para as operações com a Microsoft, entre em contato com o grupo do Yammer de suporte ao parceiro.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-154">If you have any questions or need support for your operations with Microsoft, reach out to your partner support Yammer group.</span></span>

________________
## <a name="new-exchange-admin-center-eac-experience"></a><a name="17"></a><span data-ttu-id="a1e7d-155">Nova experiência do EAC (Centro de administração do Exchange)</span><span class="sxs-lookup"><span data-stu-id="a1e7d-155">New Exchange admin center (EAC) experience</span></span>

### <a name="categories"></a><span data-ttu-id="a1e7d-156">Categorias</span><span class="sxs-lookup"><span data-stu-id="a1e7d-156">Categories</span></span>

- <span data-ttu-id="a1e7d-157">Data: 29/03/2021</span><span class="sxs-lookup"><span data-stu-id="a1e7d-157">Date: 2021-03-29</span></span>
- <span data-ttu-id="a1e7d-158">Funcionalidades</span><span class="sxs-lookup"><span data-stu-id="a1e7d-158">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="a1e7d-159">Resumo</span><span class="sxs-lookup"><span data-stu-id="a1e7d-159">Summary</span></span>

<span data-ttu-id="a1e7d-160">A partir de 27 de abril de 2021, o EAC (Centro de administração do Exchange) lançará uma nova experiência que melhorará a eficiência diária dos usuários.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-160">Starting April 27, 2021, the Exchange admin center (EAC) will roll out a new experience that will improve day-to-day efficiency for users.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a1e7d-161">Público-alvo afetado</span><span class="sxs-lookup"><span data-stu-id="a1e7d-161">Impacted audience</span></span>

<span data-ttu-id="a1e7d-162">Administradores delegados que acessam o Exchange por meio do Partner Center</span><span class="sxs-lookup"><span data-stu-id="a1e7d-162">Delegated admins accessing Exchange through Partner Center</span></span>

### <a name="details"></a><span data-ttu-id="a1e7d-163">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a1e7d-163">Details</span></span>

<span data-ttu-id="a1e7d-164">A partir de 27 de abril de 2021, os parceiros que acessam o Exchange por meio do Partner Center serão redirecionados para o novo EAC.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-164">Starting April 27, 2021, partners who navigate to Exchange through Partner Center will be redirected to the new EAC.</span></span>

<span data-ttu-id="a1e7d-165">Para acessar a nova experiência, disponível atualmente como uma versão prévia, os administradores devem selecionar o botão de alternância no canto superior direito do EAC clássico.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-165">This new experience is currently available as a preview, and admins can activate this experience by selecting the toggle on the top right corner within the classic EAC.</span></span> <span data-ttu-id="a1e7d-166">Outra opção para acessar o novo EAC é selecionar a faixa "Experimentar agora", exibida em todas as páginas.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-166">They can also navigate to the new EAC by selecting the “Try it now” banner that’s displayed on all the pages.</span></span>

<span data-ttu-id="a1e7d-167">Os benefícios do novo EAC incluem:</span><span class="sxs-lookup"><span data-stu-id="a1e7d-167">Benefits of the new EAC include:</span></span>

- <span data-ttu-id="a1e7d-168">Foram adicionados insights, relatórios e mecanismos de alerta para problemas relacionados ao fluxo de mensagens.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-168">Added insights, reports, and alert mechanisms for mail flow–related issues.</span></span> 

- <span data-ttu-id="a1e7d-169">Painéis personalizados para aumentar a produtividade.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-169">Personalized dashboards to increase productivity.</span></span>

<span data-ttu-id="a1e7d-170">Para ajudar a usar a nova experiência, vídeos estão disponíveis na seção **Treinamento e guia** sobre a nova experiência do EAC.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-170">To help you navigate through the new experience, videos are available within the **Training & Guide** section on the new EAC experience.</span></span> <span data-ttu-id="a1e7d-171">Eles apresentam uma visão geral para você usar melhor o novo portal.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-171">These will give you an overview of how you can best use the new portal.</span></span>

>[!NOTE]
><span data-ttu-id="a1e7d-172">Com essa alteração, a experiência clássica do EAC não será preterida.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-172">With this change, the classic EAC experience will not be deprecated.</span></span> <span data-ttu-id="a1e7d-173">Você receberá uma notificação com bastante antecedência antes que alterações sejam implementadas.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-173">You will be notified well in advance before any change is implemented.</span></span>

### <a name="next-steps"></a><span data-ttu-id="a1e7d-174">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="a1e7d-174">Next steps</span></span>

- <span data-ttu-id="a1e7d-175">Confira os [recursos sobre este tópico](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/), em que você pode ver capturas de tela da nova experiência.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-175">Check out the [resources about this topic](https://partner.microsoft.com/resources/collection/new-exchange-admin-center-experience#/), where you can view screenshots of the new experience.</span></span>

- <span data-ttu-id="a1e7d-176">Compartilhe essas informações com os stakeholders apropriados da sua organização.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-176">Share this information with the appropriate stakeholders in your organization.</span></span> 

### <a name="questions"></a><span data-ttu-id="a1e7d-177">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="a1e7d-177">Questions?</span></span>

<span data-ttu-id="a1e7d-178">Caso tenha dúvidas sobre essas alterações, confira as comunidades relevantes no Yammer.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-178">For any questions about these changes, check your relevant Yammer communities.</span></span>

________________
## <a name="microsoft-operations-introducing-the-product-launch-calendar"></a><a name="16"></a><span data-ttu-id="a1e7d-179">Operações da Microsoft: introdução ao calendário de lançamento de produtos</span><span class="sxs-lookup"><span data-stu-id="a1e7d-179">Microsoft Operations: Introducing the product launch calendar</span></span>

### <a name="categories"></a><span data-ttu-id="a1e7d-180">Categorias</span><span class="sxs-lookup"><span data-stu-id="a1e7d-180">Categories</span></span>

- <span data-ttu-id="a1e7d-181">Data: 25/03/2021</span><span class="sxs-lookup"><span data-stu-id="a1e7d-181">Date: 2021-03-25</span></span>
- <span data-ttu-id="a1e7d-182">Ofertas | Local de trabalho moderno</span><span class="sxs-lookup"><span data-stu-id="a1e7d-182">Offers | Modern Workplace</span></span>

### <a name="summary"></a><span data-ttu-id="a1e7d-183">Resumo</span><span class="sxs-lookup"><span data-stu-id="a1e7d-183">Summary</span></span>

<span data-ttu-id="a1e7d-184">Em resposta aos comentários dos parceiros, as Operações da Microsoft simplificarão as comunicações para lançamentos de produtos.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-184">In response to partner feedback, Microsoft Operations will streamline communications for product launches.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a1e7d-185">Público-alvo afetado</span><span class="sxs-lookup"><span data-stu-id="a1e7d-185">Impacted audience</span></span>

<span data-ttu-id="a1e7d-186">Parceiros do CSP (Provedor de Soluções na Nuvem)</span><span class="sxs-lookup"><span data-stu-id="a1e7d-186">Cloud Solution Provider (CSP) partners</span></span>

### <a name="details"></a><span data-ttu-id="a1e7d-187">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a1e7d-187">Details</span></span>

<span data-ttu-id="a1e7d-188">A Microsoft está comprometida em melhorar continuamente as experiências dos parceiros.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-188">Microsoft is committed to continually improving partner experiences.</span></span> <span data-ttu-id="a1e7d-189">Recebemos seus comentários de que vocês recebiam um número excessivo de comunicações da Microsoft, incluindo anúncios duplicados de lançamentos de produtos.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-189">We’ve had feedback from you that you’ve been receiving too many communications from Microsoft, including duplicate announcements for product launches.</span></span>

<span data-ttu-id="a1e7d-190">Em resposta aos seus comentários, a Microsoft simplificou a experiência de preparação para o lançamento de produtos para ofertas novas e atuais.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-190">In response to your feedback, Microsoft has streamlined the readiness experience for product launches for new and existing offers.</span></span>

<span data-ttu-id="a1e7d-191">Agora, apresentamos uma exibição mensal única dos lançamentos de produtos, publicada na galeria de recursos de preparação de Operações.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-191">We now provide you with a single monthly view of product launches, published in the Operations readiness resource gallery.</span></span> <span data-ttu-id="a1e7d-192">A [exibição mensal do calendário de lançamento de produtos](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) substituirá as comunicações individuais de lançamentos de produtos na galeria de recursos de preparação de Operações e nos anúncios do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-192">This monthly [product launch calendar view](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) will replace individual product launch communications in the Operations readiness resource gallery and in Partner Center announcements.</span></span>

<span data-ttu-id="a1e7d-193">Você também pode acessar o [calendário de lançamento de produtos](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) em [coleções da comunidade](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), [exibições de calendário](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated) e [boletins informativos do CSP](https://partner.microsoft.com/resources/collection/csp-monthly-update#/).</span><span class="sxs-lookup"><span data-stu-id="a1e7d-193">You can also access this [product launch calendar](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/) from [community collections](https://partner.microsoft.com/resources/collection/product-launch-calendar-collection#/), [calendar views](https://partner.microsoft.com/resources/assets#/?type=collection&search=Calendar&sort=updated), and [CSP newsletters](https://partner.microsoft.com/resources/collection/csp-monthly-update#/).</span></span> <span data-ttu-id="a1e7d-194">Quando publicarmos o calendário de lançamento de produtos de cada mês, você receberá um comunicado na galeria de recursos de preparação de Operações.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-194">We’ll notify you when we publish each month’s product launch calendar with an announcement in the Operations readiness resource gallery.</span></span>

<span data-ttu-id="a1e7d-195">Você ainda encontra as informações sobre ofertas novas e atuais na visualização e nos logs de alterações da lista de preços, bem como nos blogs de produto, nos guias de licenciamento e nas páginas de marketing de produto.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-195">You can still find information regarding new and existing offers in the price list preview and price list change logs, as well as in product blogs, licensing guides, and product marketing pages.</span></span>

<span data-ttu-id="a1e7d-196">A alteração será aplicada aos lançamentos dos seguintes produtos:</span><span class="sxs-lookup"><span data-stu-id="a1e7d-196">The change will apply to launches for the following products:</span></span>

- <span data-ttu-id="a1e7d-197">Dynamics local</span><span class="sxs-lookup"><span data-stu-id="a1e7d-197">Dynamics on-premises</span></span>
- <span data-ttu-id="a1e7d-198">Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="a1e7d-198">Microsoft 365</span></span>
- <span data-ttu-id="a1e7d-199">Microsoft Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="a1e7d-199">Microsoft Dynamics 365</span></span>
- <span data-ttu-id="a1e7d-200">Windows</span><span class="sxs-lookup"><span data-stu-id="a1e7d-200">Windows</span></span>
- <span data-ttu-id="a1e7d-201">Servidor</span><span class="sxs-lookup"><span data-stu-id="a1e7d-201">Server</span></span>  
- <span data-ttu-id="a1e7d-202">Ferramentas</span><span class="sxs-lookup"><span data-stu-id="a1e7d-202">Tools</span></span>
- <span data-ttu-id="a1e7d-203">Equipes e telecomunicações</span><span class="sxs-lookup"><span data-stu-id="a1e7d-203">Teams and Telco</span></span>

<span data-ttu-id="a1e7d-204">Continuaremos a enviar anúncios específicos para lançamentos de produtos que exigem detalhes de preparação de Operações.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-204">We’ll continue to send specific announcements for product launches that require Operations readiness details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="a1e7d-205">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="a1e7d-205">Next steps</span></span>

<span data-ttu-id="a1e7d-206">Analise os recursos relacionados a este tópico e repasse as informações aos stakeholders apropriados da sua organização.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-206">Review the resources about this topic and share this information with the appropriate stakeholders in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="a1e7d-207">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="a1e7d-207">Questions?</span></span>

<span data-ttu-id="a1e7d-208">Em caso de dúvidas adicionais sobre essas ofertas, confira as comunidades relevantes no Yammer.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-208">For any further questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="changes-to-csp-customer-onboarding-requirements"></a><a name="15"></a><span data-ttu-id="a1e7d-209">Alterações nos requisitos de integração de cliente CSP</span><span class="sxs-lookup"><span data-stu-id="a1e7d-209">Changes to CSP customer onboarding requirements</span></span>

### <a name="categories"></a><span data-ttu-id="a1e7d-210">Categorias</span><span class="sxs-lookup"><span data-stu-id="a1e7d-210">Categories</span></span>

- <span data-ttu-id="a1e7d-211">Data: 25/03/2021</span><span class="sxs-lookup"><span data-stu-id="a1e7d-211">Date: 2021-03-25</span></span>
- <span data-ttu-id="a1e7d-212">Funcionalidades</span><span class="sxs-lookup"><span data-stu-id="a1e7d-212">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="a1e7d-213">Resumo</span><span class="sxs-lookup"><span data-stu-id="a1e7d-213">Summary</span></span>

<span data-ttu-id="a1e7d-214">Como parte do nosso compromisso de ajudar parceiros e clientes a administrar os negócios com base na confiança, solicitaremos informações adicionais do cliente a partir do dia 25 de março de 2021.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-214">As part of our commitment to help partners and customers run their business based on trust, we will request additional customer information, effective March 25, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a1e7d-215">Público-alvo afetado</span><span class="sxs-lookup"><span data-stu-id="a1e7d-215">Impacted audience</span></span>

<span data-ttu-id="a1e7d-216">Os provedores indiretos e os parceiros de cobrança direta do CSP (Provedor de Soluções na Nuvem) que têm clientes novos ou atuais nos países/regiões listados na próxima seção</span><span class="sxs-lookup"><span data-stu-id="a1e7d-216">Cloud Solution Provider (CSP) direct bill partners and indirect providers who have new or existing customers in the countries listed in the next section</span></span>

### <a name="details"></a><span data-ttu-id="a1e7d-217">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a1e7d-217">Details</span></span>

<span data-ttu-id="a1e7d-218">O trabalho da Microsoft é baseado em confiança.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-218">Microsoft runs on trust.</span></span> <span data-ttu-id="a1e7d-219">Temos o compromisso de fornecer um método de validação do cliente que esteja em conformidade e que seja seguro e protegido para realizar transações de assinatura de clientes no programa CSP.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-219">We’re committed to providing a compliant, safe, and secure method of customer validation for transacting customer subscriptions in the CSP program.</span></span> <span data-ttu-id="a1e7d-220">Em 25 de março de 2021, apresentaremos os aprimoramentos da IU (interface do usuário) e da API do Partner Center que afetarão os parceiros que atendem a estes dois critérios:</span><span class="sxs-lookup"><span data-stu-id="a1e7d-220">On March 25, 2021, we will be introducing Partner Center API and user interface (UI) enhancements that will affect partners who meet both of the following criteria:</span></span>

1. <span data-ttu-id="a1e7d-221">O parceiro tem um relacionamento de cobrança direta com a Microsoft (o que significa que ele é um parceiro de cobrança direta ou um provedor indireto).</span><span class="sxs-lookup"><span data-stu-id="a1e7d-221">The partner has a direct billing relationship with Microsoft (which means that the partner is either a direct bill partner or an indirect provider).</span></span>

2. <span data-ttu-id="a1e7d-222">O parceiro faz negócios com clientes novos ou existentes nos seguintes países/regiões:</span><span class="sxs-lookup"><span data-stu-id="a1e7d-222">The partner does business with new or existing customers in the following countries:</span></span>

    - <span data-ttu-id="a1e7d-223">Tailândia</span><span class="sxs-lookup"><span data-stu-id="a1e7d-223">Thailand</span></span>
    - <span data-ttu-id="a1e7d-224">Vietnã</span><span class="sxs-lookup"><span data-stu-id="a1e7d-224">Vietnam</span></span>
    - <span data-ttu-id="a1e7d-225">Turquia</span><span class="sxs-lookup"><span data-stu-id="a1e7d-225">Turkey</span></span>
    - <span data-ttu-id="a1e7d-226">Polônia</span><span class="sxs-lookup"><span data-stu-id="a1e7d-226">Poland</span></span>
    - <span data-ttu-id="a1e7d-227">África do Sul</span><span class="sxs-lookup"><span data-stu-id="a1e7d-227">South Africa</span></span>
    - <span data-ttu-id="a1e7d-228">Índia</span><span class="sxs-lookup"><span data-stu-id="a1e7d-228">India</span></span>
    - <span data-ttu-id="a1e7d-229">Brasil</span><span class="sxs-lookup"><span data-stu-id="a1e7d-229">Brazil</span></span>
    - <span data-ttu-id="a1e7d-230">Iraque</span><span class="sxs-lookup"><span data-stu-id="a1e7d-230">Iraq</span></span>
    - <span data-ttu-id="a1e7d-231">Myanmar</span><span class="sxs-lookup"><span data-stu-id="a1e7d-231">Myanmar</span></span>
    - <span data-ttu-id="a1e7d-232">Sudão do Sul</span><span class="sxs-lookup"><span data-stu-id="a1e7d-232">South Sudan</span></span>
    - <span data-ttu-id="a1e7d-233">Arábia Saudita</span><span class="sxs-lookup"><span data-stu-id="a1e7d-233">Saudi Arabia</span></span>
    - <span data-ttu-id="a1e7d-234">Emirados Árabes Unidos</span><span class="sxs-lookup"><span data-stu-id="a1e7d-234">United Arab Emirates</span></span>
    - <span data-ttu-id="a1e7d-235">Venezuela</span><span class="sxs-lookup"><span data-stu-id="a1e7d-235">Venezuela</span></span>

<span data-ttu-id="a1e7d-236">Os parceiros que atendem aos critérios precisarão enviar a **ID de registro da empresa** (também conhecido como o **INN da organização** do cliente) e o **número de telefone** do cliente ao integrar clientes ou modificar os detalhes deles.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-236">Partners who meet the criteria will have to submit a customer's **company registration ID** (also known as the customer's **organization INN**) and **phone number** when they onboard new customers or modify existing customer details.</span></span> <span data-ttu-id="a1e7d-237">Esses parceiros também podem inserir um **segundo nome** opcional para o cliente.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-237">These partners can also enter an optional **middle name** for the customer.</span></span>

<span data-ttu-id="a1e7d-238">Observe que, ao adicionar a ID de registro da sua empresa, você deve usar o número de identificação de contribuinte da sua empresa e não a ID pessoal do cliente.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-238">Note that when you add your company registration ID you should use your business tax ID and not the customer personal ID.</span></span>

<span data-ttu-id="a1e7d-239">Os parceiros que fazem negócios com clientes novos ou existentes nos países/regiões a seguir já foram integrados a uma versão anterior em novembro de 2020.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-239">Partners who do business with new or existing customers in the following countries have already been onboarded with a previous release in November 2020.</span></span>

- <span data-ttu-id="a1e7d-240">Armênia</span><span class="sxs-lookup"><span data-stu-id="a1e7d-240">Armenia</span></span>
- <span data-ttu-id="a1e7d-241">Azerbaijão</span><span class="sxs-lookup"><span data-stu-id="a1e7d-241">Azerbaijan</span></span>
- <span data-ttu-id="a1e7d-242">Bielorrússia</span><span class="sxs-lookup"><span data-stu-id="a1e7d-242">Belarus</span></span>
- <span data-ttu-id="a1e7d-243">Hungria</span><span class="sxs-lookup"><span data-stu-id="a1e7d-243">Hungary</span></span>
- <span data-ttu-id="a1e7d-244">Cazaquistão</span><span class="sxs-lookup"><span data-stu-id="a1e7d-244">Kazakhstan</span></span>
- <span data-ttu-id="a1e7d-245">Quirguistão</span><span class="sxs-lookup"><span data-stu-id="a1e7d-245">Kyrgyzstan</span></span>
- <span data-ttu-id="a1e7d-246">Moldova</span><span class="sxs-lookup"><span data-stu-id="a1e7d-246">Moldova</span></span>
- <span data-ttu-id="a1e7d-247">Rússia</span><span class="sxs-lookup"><span data-stu-id="a1e7d-247">Russia</span></span>
- <span data-ttu-id="a1e7d-248">Tadjiquistão</span><span class="sxs-lookup"><span data-stu-id="a1e7d-248">Tajikistan</span></span>
- <span data-ttu-id="a1e7d-249">Ucrânia</span><span class="sxs-lookup"><span data-stu-id="a1e7d-249">Ukraine</span></span>
- <span data-ttu-id="a1e7d-250">Uzbequistão</span><span class="sxs-lookup"><span data-stu-id="a1e7d-250">Uzbekistan</span></span>

<span data-ttu-id="a1e7d-251">No dia 25 de março de 2021, os parceiros com clientes no restante do mundo poderão inserir a **ID de registro da empresa**, o **número de telefone** e o **segundo nome** dos clientes como detalhes opcionais.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-251">Partners with customers in the rest of the world will have the ability on March 25, 2021 to enter the **company registration ID**, **phone number**, and **middle name** for customers as optional details.</span></span>

### <a name="next-steps"></a><span data-ttu-id="a1e7d-252">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="a1e7d-252">Next steps</span></span>

- <span data-ttu-id="a1e7d-253">Examine a documentação técnica e as perguntas frequentes na [coleção de parceiros dedicada](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) para obter diretrizes mais detalhadas.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-253">Review the technical documentation and frequently asked questions in the [dedicated partner collection](https://partner.microsoft.com/resources/collection/additionalfields-csp-customers-selected-geos#/) for more detailed guidance.</span></span>

- <span data-ttu-id="a1e7d-254">Prepare-se para incorporar as alterações usando a experiência do usuário da Web e a API do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-254">Prepare to incorporate the changes using the Partner Center API and web user experience.</span></span> <span data-ttu-id="a1e7d-255">A API e os SDKs estarão disponíveis para teste.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-255">API/SDKs will be available for testing.</span></span>

- <span data-ttu-id="a1e7d-256">Lembre-se de enviar os dados adicionais ao integrar novos clientes ou modificar detalhes dos clientes existentes.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-256">Make sure to submit the additional data when onboarding new customers or modifying existing customer details.</span></span>

- <span data-ttu-id="a1e7d-257">Se estiver usando uma solução de CPV (fornecedor de painel de controle), consulte seu CPV.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-257">If you’re using a control panel vendor (CPV) solution, consult your CPV.</span></span>

### <a name="questions"></a><span data-ttu-id="a1e7d-258">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="a1e7d-258">Questions?</span></span>

<span data-ttu-id="a1e7d-259">Entre em contato com seu consultor fiscal ou o escritório fiscal local em caso de dúvidas relacionadas ao identificador legal (também chamado de INN ou TIN).</span><span class="sxs-lookup"><span data-stu-id="a1e7d-259">Contact your tax advisor or local tax office if you have any questions related to the legal identifier (also called INN or TIN).</span></span> <span data-ttu-id="a1e7d-260">A Microsoft não pode fornecer diretrizes sobre questões fiscais.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-260">Microsoft cannot provide guidance on tax matters.</span></span>

<span data-ttu-id="a1e7d-261">Caso precise obter suporte para suas operações com a Microsoft, [abra uma solicitação de serviço](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span><span class="sxs-lookup"><span data-stu-id="a1e7d-261">If you need support in your operations with Microsoft, [open a service request](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=2&topicid=aa679372-d996-73df-e244-cb28bbbf28e8).</span></span>

________________
## <a name="corrections-made-to-march-1-2021-perpetual-software-price-list"></a><a name="14"></a><span data-ttu-id="a1e7d-262">Correções feitas na lista de preços de software perpétuo de 1º de março de 2021</span><span class="sxs-lookup"><span data-stu-id="a1e7d-262">Corrections made to March 1, 2021 perpetual software price list</span></span>

### <a name="categories"></a><span data-ttu-id="a1e7d-263">Categorias</span><span class="sxs-lookup"><span data-stu-id="a1e7d-263">Categories</span></span>

- <span data-ttu-id="a1e7d-264">Data: 23/03/2021</span><span class="sxs-lookup"><span data-stu-id="a1e7d-264">Date: 2021-03-23</span></span>
- <span data-ttu-id="a1e7d-265">Ofertas/mercados</span><span class="sxs-lookup"><span data-stu-id="a1e7d-265">Offers/Markets</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a1e7d-266">Público-alvo afetado</span><span class="sxs-lookup"><span data-stu-id="a1e7d-266">Impacted audience</span></span>

<span data-ttu-id="a1e7d-267">Provedores indiretos e parceiros de cobrança direta realizando transações de software perpétuo no programa do Provedor de Soluções na Nuvem</span><span class="sxs-lookup"><span data-stu-id="a1e7d-267">Indirect providers and direct bill partners transacting perpetual software in the Cloud Solution Provider program</span></span> 

### <a name="details"></a><span data-ttu-id="a1e7d-268">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a1e7d-268">Details</span></span>

<span data-ttu-id="a1e7d-269">A lista de preços para software perpétuo publicada em 1º de março de 2021 incluiu mercados que não deveriam estar lá.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-269">The price list for perpetual software posted on March 1, 2021 included markets that should not have been there.</span></span> <span data-ttu-id="a1e7d-270">A lista de preços de software perpétuo foi atualizada em 17 de março de 2021 com as devidas correções.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-270">The perpetual software price list was updated on March 17, 2021 with the corrections.</span></span> <span data-ttu-id="a1e7d-271">Tais correções aplicavam-se somente a:</span><span class="sxs-lookup"><span data-stu-id="a1e7d-271">These corrections were only applicable to:</span></span>

- <span data-ttu-id="a1e7d-272">ID do produto: DF77X4D43RKT</span><span class="sxs-lookup"><span data-stu-id="a1e7d-272">Product ID: DF77X4D43RKT</span></span> 
- <span data-ttu-id="a1e7d-273">Nome do produto: atualização do Windows 10 Home para Pro para Microsoft 365 Business</span><span class="sxs-lookup"><span data-stu-id="a1e7d-273">Product name: Windows 10 Home to Pro Upgrade for Microsoft 365 Business</span></span>
- <span data-ttu-id="a1e7d-274">Mercados removidos ou sem suporte: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG, NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM e ZW</span><span class="sxs-lookup"><span data-stu-id="a1e7d-274">Removed or unsupported markets: AE, AF, AL, AM, AO, BA, BB, BD, BH, BM, BN, BO, BR, BS, BW, BY, BZ, CI, CL, CM, CO, CR, CW, DO, DZ, EC, EG, ET, FJ, FO, GE, GH, GT, HN, IL, IN, IQ, JM, JO, KE, KG, KN, KW, KY, KZ, LB, LK, LY, MA, MC, MD, ME, MN, MO, MU, NA, NG, NI, NP, OM, PA, PE, PH, PK, PR, PY, QA, RS, RU, RW, SG, SN, SV, TH, TJ, TM, TN, TT, TZ, UA, UG, UY, UZ, VE, VN, YE, ZM, ZW</span></span>

<span data-ttu-id="a1e7d-275">Essas alterações se aplicam somente ao produto acima.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-275">These changes only apply to the above product.</span></span> <span data-ttu-id="a1e7d-276">Os demais produtos não tiveram correções.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-276">Other products had no corrections.</span></span> 

### <a name="next-steps-and-resources"></a><span data-ttu-id="a1e7d-277">Próximas etapas e recursos</span><span class="sxs-lookup"><span data-stu-id="a1e7d-277">Next steps and resources</span></span>

- <span data-ttu-id="a1e7d-278">Os parceiros que realizam transações com software perpétuo devem baixar a mais recente lista de preços de software perpétuo.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-278">Partners who transact perpetual software should download the latest perpetual software price list.</span></span>
- <span data-ttu-id="a1e7d-279">Consulte os [códigos de país da região](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) para ver o mapeamento correto da abreviação dos países com apenas duas letras.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-279">Consult the [region country codes](https://docs.microsoft.com/azure/marketplace/commercial-marketplace-co-sell-countries) for a friendly mapping of the two letter abbreviation to countries.</span></span>
________________
## <a name="sdk-release-on-net-standard-v1170"></a><a name="13"></a> <span data-ttu-id="a1e7d-280">Lançamento do SDK no .NET Standard (v1.17.0)</span><span class="sxs-lookup"><span data-stu-id="a1e7d-280">SDK Release on .NET Standard (v1.17.0)</span></span>

### <a name="categories"></a><span data-ttu-id="a1e7d-281">Categorias</span><span class="sxs-lookup"><span data-stu-id="a1e7d-281">Categories</span></span>

- <span data-ttu-id="a1e7d-282">Data: 23/03/2021</span><span class="sxs-lookup"><span data-stu-id="a1e7d-282">Date: 2021-03-23</span></span>

- <span data-ttu-id="a1e7d-283">Capacidades</span><span class="sxs-lookup"><span data-stu-id="a1e7d-283">Capabilities</span></span>
 
### <a name="impacted-audience"></a><span data-ttu-id="a1e7d-284">Público-alvo afetado</span><span class="sxs-lookup"><span data-stu-id="a1e7d-284">Impacted audience</span></span>

<span data-ttu-id="a1e7d-285">Parceiros do programa CSP Direct Bill Partner e fornecedores do programa CSP Indirect Provider que estão usando o SDK do .NET do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-285">Direct Bill partners and Indirect Providers participating in the CSP program who are using the Partner Center .NET SDK.</span></span>

### <a name="details"></a><span data-ttu-id="a1e7d-286">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a1e7d-286">Details</span></span>

<span data-ttu-id="a1e7d-287">Desde 23 de março de 2020, os parceiros já podem baixar a versão do [MicrosoftPartnerCenter.NETSDK (Galeria do NuGet | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), juntamente com as [amostras públicas atualizadas do GitHub](https://github.com/Microsoft/Partner-Center-DotNet-Samples) do SDK do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-287">As of March 23 2020, Partners can start downloading the version of [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0), along with updated public Partner Center SDK [GitHub samples](https://github.com/Microsoft/Partner-Center-DotNet-Samples).</span></span> <span data-ttu-id="a1e7d-288">Esta versão inclui atualizações para os seguintes métodos:</span><span class="sxs-lookup"><span data-stu-id="a1e7d-288">This version includes updates to the following methods:</span></span>

#### <a name="audit-updated-new-operation-types"></a><span data-ttu-id="a1e7d-289">Auditoria atualizada: novos tipos de operação</span><span class="sxs-lookup"><span data-stu-id="a1e7d-289">Audit Updated: New operation types</span></span>

<span data-ttu-id="a1e7d-290">Adicionados novos [tipos de operação](https://docs.microsoft.com/partner-center/develop/auditing-resources) para saber quando o cliente aprovou e terminou o DAP.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-290">Added new [operation types](https://docs.microsoft.com/partner-center/develop/auditing-resources) for knowing when the customer approved and terminated DAP.</span></span>

- <span data-ttu-id="a1e7d-291">DapAdminRelationshipApproved</span><span class="sxs-lookup"><span data-stu-id="a1e7d-291">DapAdminRelationshipApproved</span></span>

- <span data-ttu-id="a1e7d-292">DapAdminRelationshipTerminated</span><span class="sxs-lookup"><span data-stu-id="a1e7d-292">DapAdminRelationshipTerminated</span></span>

#### <a name="audit-updated-new-resource-and-operation-types"></a><span data-ttu-id="a1e7d-293">Auditoria atualizada: novos tipos de recurso e operação</span><span class="sxs-lookup"><span data-stu-id="a1e7d-293">Audit Updated: New resource and operation types</span></span>

<span data-ttu-id="a1e7d-294">Adição de novos [tipos de recursos e operação](https://docs.microsoft.com/partner-center/develop/auditing-resources) para dar suporte ao cenário de função de diretório do cliente.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-294">Added new [resource and operation types](https://docs.microsoft.com/partner-center/develop/auditing-resources) for supporting the customer directory role scenario.</span></span>

- <span data-ttu-id="a1e7d-295">Novo tipo de recurso "CustomerDirectoryRole"</span><span class="sxs-lookup"><span data-stu-id="a1e7d-295">New resource type “CustomerDirectoryRole”</span></span>

- <span data-ttu-id="a1e7d-296">Tipos de operação "AddUserMember" e "RemoveUserMember"</span><span class="sxs-lookup"><span data-stu-id="a1e7d-296">Operation types “AddUserMember” and “RemoveUserMember”</span></span>

#### <a name="sdk-updates-to-customer-accounts"></a><span data-ttu-id="a1e7d-297">Atualizações do SDK para contas de clientes</span><span class="sxs-lookup"><span data-stu-id="a1e7d-297">SDK Updates to customer accounts</span></span>

- <span data-ttu-id="a1e7d-298">Suporte para GET/customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus</span><span class="sxs-lookup"><span data-stu-id="a1e7d-298">Support for GET /customers/{customer-tenant-id}/directSignedMicrosoftCustomerAgreementStatus</span></span>

- <span data-ttu-id="a1e7d-299">GET /customers/{customer-tenant-id}/qualifications</span><span class="sxs-lookup"><span data-stu-id="a1e7d-299">GET /customers/{customer-tenant-id}/qualifications</span></span>

- <span data-ttu-id="a1e7d-300">POST /customers/{customer_id}/qualifications?code={validationCode}</span><span class="sxs-lookup"><span data-stu-id="a1e7d-300">POST /customers/{customer_id}/qualifications?code={validationCode}</span></span>

#### <a name="additional-changes"></a><span data-ttu-id="a1e7d-301">Alterações adicionais</span><span class="sxs-lookup"><span data-stu-id="a1e7d-301">Additional changes</span></span>

<span data-ttu-id="a1e7d-302">As seguintes alterações são introduzidas como parte do Novo Comércio e atualmente estão disponíveis somente por convite para parceiros que fazem parte da visualização técnica da experiência de Novo Comércio M365/D365.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-302">The following changes are introduced as part of New Commerce, and are currently available by invitation only to partners who are part of the M365/D365 New Commerce experience technical preview.</span></span> <span data-ttu-id="a1e7d-303">Os parceiros que não fazem parte da visualização técnica do Novo Comércio não devem notar os impactos e devem ser compatíveis com versões anteriores.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-303">Partners who are not part of the New Commerce technical preview should not notice impacts and should be backward compatible.</span></span>

- <span data-ttu-id="a1e7d-304">Alterações no catálogo:</span><span class="sxs-lookup"><span data-stu-id="a1e7d-304">Catalog Changes:</span></span>

  - <span data-ttu-id="a1e7d-305">GET /products/{product-id}/skus/{sku-id}</span><span class="sxs-lookup"><span data-stu-id="a1e7d-305">GET /products/{product-id}/skus/{sku-id}</span></span>

- <span data-ttu-id="a1e7d-306">Comprar e gerenciar:</span><span class="sxs-lookup"><span data-stu-id="a1e7d-306">Purchase and Manage:</span></span>
  - <span data-ttu-id="a1e7d-307">GET /customers/{customerId}/subscriptions</span><span class="sxs-lookup"><span data-stu-id="a1e7d-307">GET /customers/{customerId}/subscriptions</span></span>
  - <span data-ttu-id="a1e7d-308">GET /customers/{customerId}/subscriptions/{subscriptionId}</span><span class="sxs-lookup"><span data-stu-id="a1e7d-308">GET /customers/{customerId}/subscriptions/{subscriptionId}</span></span>
  - <span data-ttu-id="a1e7d-309">PATCH /customers/{customerId}/subscriptions/{subscriptionId}</span><span class="sxs-lookup"><span data-stu-id="a1e7d-309">PATCH /customers/{customerId}/subscriptions/{subscriptionId}</span></span>
  - <span data-ttu-id="a1e7d-310">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities</span><span class="sxs-lookup"><span data-stu-id="a1e7d-310">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitioneligibilities</span></span>
  - <span data-ttu-id="a1e7d-311">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span><span class="sxs-lookup"><span data-stu-id="a1e7d-311">GET /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span></span>
  - <span data-ttu-id="a1e7d-312">POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span><span class="sxs-lookup"><span data-stu-id="a1e7d-312">POST /customers/{customerId}/subscriptions/{subscriptionId}/transitions</span></span>

### <a name="next-steps"></a><span data-ttu-id="a1e7d-313">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="a1e7d-313">Next Steps</span></span>

- <span data-ttu-id="a1e7d-314">Baixar a versão mais recente do [MicrosoftPartnerCenter.NETSDK (Galeria do NuGet | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)</span><span class="sxs-lookup"><span data-stu-id="a1e7d-314">Download the latest version [MicrosoftPartnerCenter.NETSDK (NuGet Gallery | Microsoft.Store.PartnerCenter 1.17.0)](https://www.nuget.org/packages/Microsoft.Store.PartnerCenter/1.17.0)</span></span>
- <span data-ttu-id="a1e7d-315">Baixe e examine as [amostras do GitHub](https://github.com/Microsoft/Partner-Center-DotNet-Samples)</span><span class="sxs-lookup"><span data-stu-id="a1e7d-315">Download and review the [GitHub samples](https://github.com/Microsoft/Partner-Center-DotNet-Samples)</span></span>

________________
## <a name="csp-commercial-marketplace-offer-and-fy21-csp-incentives-for-eligible-offers"></a><a name="12"></a><span data-ttu-id="a1e7d-316">Oferta do marketplace comercial do CSP e incentivos do CSP no ano fiscal de 2021 para ofertas qualificadas</span><span class="sxs-lookup"><span data-stu-id="a1e7d-316">CSP commercial marketplace offer and FY21 CSP incentives for eligible offers</span></span>

### <a name="categories"></a><span data-ttu-id="a1e7d-317">Categorias</span><span class="sxs-lookup"><span data-stu-id="a1e7d-317">Categories</span></span>

- <span data-ttu-id="a1e7d-318">Data: 18/03/2021</span><span class="sxs-lookup"><span data-stu-id="a1e7d-318">Date: 2021-03-18</span></span>
- <span data-ttu-id="a1e7d-319">Capacidades</span><span class="sxs-lookup"><span data-stu-id="a1e7d-319">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a1e7d-320">Público-alvo afetado</span><span class="sxs-lookup"><span data-stu-id="a1e7d-320">Impacted audience</span></span>

<span data-ttu-id="a1e7d-321">Provedores indiretos e parceiros de cobrança direta do programa Provedor de Soluções na Nuvem</span><span class="sxs-lookup"><span data-stu-id="a1e7d-321">Indirect providers and direct bill partners in the Cloud Solution Provider program</span></span> 

### <a name="details"></a><span data-ttu-id="a1e7d-322">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a1e7d-322">Details</span></span>

<span data-ttu-id="a1e7d-323">Provedores indiretos e parceiros de cobrança direta no programa de Provedor de Soluções na Nuvem podem vender ofertas de terceiros e receber um incentivo de reembolso para cada oferta de terceiros qualificada transacionada no Partner Center ou no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-323">Indirect providers and direct bill partners in the Cloud Solution Provider program can sell third party offers and earn a rebate incentive for each eligible third-party offer transacted in Partner Center or the Azure portal.</span></span> <span data-ttu-id="a1e7d-324">O incentivo será oferecido na forma de reembolso sobre as vendas cobradas de ofertas qualificadas e estará **disponível até 30 de junho de 2021**.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-324">The incentive will be in the form of a rebate on billed sales for the eligible offers and is **available until June 30, 2021**.</span></span>  

<span data-ttu-id="a1e7d-325">Saiba mais abaixo sobre este incentivo para Ofertas do Marketplace Comercial dos CSP e entre em contato com seus clientes hoje mesmo para identificar as ofertas corretas a fim de habilitar o sucesso contínuo e transformação digital deles.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-325">Continue learning about this CSP Commercial Marketplace Offer incentive below and contact your customers today to identify the right offers to enable their continued success and digital transformation.</span></span>

<span data-ttu-id="a1e7d-326">Firmamos parcerias com ISVs (fornecedores independentes de software) para trazer as soluções de IaaS e SaaS mais recentes ao mercado a fim de atender aos clientes da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-326">We partner with Independent Software Vendors (ISVs) to bring the latest IaaS and SaaS solutions to market for Microsoft customers.</span></span> <span data-ttu-id="a1e7d-327">Os distribuidores ISV têm a opção de habilitar as vendas de suas ofertas por meio do canal Microsoft Partner.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-327">ISV publishers have the option of enabling sales of their offers through the Microsoft partner channel.</span></span> <span data-ttu-id="a1e7d-328">Nossas ofertas qualificadas para receber o incentivo se enquadram em duas categorias:</span><span class="sxs-lookup"><span data-stu-id="a1e7d-328">Our incentive-eligible offers fall into two categories:</span></span>

- <span data-ttu-id="a1e7d-329">Algumas ofertas SaaS e IaaS de terceiros com status incentivado de venda conjunta do Azure IP.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-329">Select SaaS and IaaS third-party offers with Azure IP co-sell incentivized status.</span></span> 

- <span data-ttu-id="a1e7d-330">Aplicativos SaaS integrados com o Teams ou pelo menos dois aplicativos de produtividade do Microsoft 365, como PowerPoint, Word, Excel, Outlook ou SharePoint.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-330">SaaS applications integrated with Teams or at least two Microsoft 365 productivity apps, such as PowerPoint, Word, Excel, Outlook, or SharePoint.</span></span>

### <a name="next-steps-and-resources"></a><span data-ttu-id="a1e7d-331">Próximas etapas e recursos</span><span class="sxs-lookup"><span data-stu-id="a1e7d-331">Next steps and resources</span></span>

- <span data-ttu-id="a1e7d-332">Saiba mais sobre a conquista de [Incentivos de Parceiros](https://partner.microsoft.com/membership/partner-incentives) pela venda dos aplicativos do Marketplace qualificados para incentivos.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-332">Learn about earning [Partner Incentives](https://partner.microsoft.com/membership/partner-incentives) for selling eligible marketplace apps the incentive eligible apps.</span></span> <span data-ttu-id="a1e7d-333">Novas ofertas são adicionadas mensalmente.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-333">New offers are added monthly.</span></span>  
- [<span data-ttu-id="a1e7d-334">Recursos de incentivo para parceiro de cobrança direta do programa Provedor de Soluções na Nuvem</span><span class="sxs-lookup"><span data-stu-id="a1e7d-334">Cloud Solution Provider direct bill partner incentive resources</span></span>](https://partner.microsoft.com/asset/collection/cloud-solution-provider-direct-partner-incentive-resources#/)
- [<span data-ttu-id="a1e7d-335">Recursos de incentivo para provedor indireto no programa Provedor de Soluções na Nuvem</span><span class="sxs-lookup"><span data-stu-id="a1e7d-335">Cloud Solution Provider indirect provider incentive resources</span></span>](https://partner.microsoft.com/asset/collection/cloud-solution-provider-indirect-provider-incentive-resources#/)
- <span data-ttu-id="a1e7d-336">Examine esta [apresentação](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) para saber mais sobre como vender os aplicativos do marketplace comercial.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-336">Review this [presentation](https://partner.microsoft.com/resources/detail/partner-center-cm-for-csp-overview-pdf) to learn more about selling the commercial marketplace apps.</span></span> <span data-ttu-id="a1e7d-337">Confira os recursos adicionais [aqui](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/).</span><span class="sxs-lookup"><span data-stu-id="a1e7d-337">Check out additional resources [here](https://partner.microsoft.com/resources/collection/partner-center-cm-for-csp-collection#/).</span></span> 
- <span data-ttu-id="a1e7d-338">Explorar o catálogo do marketplace comercial no [Partner Center](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) ou no [portal do Azure](https://ms.portal.azure.com/#home)</span><span class="sxs-lookup"><span data-stu-id="a1e7d-338">Explore the commercial marketplace catalog in [Partner Center](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-discover) or [Azure portal](https://ms.portal.azure.com/#home)</span></span>
- <span data-ttu-id="a1e7d-339">Usar [APIs](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) para integrar aplicativos ao marketplace da sua empresa</span><span class="sxs-lookup"><span data-stu-id="a1e7d-339">Use [APIs](https://docs.microsoft.com/partner-center/develop/create-subscription-azure-marketplace-products#get-a-list-of-offers-for-a-market) to integrate apps into your company’s marketplace</span></span>
- <span data-ttu-id="a1e7d-340">Entre em contato com os ISVs com quem está interessado em fazer negócios</span><span class="sxs-lookup"><span data-stu-id="a1e7d-340">Reach out to ISVs you are interested in doing business with</span></span>
- <span data-ttu-id="a1e7d-341">Os provedores indiretos precisam se integrar usando APIs e orientar os revendedores sobre quais aplicativos vender</span><span class="sxs-lookup"><span data-stu-id="a1e7d-341">Indirect providers need to integrate using APIs and guide resellers on which apps to sell</span></span>

### <a name="questions"></a><span data-ttu-id="a1e7d-342">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="a1e7d-342">Questions?</span></span>  

<span data-ttu-id="a1e7d-343">Confira [este artigo](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) para obter uma visão geral do marketplace comercial no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-343">Refer to [this article](https://docs.microsoft.com/partner-center/csp-commercial-marketplace-overview) for an overview of the commercial marketplace in Partner Center.</span></span>

<span data-ttu-id="a1e7d-344">Para obter assistência adicional, crie uma solicitação de suporte no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-344">If you need additional assistance you can create a support request in Partner Center.</span></span> <span data-ttu-id="a1e7d-345">Saiba mais em [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1).</span><span class="sxs-lookup"><span data-stu-id="a1e7d-345">Learn more at [https://aka.ms/IncentivesSupport](https://partner.microsoft.com/dashboard/support/servicerequests/create?stage=1).</span></span>

________________
## <a name="power-bi-premium-offer-naming-and-prerequisite-update"></a><a name="11"></a><span data-ttu-id="a1e7d-346">Atualizações de nomenclatura e pré-requisitos da oferta do Power BI Premium</span><span class="sxs-lookup"><span data-stu-id="a1e7d-346">Power BI Premium offer naming and prerequisite update</span></span>

### <a name="categories"></a><span data-ttu-id="a1e7d-347">Categorias</span><span class="sxs-lookup"><span data-stu-id="a1e7d-347">Categories</span></span>

- <span data-ttu-id="a1e7d-348">Data: 18/03/2021</span><span class="sxs-lookup"><span data-stu-id="a1e7d-348">Date: 2021-03-18</span></span>
- <span data-ttu-id="a1e7d-349">Funcionalidades</span><span class="sxs-lookup"><span data-stu-id="a1e7d-349">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="a1e7d-350">Resumo</span><span class="sxs-lookup"><span data-stu-id="a1e7d-350">Summary</span></span>

<span data-ttu-id="a1e7d-351">A lista de preços final de 1º de abril de 2021 será atualizada para esclarecer as informações de nomenclatura e/ou pré-requisitos das ofertas do Power BI Premium por usuário.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-351">The April 1, 2021 final price list will be updated to add clarity to the naming and/or prerequisite information for Power BI Premium Per User offers.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a1e7d-352">Público-alvo afetado</span><span class="sxs-lookup"><span data-stu-id="a1e7d-352">Impacted audience</span></span>

<span data-ttu-id="a1e7d-353">Parceiros diretos e indiretos do programa CSP (Provedor de Soluções na Nuvem)</span><span class="sxs-lookup"><span data-stu-id="a1e7d-353">Cloud Solution Provider (CSP) direct and indirect partners</span></span>

### <a name="details"></a><span data-ttu-id="a1e7d-354">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a1e7d-354">Details</span></span>

<span data-ttu-id="a1e7d-355">A lista de preços final de 1º de abril de 2021 será atualizada para esclarecer as informações de nomenclatura e/ou pré-requisitos das ofertas do Power BI Premium por usuário.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-355">The April 1, 2021 final price list will be updated to add clarity to the naming and/or prerequisite information for Power BI Premium Per User offers.</span></span>

<span data-ttu-id="a1e7d-356">Até que a lista de preços final seja atualizada, use as informações desta seção para efetuar pedidos dos produtos corretos.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-356">Until the final price list is updated, use the information in this section to ensure that the correct product is ordered.</span></span>

<span data-ttu-id="a1e7d-357">A seguir são mostrados os detalhes do SKU e dos pré-requisitos afetados.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-357">The following details show the affected SKU and prerequisite details.</span></span>

| <span data-ttu-id="a1e7d-358">Nome de exibição da oferta na versão prévia da lista de preços de 1º de março</span><span class="sxs-lookup"><span data-stu-id="a1e7d-358">Offer display name on March 1 price list preview</span></span> |  <span data-ttu-id="a1e7d-359">Nome de exibição da oferta atualizada na lista de preços final de 1º de abril</span><span class="sxs-lookup"><span data-stu-id="a1e7d-359">Updated offer display name on April 1 final price list</span></span>| <span data-ttu-id="a1e7d-360">ID da oferta</span><span class="sxs-lookup"><span data-stu-id="a1e7d-360">Offer ID</span></span> |
| ------ | ----------- | ----------- |
| <span data-ttu-id="a1e7d-361">Complemento do Power BI Premium por Usuário (preço de equipe sem fins lucrativos)</span><span class="sxs-lookup"><span data-stu-id="a1e7d-361">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span>  |  <span data-ttu-id="a1e7d-362">Complemento do Power BI Premium por Usuário **(Office)** (preço para equipes de organizações sem fins lucrativos)</span><span class="sxs-lookup"><span data-stu-id="a1e7d-362">Power BI Premium Per User Add-On **(Office)** (Nonprofit Staff Pricing)</span></span>   | <span data-ttu-id="a1e7d-363">31c03289-47ab-4ab0-8df1-03742c127ac6</span><span class="sxs-lookup"><span data-stu-id="a1e7d-363">31c03289-47ab-4ab0-8df1-03742c127ac6</span></span>   |

<span data-ttu-id="a1e7d-364">Os clientes precisam ter um dos seguintes pré-requisitos para adquirir essa oferta:</span><span class="sxs-lookup"><span data-stu-id="a1e7d-364">Customers are required to have any one of the following prerequisites to purchase this offer:</span></span>

| <span data-ttu-id="a1e7d-365">Nome de exibição da oferta</span><span class="sxs-lookup"><span data-stu-id="a1e7d-365">Offer display name</span></span> | <span data-ttu-id="a1e7d-366">ID da oferta</span><span class="sxs-lookup"><span data-stu-id="a1e7d-366">Offer ID</span></span> |
| ------ | ----------- |
| <span data-ttu-id="a1e7d-367">Microsoft 365 E5 (preço para equipes de organizações sem fins lucrativos)</span><span class="sxs-lookup"><span data-stu-id="a1e7d-367">Microsoft 365 E5 (Nonprofit Staff Pricing)</span></span>  |  <span data-ttu-id="a1e7d-368">31bedf01-9e57-4ece-a53a-d3656a563931</span><span class="sxs-lookup"><span data-stu-id="a1e7d-368">31bedf01-9e57-4ece-a53a-d3656a563931</span></span>   |
|   <span data-ttu-id="a1e7d-369">Microsoft 365 E5 sem conferência de áudio (preço para equipes de organizações sem fins lucrativos)</span><span class="sxs-lookup"><span data-stu-id="a1e7d-369">Microsoft 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="a1e7d-370">b456810a-c414-4e07-98fc-ef74e8175a09</span><span class="sxs-lookup"><span data-stu-id="a1e7d-370">b456810a-c414-4e07-98fc-ef74e8175a09</span></span>|
|   <span data-ttu-id="a1e7d-371">Office 365 E5 (preço para equipes de organizações sem fins lucrativos)</span><span class="sxs-lookup"><span data-stu-id="a1e7d-371">Office 365 E5 (Nonprofit Staff Pricing)</span></span>| <span data-ttu-id="a1e7d-372">ce139fe5-8bd5-47ed-a5be-07c286f8b9e</span><span class="sxs-lookup"><span data-stu-id="a1e7d-372">ce139fe5-8bd5-47ed-a5be-07c286f8b9e</span></span>    |
|   <span data-ttu-id="a1e7d-373">Office 365 E5 (preço para equipes de organizações sem fins lucrativos) Avaliação</span><span class="sxs-lookup"><span data-stu-id="a1e7d-373">Office 365 E5 (Nonprofit Staff Pricing) Trial</span></span>|  <span data-ttu-id="a1e7d-374">2f192efe-608a-4c9c-9d19-2b0b70b0962e</span><span class="sxs-lookup"><span data-stu-id="a1e7d-374">2f192efe-608a-4c9c-9d19-2b0b70b0962e</span></span>|
|   <span data-ttu-id="a1e7d-375">Office 365 E5 sem conferência de áudio (preço para equipes de organizações sem fins lucrativos)</span><span class="sxs-lookup"><span data-stu-id="a1e7d-375">Office 365 E5 without Audio Conferencing (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="a1e7d-376">c3897426-9f49-4eaf-9b4d-7d9a1c72aef7</span><span class="sxs-lookup"><span data-stu-id="a1e7d-376">c3897426-9f49-4eaf-9b4d-7d9a1c72aef7</span></span>|

<span data-ttu-id="a1e7d-377">A seguinte oferta do Power BI Premium tem um pré-requisito obrigatório para a compra:</span><span class="sxs-lookup"><span data-stu-id="a1e7d-377">The following Power BI Premium offer has a prerequisite required for purchase:</span></span>

| <span data-ttu-id="a1e7d-378">Nome de exibição da oferta</span><span class="sxs-lookup"><span data-stu-id="a1e7d-378">Offer display name</span></span> | <span data-ttu-id="a1e7d-379">ID da oferta</span><span class="sxs-lookup"><span data-stu-id="a1e7d-379">Offer ID</span></span> |
| ------ | ----------- |
|   <span data-ttu-id="a1e7d-380">Complemento do Power BI Premium por Usuário (preço de equipe sem fins lucrativos)</span><span class="sxs-lookup"><span data-stu-id="a1e7d-380">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span>|  <span data-ttu-id="a1e7d-381">ef0b895b-681b-4026-a5b1-dda182a57d40</span><span class="sxs-lookup"><span data-stu-id="a1e7d-381">ef0b895b-681b-4026-a5b1-dda182a57d40</span></span> |

<span data-ttu-id="a1e7d-382">Os clientes precisam ter este pré-requisito para adquirir essa oferta:</span><span class="sxs-lookup"><span data-stu-id="a1e7d-382">Customers are required to have this prerequisite to purchase this offer:</span></span>

| <span data-ttu-id="a1e7d-383">Nome de exibição da oferta</span><span class="sxs-lookup"><span data-stu-id="a1e7d-383">Offer display name</span></span> | <span data-ttu-id="a1e7d-384">ID da oferta</span><span class="sxs-lookup"><span data-stu-id="a1e7d-384">Offer ID</span></span> |
| ------ |----------|
| <span data-ttu-id="a1e7d-385">Power BI Pro (preço para equipes de organizações sem fins lucrativos)</span><span class="sxs-lookup"><span data-stu-id="a1e7d-385">Power BI Pro (Nonprofit Staff Pricing)</span></span>  |   <span data-ttu-id="a1e7d-386">cabdfc93-5786-4224-bfd3-35d58f833b35</span><span class="sxs-lookup"><span data-stu-id="a1e7d-386">cabdfc93-5786-4224-bfd3-35d58f833b35</span></span> |

### <a name="next-steps"></a><span data-ttu-id="a1e7d-387">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="a1e7d-387">Next steps</span></span>

<span data-ttu-id="a1e7d-388">Examine os recursos relacionados a esse tópico e compartilhe essas informações com os stakeholders apropriados da organização.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-388">Review the resources about this topic, and share this information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="a1e7d-389">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="a1e7d-389">Questions?</span></span>

<span data-ttu-id="a1e7d-390">Caso tenha dúvidas sobre essas ofertas, confira as comunidades relevantes no Yammer.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-390">For any questions about these offers, check your relevant Yammer communities.</span></span> 

## <a name="march-price-updates-for-microsoft-365-f3"></a><a name="10"></a> <span data-ttu-id="a1e7d-391">Atualizações de preço de março para Microsoft 365 F3</span><span class="sxs-lookup"><span data-stu-id="a1e7d-391">March price updates for Microsoft 365 F3</span></span>

### <a name="categories"></a><span data-ttu-id="a1e7d-392">Categorias</span><span class="sxs-lookup"><span data-stu-id="a1e7d-392">Categories</span></span>

- <span data-ttu-id="a1e7d-393">Data: 16/03/2021</span><span class="sxs-lookup"><span data-stu-id="a1e7d-393">Date: 2021-03-16</span></span>
- <span data-ttu-id="a1e7d-394">Ofertas/mercados</span><span class="sxs-lookup"><span data-stu-id="a1e7d-394">Offers/Markets</span></span>

### <a name="summary"></a><span data-ttu-id="a1e7d-395">Resumo</span><span class="sxs-lookup"><span data-stu-id="a1e7d-395">Summary</span></span>

<span data-ttu-id="a1e7d-396">Os preços incorretos de março de 2021 para Microsoft 365 F3 em GBP (libras esterlinas) e EUR (euro) foram corrigidos.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-396">Incorrect March 2021 pricing has been corrected for Microsoft 365 F3 British Pound (GBP) and Euro (EUR).</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a1e7d-397">Público-alvo afetado</span><span class="sxs-lookup"><span data-stu-id="a1e7d-397">Impacted audience</span></span>

<span data-ttu-id="a1e7d-398">Parceiros que compraram o Microsoft 365 F3 em GBP ou EUR entre os dias 1º e 17 de março de 2021 por meio do programa CSP (Provedor de Soluções na Nuvem).</span><span class="sxs-lookup"><span data-stu-id="a1e7d-398">Partners purchasing Microsoft 365 F3 in GBP or EUR between March 1 and March 17, 2021 through the Cloud Solution Provider (CSP) program.</span></span>

### <a name="details"></a><span data-ttu-id="a1e7d-399">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a1e7d-399">Details</span></span>

<span data-ttu-id="a1e7d-400">A Microsoft corrigiu os preços incorretos do Microsoft 365 F3.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-400">Microsoft has resolved incorrect pricing for Microsoft 365 F3.</span></span> <span data-ttu-id="a1e7d-401">Os preços estavam incorretos apenas em GBP e EUR e somente nas ofertas adquiridas entre os dias 1º e 17 de março de 2021.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-401">The incorrect prices were for GBP and EUR and only for offers purchased between March 1 and March 17, 2021.</span></span> <span data-ttu-id="a1e7d-402">As ofertas e as moedas afetadas estão listadas abaixo.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-402">The impacted offers and currencies are listed below.</span></span> 

| <span data-ttu-id="a1e7d-403">Nome da oferta</span><span class="sxs-lookup"><span data-stu-id="a1e7d-403">Offer name</span></span> | <span data-ttu-id="a1e7d-404">Moeda</span><span class="sxs-lookup"><span data-stu-id="a1e7d-404">Currency</span></span> | <span data-ttu-id="a1e7d-405">ID da oferta</span><span class="sxs-lookup"><span data-stu-id="a1e7d-405">Offer ID</span></span> | <span data-ttu-id="a1e7d-406">ID do material</span><span class="sxs-lookup"><span data-stu-id="a1e7d-406">Material ID</span></span> |
| ------ |----------- |----------- |----------- |
| <span data-ttu-id="a1e7d-407">Microsoft 365 F3 (caridade)</span><span class="sxs-lookup"><span data-stu-id="a1e7d-407">Microsoft 365 F3 (Charity)</span></span> | <span data-ttu-id="a1e7d-408">GBP</span><span class="sxs-lookup"><span data-stu-id="a1e7d-408">GBP</span></span> | <span data-ttu-id="a1e7d-409">57b722c2-c435-4bfb-9bc8-80509213a13a</span><span class="sxs-lookup"><span data-stu-id="a1e7d-409">57b722c2-c435-4bfb-9bc8-80509213a13a</span></span> | <span data-ttu-id="a1e7d-410">AAD-11626</span><span class="sxs-lookup"><span data-stu-id="a1e7d-410">AAD-11626</span></span> |
| <span data-ttu-id="a1e7d-411">Microsoft 365 F3 (comercial)</span><span class="sxs-lookup"><span data-stu-id="a1e7d-411">Microsoft 365 F3 (Commercial)</span></span> | <span data-ttu-id="a1e7d-412">EUR</span><span class="sxs-lookup"><span data-stu-id="a1e7d-412">EUR</span></span>| <span data-ttu-id="a1e7d-413">3451a3b0-8cda-44a7-bad7-c30be81c4aaa</span><span class="sxs-lookup"><span data-stu-id="a1e7d-413">3451a3b0-8cda-44a7-bad7-c30be81c4aaa</span></span> | <span data-ttu-id="a1e7d-414">AAA-89898</span><span class="sxs-lookup"><span data-stu-id="a1e7d-414">AAA-89898</span></span> |
 
<span data-ttu-id="a1e7d-415">As versões prévias das listas de preços baseadas em licença de março e abril foram atualizadas em 16 de março, às 17h, horário padrão do Pacífico.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-415">The March and April preview license-base price lists were updated March 16, 5PM pacific standard time.</span></span>

### <a name="next-steps"></a><span data-ttu-id="a1e7d-416">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="a1e7d-416">Next steps</span></span>

- <span data-ttu-id="a1e7d-417">Os parceiros devem baixar novamente as listas de preços atuais baseadas em licença, tanto da versão prévia de março quanto de abril, com essas correções de preços, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-417">Partners should redownload the current license-based price lists, both March and the April preview, with these price corrections if applicable.</span></span>  
- <span data-ttu-id="a1e7d-418">A Microsoft entrará em contato por email com os parceiros afetados nas próximas semanas para informar sobre o que fazer em seguida com relação à correção das transações afetadas.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-418">Microsoft will be contacting impacted partners in the coming weeks via email to inform them of next steps related to correcting affected transactions.</span></span>

### <a name="questions"></a><span data-ttu-id="a1e7d-419">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="a1e7d-419">Questions?</span></span>

<span data-ttu-id="a1e7d-420">Em caso de dúvidas adicionais, confira as comunidades relevantes sobre o CSP no Yammer.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-420">For any further questions please check your relevant CSP Yammer communities.</span></span>

________________

## <a name="update-a-legal-company-name-through-partner-center"></a><a name="9"></a> <span data-ttu-id="a1e7d-421">Atualizar a razão social de uma empresa por meio do Partner Center</span><span class="sxs-lookup"><span data-stu-id="a1e7d-421">Update a legal company name through Partner Center</span></span>

### <a name="categories"></a><span data-ttu-id="a1e7d-422">Categorias</span><span class="sxs-lookup"><span data-stu-id="a1e7d-422">Categories</span></span>

- <span data-ttu-id="a1e7d-423">Data: 16/03/2021</span><span class="sxs-lookup"><span data-stu-id="a1e7d-423">Date: 2021-03-16</span></span>
- <span data-ttu-id="a1e7d-424">Conduza Eficiência e Escala</span><span class="sxs-lookup"><span data-stu-id="a1e7d-424">Drive Efficiency & Scale</span></span>

### <a name="summary"></a><span data-ttu-id="a1e7d-425">Resumo</span><span class="sxs-lookup"><span data-stu-id="a1e7d-425">Summary</span></span>

<span data-ttu-id="a1e7d-426">Desde março de 2021, os parceiros do MPN (Microsoft Partner Network) e os revendedores indiretos do CSP (Provedor de Soluções na Nuvem) podem atualizar a razão social da empresa por meio do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-426">Starting March 2021, Microsoft Partner Network (MPN) partners and Cloud Solution Provider (CSP) indirect resellers can update their legal company name through Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a1e7d-427">Público-alvo afetado</span><span class="sxs-lookup"><span data-stu-id="a1e7d-427">Impacted audience</span></span>

<span data-ttu-id="a1e7d-428">Parceiros do MPN e revendedores indiretos do CSP (não aplicável a parceiros de cobrança direta do CSP)</span><span class="sxs-lookup"><span data-stu-id="a1e7d-428">MPN partners and CSP indirect resellers (not applicable to CSP direct bill partners)</span></span>

### <a name="details"></a><span data-ttu-id="a1e7d-429">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a1e7d-429">Details</span></span>

<span data-ttu-id="a1e7d-430">Desde março de 2021, os parceiros do MPN e os revendedores indiretos do CSP podem atualizar a razão social da empresa por meio do Partner Center com conformidade e de maneira autônoma.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-430">Starting March 2021, MPN partners and CSP indirect resellers can update their legal company name through Partner Center in a compliant, self-serve manner.</span></span> <span data-ttu-id="a1e7d-431">Com esse novo recurso, os parceiros não precisarão mais enviar um tíquete de suporte do Partner Center para atualizar o nome da empresa.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-431">With this new feature, partners will no longer need to submit a Partner Center support ticket to update their company name.</span></span> <span data-ttu-id="a1e7d-432">Isso economizará muito tempo para os parceiros na execução dessas atividades.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-432">This will save a significant amount of time for partners when performing these activities.</span></span> 

<span data-ttu-id="a1e7d-433">Para saber mais, confira [Atualizar seu perfil comercial legal](../update-your-partner-profile.md#update-your-legal-business-profile).</span><span class="sxs-lookup"><span data-stu-id="a1e7d-433">To learn more, see [Update your legal business profile](../update-your-partner-profile.md#update-your-legal-business-profile).</span></span>

>[!NOTE]
><span data-ttu-id="a1e7d-434">Verifique se o nome da empresa no perfil comercial legal não tem erros de ortografia nem abreviações e se ele corresponde exatamente aos registros comerciais formais da empresa.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-434">Ensure that the company name in your legal business profile is free of spelling errors and abbreviations, and exactly matches your formal company business registration records.</span></span> <span data-ttu-id="a1e7d-435">Para mais informações sobre como atualizar o perfil da sua organização, veja [Verificar o perfil da organização](../update-your-partner-profile.md#update-your-legal-business-profile).</span><span class="sxs-lookup"><span data-stu-id="a1e7d-435">For more information on updating your organization profile, refer to [Verify your organization profile](../update-your-partner-profile.md#update-your-legal-business-profile).</span></span>

### <a name="next-steps"></a><span data-ttu-id="a1e7d-436">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="a1e7d-436">Next steps</span></span>

<span data-ttu-id="a1e7d-437">Compartilhe essas informações em sua organização para que a equipe correta possa examinar e atualizar os processos delas.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-437">Share this information within your organization so that the appropriate team can review and update their processes.</span></span>

### <a name="questions"></a><span data-ttu-id="a1e7d-438">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="a1e7d-438">Questions?</span></span>

<span data-ttu-id="a1e7d-439">Em caso de dúvidas adicionais, confira as comunidades relevantes sobre o CSP no Yammer.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-439">For any further questions please check your relevant CSP Yammer communities.</span></span>

________________
## <a name="update-to-cloud-solution-provider-csp-program-evolution-and-open-license-program-changes"></a><a name="8"></a> <span data-ttu-id="a1e7d-440">Atualização sobre a evolução do programa CSP (Provedor de Soluções na Nuvem) e as alterações do programa Open License</span><span class="sxs-lookup"><span data-stu-id="a1e7d-440">Update to Cloud Solution Provider (CSP) program evolution and Open License program changes</span></span>

### <a name="categories"></a><span data-ttu-id="a1e7d-441">Categorias</span><span class="sxs-lookup"><span data-stu-id="a1e7d-441">Categories</span></span>

- <span data-ttu-id="a1e7d-442">Data: 15/03/2021</span><span class="sxs-lookup"><span data-stu-id="a1e7d-442">Date: 2021-03-15</span></span>
- <span data-ttu-id="a1e7d-443">Funcionalidades</span><span class="sxs-lookup"><span data-stu-id="a1e7d-443">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="a1e7d-444">Resumo</span><span class="sxs-lookup"><span data-stu-id="a1e7d-444">Summary</span></span>

<span data-ttu-id="a1e7d-445">Novas ofertas de software perpétuo para o setor público e comercial estão chegando ao programa CSP (Provedor de Soluções na Nuvem), juntamente com alterações no programa de Licenciamento Aberto.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-445">New commercial and public sector perpetual software offers are coming to the Cloud Solution Provider (CSP) program along with changes to the Open Licensing program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a1e7d-446">Público-alvo afetado</span><span class="sxs-lookup"><span data-stu-id="a1e7d-446">Impacted audience</span></span>

<span data-ttu-id="a1e7d-447">Distribuidores comerciais e revendedores gerenciados que fazem vendas usando o programa Open License e todos os parceiros CSP que realizam transações com software perpétuo</span><span class="sxs-lookup"><span data-stu-id="a1e7d-447">Commercial distributors and managed resellers selling through the Open License program, as well as all CSP partners transacting perpetual software</span></span>

### <a name="details"></a><span data-ttu-id="a1e7d-448">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a1e7d-448">Details</span></span>

<span data-ttu-id="a1e7d-449">Em setembro de 2020, a Microsoft [anunciou](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) uma série de etapas em nosso percurso de transformação digital para expandir oportunidades para parceiros no programa CSP, incluindo a disponibilidade de software local para parceiros.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-449">In September 2020, Microsoft [announced](https://blogs.partner.microsoft.com/mpn/expanding-opportunities-for-partners-in-the-cloud-solution-provider-program/) a series of steps in our digital transformation journey to expand opportunities to partners in the CSP program, including the availability of on-premises software for partners.</span></span> <span data-ttu-id="a1e7d-450">Essas mudanças permitem que os parceiros expandam os negócios e ampliem o alcance deles aproveitando as licenças de software no CSP, preparando-os para ter sucesso no atual mundo que prioriza a nuvem.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-450">These changes enable partners to grow their business and extend their reach by leveraging software licenses in CSP, positioning them for success in today’s cloud-first world.</span></span> <span data-ttu-id="a1e7d-451">Elas também capacitam as transições dos clientes para a nuvem e dão aos parceiros a flexibilidade necessária para ambientes de nuvem híbrida.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-451">They also empower customers’ transitions to the cloud and give partners the flexibility needed for customer hybrid cloud environments.</span></span>

<span data-ttu-id="a1e7d-452">Na continuação dessa transformação digital, estamos anunciando as seguintes mudanças:</span><span class="sxs-lookup"><span data-stu-id="a1e7d-452">In continuation of this digital transformation, we are announcing the following changes:</span></span>

- <span data-ttu-id="a1e7d-453">1º de julho de 2021: não serão adicionados SKUs, produtos nem promoções à lista de preços do programa Open License.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-453">July 1, 2021:  No new SKUs, products, or promotions will be added to the Open License program price list.</span></span>

- <span data-ttu-id="a1e7d-454">7 de julho de 2021: duas ofertas comerciais, Get Genuine Windows e Visual Studio Professional, e ofertas para o setor público (governamental, educação e sem fins lucrativos – veja o [comunicado](./2020-december.md#9)) serão adicionadas à lista de preços do software perpétuo do CSP.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-454">July 7, 2021:  Two commercial offers, Get Genuine Windows and Visual Studio Professional, and public sector offers (government, education and nonprofit – see [announcement](./2020-december.md#9)) will be added to the CSP perpetual software price list.</span></span>  <span data-ttu-id="a1e7d-455">A lista de preços pode ser encontrada na seção Software da página [Vender > Preços e Ofertas](https://partnercenter.microsoft.com/pcv/sales) no Partner Center e será publicada novamente nessa data.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-455">The price list can be found in the Software section of the [Sell > Pricing & Offers](https://partnercenter.microsoft.com/pcv/sales) page in Partner Center and will be republished on this date.</span></span>

<span data-ttu-id="a1e7d-456">Para obter detalhes completos sobre a evolução do programa CSP e as mudanças no programa Open License, confira as **Próximas Etapas** abaixo.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-456">For full details regarding the CSP program evolution and Open License program changes, please see **Next Steps** below.</span></span>

### <a name="next-steps"></a><span data-ttu-id="a1e7d-457">Próximas etapas:</span><span class="sxs-lookup"><span data-stu-id="a1e7d-457">Next Steps:</span></span>

- <span data-ttu-id="a1e7d-458">Evolução do programa CSP: examine os materiais de preparação sobre [Software perpétuo no programa Provedor de Soluções na Nuvem](https://partner.microsoft.com/resources/collection/software-in-csp#/).</span><span class="sxs-lookup"><span data-stu-id="a1e7d-458">CSP Program evolution:  Review the [Perpetual software in the Cloud Solution Provider program](https://partner.microsoft.com/resources/collection/software-in-csp#/) readiness materials.</span></span> <span data-ttu-id="a1e7d-459">Use este [mapa de preparação](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) para localizar de maneira rápida as informações corretas para sua função.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-459">Use this [readiness map](https://partner.microsoft.com/resources/detail/software-in-csp-readiness-map-pdf) to quickly locate the right information for your role.</span></span>

- <span data-ttu-id="a1e7d-460">Mudanças no programa Open License: examine os materiais de preparação [Evolução do programa CSP e mudanças no programa Open License](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/).</span><span class="sxs-lookup"><span data-stu-id="a1e7d-460">Open License program changes:  Review the [CSP program evolution and Open License program changes](https://partner.microsoft.com/resources/collection/csp-open-evolution-to-a-better-experience#/) readiness materials.</span></span> <span data-ttu-id="a1e7d-461">Use este [mapa de preparação](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) para localizar de maneira rápida as informações corretas para sua função.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-461">Use this [readiness map](https://partner.microsoft.com/resources/detail/csp-open-evolution-to-a-better-experience-readiness-map-pdf) to quickly locate the right information for your role.</span></span>

### <a name="questions"></a><span data-ttu-id="a1e7d-462">Perguntas</span><span class="sxs-lookup"><span data-stu-id="a1e7d-462">Questions</span></span>

<span data-ttu-id="a1e7d-463">Em caso de dúvidas adicionais, confira as comunidades relevantes sobre o CSP no Yammer.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-463">For any further questions please check your relevant CSP Yammer communities.</span></span>

_______________
## <a name="update-to-a-previous-announcement-premium-assessments-an-add-on-to-compliance-manager"></a><a name="7"></a><span data-ttu-id="a1e7d-464">Atualização sobre um comunicado anterior: Avaliações Premium e complemento do Gerenciador de Conformidade</span><span class="sxs-lookup"><span data-stu-id="a1e7d-464">Update to a previous announcement: Premium Assessments, an add-on to Compliance Manager</span></span>

### <a name="categories"></a><span data-ttu-id="a1e7d-465">Categorias</span><span class="sxs-lookup"><span data-stu-id="a1e7d-465">Categories</span></span>

- <span data-ttu-id="a1e7d-466">Data: 15/03/2021</span><span class="sxs-lookup"><span data-stu-id="a1e7d-466">Date: 2021-03-15</span></span>
- <span data-ttu-id="a1e7d-467">Amplie seu negócio</span><span class="sxs-lookup"><span data-stu-id="a1e7d-467">Grow your business</span></span>

### <a name="summary"></a><span data-ttu-id="a1e7d-468">Resumo</span><span class="sxs-lookup"><span data-stu-id="a1e7d-468">Summary</span></span>

<span data-ttu-id="a1e7d-469">As ofertas de avaliação não deveriam ter sido listadas na lista de preço e serão removidas.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-469">The trial offers shouldn’t have been listed on the price list and will be removed.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a1e7d-470">Público-alvo afetado</span><span class="sxs-lookup"><span data-stu-id="a1e7d-470">Impacted audience</span></span>

<span data-ttu-id="a1e7d-471">Parceiros que fazem transações pelo programa Provedor de Soluções na Nuvem</span><span class="sxs-lookup"><span data-stu-id="a1e7d-471">Partners transacting through Cloud Solution Provider</span></span>

### <a name="details"></a><span data-ttu-id="a1e7d-472">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a1e7d-472">Details</span></span>

<span data-ttu-id="a1e7d-473">As ofertas de avaliação não deveriam ter sido incluídas na lista de preços.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-473">The trial offers shouldn’t have been included in the price list.</span></span> <span data-ttu-id="a1e7d-474">Elas serão removidas da lista de preços de 1º de maio de 2021.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-474">These will be removed from the May 1, 2021 price list.</span></span>

<span data-ttu-id="a1e7d-475">O comunicado original está [aqui](./2021-february.md#4).</span><span class="sxs-lookup"><span data-stu-id="a1e7d-475">The original announcement is [here](./2021-february.md#4).</span></span>

### <a name="additional-resources"></a><span data-ttu-id="a1e7d-476">Recursos adicionais</span><span class="sxs-lookup"><span data-stu-id="a1e7d-476">Additional resources</span></span>

- [<span data-ttu-id="a1e7d-477">Segurança e conformidade do Microsoft 365 E5</span><span class="sxs-lookup"><span data-stu-id="a1e7d-477">Microsoft 365 E5 security and compliance</span></span>](https://www.microsoft.com/licensing/product-licensing/microsoft-365-enterprise?activetab=m365-enterprise:primaryr5)

- [<span data-ttu-id="a1e7d-478">Criar e gerenciar as avaliações no Gerenciador de Conformidade da Microsoft – Conformidade do Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="a1e7d-478">Build and manage assessments in Microsoft Compliance Manager - Microsoft 365 Compliance</span></span>](/microsoft-365/compliance/compliance-manager-assessments)

### <a name="next-steps"></a><span data-ttu-id="a1e7d-479">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="a1e7d-479">Next steps</span></span>

<span data-ttu-id="a1e7d-480">Examine os recursos relacionados a esse tópico e compartilhe essas informações com os stakeholders apropriados da organização.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-480">Review the resources about this topic, and share this information with the appropriate stakeholders in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="a1e7d-481">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="a1e7d-481">Questions?</span></span>

<span data-ttu-id="a1e7d-482">Caso tenha dúvidas sobre essas ofertas, confira as comunidades relevantes no Yammer.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-482">For questions about these offers, check your relevant Yammer communities.</span></span>

________________
## <a name="migrate-your-solutions-from-one-commercial-partner-ocp-go-to-market-gtm-to-the-microsoft-commercial-marketplace"></a><a name="6"></a> <span data-ttu-id="a1e7d-483">Migrar suas soluções OCP (One Commercial Partner) GTM (go-to-market) para o marketplace comercial da Microsoft</span><span class="sxs-lookup"><span data-stu-id="a1e7d-483">Migrate your solutions from One Commercial Partner (OCP) go-to market (GTM) to the Microsoft commercial marketplace</span></span>

### <a name="categories"></a><span data-ttu-id="a1e7d-484">Categorias</span><span class="sxs-lookup"><span data-stu-id="a1e7d-484">Categories</span></span>

- <span data-ttu-id="a1e7d-485">Data: 12/03/2021</span><span class="sxs-lookup"><span data-stu-id="a1e7d-485">Date: 2021-03-12</span></span>
- <span data-ttu-id="a1e7d-486">Funcionalidades</span><span class="sxs-lookup"><span data-stu-id="a1e7d-486">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="a1e7d-487">Resumo</span><span class="sxs-lookup"><span data-stu-id="a1e7d-487">Summary</span></span>

<span data-ttu-id="a1e7d-488">A partir de 29 de março de 2021, você começará a experimentar funcionalidades da OCP (One Commercial Partner) GTM (go-to-market) limitadas.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-488">From March 29, 2021, you will begin to experience limited One Commercial Partner (OCP) go-to market (GTM) capabilities.</span></span> <span data-ttu-id="a1e7d-489">Incentivamos você a migrar suas soluções para o marketplace comercial no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-489">We encourage you to migrate your solutions to the commercial marketplace in Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a1e7d-490">Público-alvo afetado</span><span class="sxs-lookup"><span data-stu-id="a1e7d-490">Impacted audience</span></span>

<span data-ttu-id="a1e7d-491">Organizações que fazem vendas conjuntas com soluções OCP GTM</span><span class="sxs-lookup"><span data-stu-id="a1e7d-491">Organizations co-selling with solutions in OCP GTM</span></span>

### <a name="details"></a><span data-ttu-id="a1e7d-492">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a1e7d-492">Details</span></span>

<span data-ttu-id="a1e7d-493">Em dezembro de 2020, iniciamos o percurso desde a ferramenta Microsoft OCP GTM até o marketplace comercial da Microsoft no Partner Center.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-493">In December 2020, we started our journey from the Microsoft OCP GTM tool to the Microsoft commercial marketplace in Partner Center.</span></span> <span data-ttu-id="a1e7d-494">Essa transição expande as funcionalidades do marketplace comercial em que você pode demonstrar suas soluções para milhões de clientes, compartilhar oportunidades de maneira bidirecional com outros vendedores parceiros e da Microsoft e vender soluções inovadoras em conjunto.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-494">This transition expands the capabilities of the commercial marketplace where you can showcase your solutions to millions of customers, bidirectionally share opportunities with other Microsoft and partner sellers, and jointly sell innovative solutions.</span></span>

<span data-ttu-id="a1e7d-495">O próximo marco da transição ocorrerá em 29 de março de 2021.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-495">The next milestone in the transition will take place on March 29, 2021.</span></span> <span data-ttu-id="a1e7d-496">É quando você começará a experimentar funcionalidades da OCP GTM limitadas, com alguns campos se tornando somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-496">That’s when you’ll begin to experience limited OCP GTM capabilities, with some fields becoming read-only.</span></span> <span data-ttu-id="a1e7d-497">Se, no momento, você estiver fazendo venda conjunta de soluções na OCP GTM, recomendamos que migre suas soluções para o marketplace comercial para aproveitar as funcionalidades dele e simplificar sua experiência de publicação.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-497">If you’re currently co-selling with solutions in OCP GTM, we encourage you to migrate your solutions to the commercial marketplace to take advantage of its capabilities and simplify your publishing experience.</span></span> 

<span data-ttu-id="a1e7d-498">A migração para o marketplace comercial faz do Partner Center o principal destino para a experiência de publicação de venda conjunta.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-498">Moving to the commercial marketplace makes Partner Center the primary destination for the co-sell publishing experience.</span></span> <span data-ttu-id="a1e7d-499">É lá que você pode continuar expandindo seus negócios conectando suas soluções com nossos clientes compartilhados por meio dos mesmos canais e de experiências no produto que usamos para produtos da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-499">It’s where you can continue to grow your business by connecting your solutions with our shared customers through the same channels and in-product experiences that we use for Microsoft products.</span></span> <span data-ttu-id="a1e7d-500">[Saiba mais sobre o marketplace comercial](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).</span><span class="sxs-lookup"><span data-stu-id="a1e7d-500">[Learn more about the commercial marketplace](https://blogs.partner.microsoft.com/mpn/getting-started-with-the-microsoft-commercial-marketplace/).</span></span>

### <a name="next-steps"></a><span data-ttu-id="a1e7d-501">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="a1e7d-501">Next steps</span></span>

- <span data-ttu-id="a1e7d-502">Se você ainda não tiver migrado suas soluções, siga as instruções detalhadas no [guia de transição](/azure/marketplace/co-sell-solution-migration) ou veja o [tutorial de vídeo passo a passo](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) para concluir todas as atividades de migração e começar a publicar suas soluções no marketplace comercial.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-502">If you have not yet moved your solutions, follow the instructions detailed in the [transition guide](/azure/marketplace/co-sell-solution-migration) or view the [step-by-step video tutorial](https://partner.microsoft.com/asset/detail/ocp-gtm-to-the-microsoft-commercial-marketplace-mp4) to complete all migration activities and start publishing your solution(s) in the commercial marketplace.</span></span>

- <span data-ttu-id="a1e7d-503">Caso tenha dúvidas sobre a experiência de funcionalidade limitada na OCP GTM, veja as [Perguntas frequentes sobre requisitos de venda conjunta para publicação no marketplace comercial da Microsoft](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf).</span><span class="sxs-lookup"><span data-stu-id="a1e7d-503">For questions regarding the limited capability experience in OCP GTM, view the [Co-sell requirements to publish in the Microsoft commercial marketplace FAQ](https://partner.microsoft.com/resources/detail/co-sell-requirements-publish-commercial-marketplace-faq-pdf).</span></span> <span data-ttu-id="a1e7d-504">(Confira a seção "Funcionalidades limitadas da OCP GTM a partir de 29 de março de 2021".)</span><span class="sxs-lookup"><span data-stu-id="a1e7d-504">(See the section “OCP GTM limited capabilities starting March 29, 2021.”)</span></span>

### <a name="questions"></a><span data-ttu-id="a1e7d-505">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="a1e7d-505">Questions?</span></span>

<span data-ttu-id="a1e7d-506">Entre em contato com o [suporte](https://partner.microsoft.com/support/?stage=1) se você tiver dúvidas ou precisar de mais informações.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-506">Contact [Support](https://partner.microsoft.com/support/?stage=1) if you have any questions or need more information.</span></span>

________________
## <a name="expanding-the-new-commerce-experience-in-the-cloud-solution-provider-csp-program-for-azure-to-russia"></a><a name="5"></a><span data-ttu-id="a1e7d-507">Expandir a nova experiência de comércio no programa CSP (Provedor de Soluções na Nuvem) para Azure para a Rússia</span><span class="sxs-lookup"><span data-stu-id="a1e7d-507">Expanding the new commerce experience in the Cloud Solution Provider (CSP) program for Azure to Russia</span></span>

### <a name="categories"></a><span data-ttu-id="a1e7d-508">Categorias</span><span class="sxs-lookup"><span data-stu-id="a1e7d-508">Categories</span></span>

- <span data-ttu-id="a1e7d-509">Data: 10/03/2021</span><span class="sxs-lookup"><span data-stu-id="a1e7d-509">Date: 2021-03-10</span></span>
- <span data-ttu-id="a1e7d-510">Capacidades</span><span class="sxs-lookup"><span data-stu-id="a1e7d-510">Capabilities</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a1e7d-511">Público-alvo afetado</span><span class="sxs-lookup"><span data-stu-id="a1e7d-511">Impacted audience</span></span>

<span data-ttu-id="a1e7d-512">Todos os parceiros na Rússia que fazem transações pelo programa CSP (Provedor de Soluções na Nuvem).</span><span class="sxs-lookup"><span data-stu-id="a1e7d-512">All partners in Russia transacting through the Cloud Solution Provider (CSP) program.</span></span>

### <a name="details"></a><span data-ttu-id="a1e7d-513">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a1e7d-513">Details</span></span>

<span data-ttu-id="a1e7d-514">Desde 10 de março de 2021, estamos empolgados em anunciar a disponibilidade da **nova experiência de comércio no CSP para Azure na Rússia**.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-514">Starting March 10 2021, we’re excited to announce the availability of the **new commerce experience in CSP for Azure in Russia**.</span></span> <span data-ttu-id="a1e7d-515">Essa experiência vai simplificar e aprimorar a maneira como os clientes compram e consomem os serviços do Azure.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-515">This experience will streamline and improve the way customers buy and consume Azure services.</span></span> <span data-ttu-id="a1e7d-516">Ela também dará aos parceiros do programa CSP uma visão consistente do preço do Azure nos movimentos de vendas, o preço em dólares para consistência global, o alinhamento da data de cobrança e o acesso ao Gerenciamento de Custos do Azure.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-516">It will also give partners in the CSP program a consistent view of Azure pricing across sales motions, USD pricing for global consistency, billing date alignment, and access to Azure Cost Management.</span></span>

### <a name="next-steps"></a><span data-ttu-id="a1e7d-517">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="a1e7d-517">Next steps</span></span>

<span data-ttu-id="a1e7d-518">Há vários recursos disponíveis que apresentam a nova experiência de comércio do Azure e fornecem mais informações.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-518">There are several resources available introducing the new Azure commerce experience and providing additional information.</span></span> <span data-ttu-id="a1e7d-519">Encontre as perguntas frequentes mais recentes, apresentações, vídeos e muito mais na [Galeria de Recursos de Atualizações do Programa CSP](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).</span><span class="sxs-lookup"><span data-stu-id="a1e7d-519">Find the latest FAQs, decks, video and more in the [CSP Program Updates Resource Gallery](https://partner.microsoft.com/resources/collection/new-azure-experience-in-csp#/).</span></span>

________________
## <a name="partner-center-software-license-key-and-download-fulfillment"></a><a name="4"></a><span data-ttu-id="a1e7d-520">Cumprimento de chave de licença e download de software do Partner Center</span><span class="sxs-lookup"><span data-stu-id="a1e7d-520">Partner Center software license key and download fulfillment</span></span>

### <a name="categories"></a><span data-ttu-id="a1e7d-521">Categorias</span><span class="sxs-lookup"><span data-stu-id="a1e7d-521">Categories</span></span>

- <span data-ttu-id="a1e7d-522">Data: 04/03/2021</span><span class="sxs-lookup"><span data-stu-id="a1e7d-522">Date: 2021-03-04</span></span>
- <span data-ttu-id="a1e7d-523">Funcionalidades</span><span class="sxs-lookup"><span data-stu-id="a1e7d-523">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="a1e7d-524">Resumo</span><span class="sxs-lookup"><span data-stu-id="a1e7d-524">Summary</span></span>

<span data-ttu-id="a1e7d-525">A capacidade de cumprimento de chave de licença e download de software do Partner Center foi restabelecida.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-525">The Partner Center software download and license key fulfillment capability has been reinstated.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a1e7d-526">Público-alvo afetado</span><span class="sxs-lookup"><span data-stu-id="a1e7d-526">Impacted audience</span></span>

<span data-ttu-id="a1e7d-527">Todos os parceiros CSP (Provedor de Soluções na Nuvem) que fazem a transação de pedidos de software de assinatura de servidor e perpétuas por meio do Partner Center</span><span class="sxs-lookup"><span data-stu-id="a1e7d-527">All Cloud Solution Provider (CSP) partners transacting perpetual and server subscription software orders through Partner Center</span></span>

### <a name="details"></a><span data-ttu-id="a1e7d-528">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a1e7d-528">Details</span></span>

<span data-ttu-id="a1e7d-529">Em resposta aos comentários dos parceiros, estamos restabelecendo a capacidade de cumprimento do Partner Center para obter software e chaves de licença para pedidos de software de assinatura de servidor e perpétuas.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-529">In response to partner feedback, we’re reinstating the Partner Center fulfillment capability to obtain software and license keys for perpetual and server subscription software orders.</span></span> <span data-ttu-id="a1e7d-530">Ela será restaurada para o estado anterior antes de ser removida em 19 de janeiro de 2021.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-530">It will be restored to its previous state prior to being removed on January 19, 2021.</span></span> <span data-ttu-id="a1e7d-531">Confira o [comunicado](2020-september.md#17).</span><span class="sxs-lookup"><span data-stu-id="a1e7d-531">(See the [announcement](2020-september.md#17).)</span></span>

<span data-ttu-id="a1e7d-532">Observe que as chaves de licença de software e os links de download são ativos de propriedade intelectual valiosos e muito procurados.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-532">Note that software license keys and download links are valuable and highly sought-after intellectual property assets.</span></span> <span data-ttu-id="a1e7d-533">Caso sejam vazados, poderão esgotar rapidamente os limites de ativação e causar uma experiência negativa para clientes e parceiros.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-533">If leaked, they can quickly be depleted of their activation limits and cause a negative customer and partner experience.</span></span>

### <a name="next-steps"></a><span data-ttu-id="a1e7d-534">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="a1e7d-534">Next steps</span></span>

<span data-ttu-id="a1e7d-535">Examine os seguintes recursos para obter instruções de uso e diretrizes importantes sobre a distribuição de chaves de software:</span><span class="sxs-lookup"><span data-stu-id="a1e7d-535">Review the following resources for usage instructions and important guidance on software key distribution:</span></span>

- [<span data-ttu-id="a1e7d-536">Vender software local por meio do programa CSP</span><span class="sxs-lookup"><span data-stu-id="a1e7d-536">Sell on-premises software through the CSP program</span></span>](../csp-on-premise-software.md)
- <span data-ttu-id="a1e7d-537">[Novo guia de operações de comércio do Partner Center](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (Confira a seção **Diretrizes sobre a distribuição de chaves de software**.)</span><span class="sxs-lookup"><span data-stu-id="a1e7d-537">[Partner Center New Commerce Operations Guide](https://partner.microsoft.com/resources/detail/partner-center-new-commerce-operations-guide-pdf) (See the **Guidance on Software Key Distribution** section.)</span></span>

### <a name="questions"></a><span data-ttu-id="a1e7d-538">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="a1e7d-538">Questions?</span></span>

<span data-ttu-id="a1e7d-539">Se tiver mais dúvidas sobre esse aviso, confira as comunidades relevantes no Yammer.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-539">If you have any further questions about this notice, check your relevant Yammer communities.</span></span>

________________
## <a name="migrate-your-deals-from-partner-sales-connect-psc-to-partner-center"></a><a name="3"></a><span data-ttu-id="a1e7d-540">Migre seus acordos do PSC (Partner Sales Connect) para o Partner Center</span><span class="sxs-lookup"><span data-stu-id="a1e7d-540">Migrate your deals from Partner Sales Connect (PSC) to Partner Center</span></span>

### <a name="categories"></a><span data-ttu-id="a1e7d-541">Categorias</span><span class="sxs-lookup"><span data-stu-id="a1e7d-541">Categories</span></span>

- <span data-ttu-id="a1e7d-542">Data: 04/03/2021</span><span class="sxs-lookup"><span data-stu-id="a1e7d-542">Date: 2021-03-04</span></span>
- <span data-ttu-id="a1e7d-543">Funcionalidades</span><span class="sxs-lookup"><span data-stu-id="a1e7d-543">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="a1e7d-544">Resumo</span><span class="sxs-lookup"><span data-stu-id="a1e7d-544">Summary</span></span>

<span data-ttu-id="a1e7d-545">O PSC (Partner Sales Connect) fará a migração para acesso somente leitura a partir de 31 de março de 2021. Portanto, incentivamos você a começar a migrar seus acordos do PSC para o Partner Center.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-545">Partner Sales Connect (PSC) will move to read-only access starting March 31, 2021, so we urge you to begin migrating your deals from PSC to Partner Center.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a1e7d-546">Público-alvo afetado</span><span class="sxs-lookup"><span data-stu-id="a1e7d-546">Impacted audience</span></span>

<span data-ttu-id="a1e7d-547">Parceiros com acordos no PSC</span><span class="sxs-lookup"><span data-stu-id="a1e7d-547">Partners with deals in PSC</span></span>

### <a name="details"></a><span data-ttu-id="a1e7d-548">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a1e7d-548">Details</span></span>

<span data-ttu-id="a1e7d-549">Como parte do nosso compromisso com o crescimento compartilhado, a **venda conjunta com a Microsoft** é o caminho para você **ser descoberto, oferecer sua experiência e expandir a superfície do cliente** para que ele tenha resultados positivos.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-549">As part of our shared commitment to growth, **co-sell with Microsoft** is the path for you to **be discovered, deliver your expertise, and expand your customer footprint** for positive customer outcomes.</span></span> <span data-ttu-id="a1e7d-550">Com uma negociação média **3,5 vezes mais rápida** do que o normal, o gerenciamento de sua experiência de venda conjunta no Partner Center permite que você venda nos canais de clientes diretos, parceiros e vendedores da Microsoft e administre seu pipeline de referência em um lugar só.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-550">With an average deal that’s **3.5 times faster** than normal, managing your co-sell experience in Partner Center allows you to sell across the direct customer, partner, and Microsoft seller channels, and manage your entire referral pipeline in one location.</span></span>

<span data-ttu-id="a1e7d-551">O **PSC** fará a migração para o **acesso somente leitura** a partir de **31 de março de 2021**. Portanto, incentivamos você a começar a fazer a migração para o Partner Center e acessar estes aprimoramentos de funcionalidade:</span><span class="sxs-lookup"><span data-stu-id="a1e7d-551">**PSC** will move to **read-only access** starting **March 31, 2021**, so we urge you to start your move to Partner Center and access these capability improvements:</span></span> 

- <span data-ttu-id="a1e7d-552">**Encaminhamento mais preciso** dos acordos que você compartilha com a Microsoft para o vendedor certo, com base no tipo de assistência de que você precisa.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-552">**More accurate routing** of the deals that you share with Microsoft to the right seller, based on the type of assistance you need.</span></span>
- <span data-ttu-id="a1e7d-553">**Validação da qualificação de acordos antecipados** para soluções qualificadas para incentivos e para atender aos critérios do programa ISV Connect, simplificando o processo de aprovação e o atestado de POE (comprovante de execução) final.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-553">**Upfront deal eligibility validation** for incentive-eligible solutions and to meet the ISV Connect program criteria, simplifying the approval process and final proof of execution (POE) attestation.</span></span>
- <span data-ttu-id="a1e7d-554">**Experiência de usuário perfeita** para gerenciar todas as suas oportunidades de venda conjunta e leads qualificados por vendas em um lugar só.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-554">**Seamless user experience** to manage all your co-sell opportunities and sales qualified leads in one place.</span></span>

<span data-ttu-id="a1e7d-555">Também adicionamos recentemente novos recursos ao Partner Center para ajudar você na sua migração:</span><span class="sxs-lookup"><span data-stu-id="a1e7d-555">We’ve also recently added new features in Partner Center to assist in your move:</span></span>

- [<span data-ttu-id="a1e7d-556">Operações em massa para oportunidades de venda conjunta</span><span class="sxs-lookup"><span data-stu-id="a1e7d-556">Bulk operations for co-sell opportunities</span></span>](../bulk-operations.md)
- <span data-ttu-id="a1e7d-557">[Recurso de migração de acordos](../psc-to-pc.md) (Confira a seção **Migração de acordos no PSC**.)</span><span class="sxs-lookup"><span data-stu-id="a1e7d-557">[Deal migration feature](../psc-to-pc.md) (See the **PSC Deals migration** section.)</span></span>

<span data-ttu-id="a1e7d-558">Usando a experiência de venda conjunta no Partner Center, suas equipes de vendas terão mais tempo para se concentrar em fomentar leads e oportunidades, fechar acordos e criar relações duradouras com o cliente.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-558">Using the co-sell experience in Partner Center, your sales teams will have more time to focus on nurturing leads and opportunities, closing deals, and creating lasting customer relationships.</span></span>

### <a name="next-steps"></a><span data-ttu-id="a1e7d-559">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="a1e7d-559">Next steps</span></span>

<span data-ttu-id="a1e7d-560">Use o [guia de transição](../psc-to-pc.md) do Partner Center para explicar as etapas para migrar seus acordos do PSC para o Partner Center.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-560">Use the Partner Center [transition guide](../psc-to-pc.md) to walk you through the steps to migrate your deals from PSC to Partner Center.</span></span>

### <a name="questions"></a><span data-ttu-id="a1e7d-561">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="a1e7d-561">Questions?</span></span>

<span data-ttu-id="a1e7d-562">Para outras perguntas, entre em contato com o [Suporte](https://partner.microsoft.com/support/?stage=1).</span><span class="sxs-lookup"><span data-stu-id="a1e7d-562">For any further questions, contact [Support](https://partner.microsoft.com/support/?stage=1).</span></span>

________________
## <a name="new-microsoft-dynamics-365-products-and-offers-available-on-april-1-2021"></a><a name="2"></a><span data-ttu-id="a1e7d-563">Novos produtos e ofertas do Microsoft Dynamics 365 disponíveis em 1º de abril de 2021</span><span class="sxs-lookup"><span data-stu-id="a1e7d-563">New Microsoft Dynamics 365 products and offers available on April 1, 2021</span></span>

### <a name="categories"></a><span data-ttu-id="a1e7d-564">Categorias</span><span class="sxs-lookup"><span data-stu-id="a1e7d-564">Categories</span></span>

- <span data-ttu-id="a1e7d-565">Data: 04/03/2021</span><span class="sxs-lookup"><span data-stu-id="a1e7d-565">Date: 2021-03-04</span></span>
- <span data-ttu-id="a1e7d-566">Funcionalidades</span><span class="sxs-lookup"><span data-stu-id="a1e7d-566">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="a1e7d-567">Resumo</span><span class="sxs-lookup"><span data-stu-id="a1e7d-567">Summary</span></span>

<span data-ttu-id="a1e7d-568">Em 1º de abril de 2021, a Microsoft iniciará vários novos produtos e ofertas para o programa CSP (Provedor de Soluções na Nuvem).</span><span class="sxs-lookup"><span data-stu-id="a1e7d-568">On April 1, 2021, Microsoft will be launching several new products and offers for the Cloud Solution Provider (CSP) program.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a1e7d-569">Público-alvo afetado</span><span class="sxs-lookup"><span data-stu-id="a1e7d-569">Impacted audience</span></span>

<span data-ttu-id="a1e7d-570">Todos os parceiros que fazem transações pelo programa CSP (Provedor de Soluções na Nuvem)</span><span class="sxs-lookup"><span data-stu-id="a1e7d-570">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="a1e7d-571">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a1e7d-571">Details</span></span>

<span data-ttu-id="a1e7d-572">Em 1º de abril de 2021, a Microsoft iniciará os seguintes novos produtos e oferecerá:</span><span class="sxs-lookup"><span data-stu-id="a1e7d-572">On April 1, 2021, Microsoft will be launching the following new products and offers:</span></span>

- <span data-ttu-id="a1e7d-573">Power BI Premium por Usuário</span><span class="sxs-lookup"><span data-stu-id="a1e7d-573">Power BI Premium Per User</span></span>
- <span data-ttu-id="a1e7d-574">Expansão geográfica e de segmento da USL do Marketing e Customer Voice</span><span class="sxs-lookup"><span data-stu-id="a1e7d-574">Customer Voice and Marketing USL geo and segment expansion</span></span>

<span data-ttu-id="a1e7d-575">**Power BI Premium por Usuário**</span><span class="sxs-lookup"><span data-stu-id="a1e7d-575">**Power BI Premium Per User**</span></span>

<span data-ttu-id="a1e7d-576">A Microsoft apresentará as primeiras ofertas do Power BI Premium por usuário.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-576">Microsoft will introduce the first per-user Power BI Premium offers.</span></span> <span data-ttu-id="a1e7d-577">No momento, o Power BI Premium é vendido apenas em um constructo de capacidade.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-577">Power BI Premium is currently sold only in a capacity construct.</span></span> <span data-ttu-id="a1e7d-578">O Power BI Premium por usuário fornece acesso a funcionalidades de BI (business intelligence empresarial) e análise.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-578">Power BI Premium Per User provides access to enterprise business intelligence (BI) and analytics capabilities.</span></span> <span data-ttu-id="a1e7d-579">O licenciamento de estação individual flexível dele atende a empresas de pequeno e médio porte.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-579">Its flexible individual seat licensing caters to small and medium-sized businesses.</span></span>

<span data-ttu-id="a1e7d-580">Examine os [detalhes de versão do Power BI](/power-platform-release-plan/2020wave2/power-bi/planned-features) para saber mais sobre esta oferta.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-580">Review the [Power BI release details](/power-platform-release-plan/2020wave2/power-bi/planned-features) to learn more about this offer.</span></span>


<span data-ttu-id="a1e7d-581">**Detalhes da oferta**</span><span class="sxs-lookup"><span data-stu-id="a1e7d-581">**Offer details**</span></span>

<span data-ttu-id="a1e7d-582">Observe que o nome da oferta difere ligeiramente da visualização da lista de preços.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-582">Note that the offer name differs slightly from the price list preview.</span></span>

| <span data-ttu-id="a1e7d-583">Nome da oferta</span><span class="sxs-lookup"><span data-stu-id="a1e7d-583">Offer name</span></span> | <span data-ttu-id="a1e7d-584">ID da oferta</span><span class="sxs-lookup"><span data-stu-id="a1e7d-584">Offer ID</span></span> |
| ------ |----------- |
| <span data-ttu-id="a1e7d-585">Power BI Premium por Usuário</span><span class="sxs-lookup"><span data-stu-id="a1e7d-585">Power BI Premium Per User</span></span> | <span data-ttu-id="a1e7d-586">9c810018-9356-4903-95ab-eeb956289290</span><span class="sxs-lookup"><span data-stu-id="a1e7d-586">9c810018-9356-4903-95ab-eeb956289290</span></span> | 
| <span data-ttu-id="a1e7d-587">Power BI Premium por Usuário para Docentes</span><span class="sxs-lookup"><span data-stu-id="a1e7d-587">Power BI Premium Per User for Faculty</span></span> | <span data-ttu-id="a1e7d-588">3affc44f-f372-4ad5-8657-aadd9574fce0</span><span class="sxs-lookup"><span data-stu-id="a1e7d-588">3affc44f-f372-4ad5-8657-aadd9574fce0</span></span> | 
| <span data-ttu-id="a1e7d-589">Power BI Premium por Usuário para Estudantes</span><span class="sxs-lookup"><span data-stu-id="a1e7d-589">Power BI Premium Per User for Students</span></span> | <span data-ttu-id="a1e7d-590">657eea87-d0b0-4c89-8c8e-9b04395bd940</span><span class="sxs-lookup"><span data-stu-id="a1e7d-590">657eea87-d0b0-4c89-8c8e-9b04395bd940</span></span> | 
| <span data-ttu-id="a1e7d-591">Power BI Premium por Usuário (preço de equipe sem fins lucrativos)</span><span class="sxs-lookup"><span data-stu-id="a1e7d-591">Power BI Premium Per User (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="a1e7d-592">7a0a856c-059f-45dd-9d26-ae27992e706a</span><span class="sxs-lookup"><span data-stu-id="a1e7d-592">7a0a856c-059f-45dd-9d26-ae27992e706a</span></span> | 
| <span data-ttu-id="a1e7d-593">Complemento do Power BI Premium por Usuário</span><span class="sxs-lookup"><span data-stu-id="a1e7d-593">Power BI Premium Per User Add-On</span></span> | <span data-ttu-id="a1e7d-594">244ff87e-5925-44a0-bf31-cea189719b58</span><span class="sxs-lookup"><span data-stu-id="a1e7d-594">244ff87e-5925-44a0-bf31-cea189719b58</span></span> | 
| <span data-ttu-id="a1e7d-595">Complemento do Power BI Premium por Usuário para Docentes</span><span class="sxs-lookup"><span data-stu-id="a1e7d-595">Power BI Premium Per User Add-On for Faculty</span></span> | <span data-ttu-id="a1e7d-596">5da849bd-b8f7-4340-b4f4-3a9eaeb8987e</span><span class="sxs-lookup"><span data-stu-id="a1e7d-596">5da849bd-b8f7-4340-b4f4-3a9eaeb8987e</span></span> | 
| <span data-ttu-id="a1e7d-597">Complemento do Power BI Premium por Usuário para Estudantes</span><span class="sxs-lookup"><span data-stu-id="a1e7d-597">Power BI Premium Per User Add-On for Students</span></span> | <span data-ttu-id="a1e7d-598">cf62d70d-5af5-422a-bda8-97936402ac8e</span><span class="sxs-lookup"><span data-stu-id="a1e7d-598">cf62d70d-5af5-422a-bda8-97936402ac8e</span></span> | 
| <span data-ttu-id="a1e7d-599">Complemento do Power BI Premium por Usuário (preço de equipe sem fins lucrativos)</span><span class="sxs-lookup"><span data-stu-id="a1e7d-599">Power BI Premium Per User Add-On (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="a1e7d-600">31c03289-47ab-4ab0-8df1-03742c127ac6</span><span class="sxs-lookup"><span data-stu-id="a1e7d-600">31c03289-47ab-4ab0-8df1-03742c127ac6</span></span> | 

<span data-ttu-id="a1e7d-601">**Expansão geográfica e de segmento da USL do Marketing e Customer Voice**</span><span class="sxs-lookup"><span data-stu-id="a1e7d-601">**Customer Voice and Marketing USL geo and segment expansion**</span></span>

<span data-ttu-id="a1e7d-602">Como um acompanhamento para o lançamento de dezembro de 2020, as ofertas USL do Dynamics 365 Customer Voice e Marketing foram alteradas para adicionar novos países e mais SKUs educacionais e sem fins lucrativos.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-602">As a follow-up to the December 2020 launch, Dynamics 365 Customer Voice and Marketing USL offers have been changed to add new countries and more nonprofit and educational SKUs.</span></span>

| <span data-ttu-id="a1e7d-603">Nome da oferta</span><span class="sxs-lookup"><span data-stu-id="a1e7d-603">Offer name</span></span> | <span data-ttu-id="a1e7d-604">ID da oferta</span><span class="sxs-lookup"><span data-stu-id="a1e7d-604">Offer ID</span></span> |
| ------ |----------- |
| <span data-ttu-id="a1e7d-605">USL do Dynamics 365 Customer Voice (preço de equipe sem fins lucrativos)</span><span class="sxs-lookup"><span data-stu-id="a1e7d-605">Dynamics 365 Customer Voice USL (Nonprofit Staff Pricing)</span></span> | <span data-ttu-id="a1e7d-606">7a8642a5-481e-4906-a642-b56dbeeb62a0</span><span class="sxs-lookup"><span data-stu-id="a1e7d-606">7a8642a5-481e-4906-a642-b56dbeeb62a0</span></span> |
| <span data-ttu-id="a1e7d-607">USL do Dynamics 365 Customer Voice para Docentes</span><span class="sxs-lookup"><span data-stu-id="a1e7d-607">Dynamics 365 Customer Voice USL for Faculty</span></span> | <span data-ttu-id="a1e7d-608">85162d70-9676-4cf6-a4bc-a0d6672f2657</span><span class="sxs-lookup"><span data-stu-id="a1e7d-608">85162d70-9676-4cf6-a4bc-a0d6672f2657</span></span> |

<span data-ttu-id="a1e7d-609">Acesse as seguintes páginas para saber mais sobre essas ofertas:</span><span class="sxs-lookup"><span data-stu-id="a1e7d-609">Visit the following pages to find out more about these offers:</span></span>

- [<span data-ttu-id="a1e7d-610">Página inicial do Dynamics 365 Customer Service Voice</span><span class="sxs-lookup"><span data-stu-id="a1e7d-610">Dynamics 365 Customer Service Voice home page</span></span>](https://dynamics.microsoft.com/customer-voice/overview/)
- [<span data-ttu-id="a1e7d-611">Página inicial do Dynamics 365 Marketing</span><span class="sxs-lookup"><span data-stu-id="a1e7d-611">Dynamics 365 Marketing home page</span></span>](https://dynamics.microsoft.com/customer-voice/overview/)

### <a name="next-steps"></a><span data-ttu-id="a1e7d-612">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="a1e7d-612">Next steps</span></span>

<span data-ttu-id="a1e7d-613">Examine os recursos sobre esse tópico e compartilhe essas informações com os stakeholders apropriados da organização.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-613">Review the resources on this topic, and share this information with the appropriate stakeholders in your organization.</span></span>  

### <a name="questions"></a><span data-ttu-id="a1e7d-614">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="a1e7d-614">Questions?</span></span>

<span data-ttu-id="a1e7d-615">Caso tenha dúvidas sobre essas ofertas, confira as comunidades relevantes no Yammer.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-615">For any questions about these offers, check your relevant Yammer communities.</span></span> 

________________
## <a name="microsoft-universal-print-now-available-in-some-suites"></a><a name="1"></a> <span data-ttu-id="a1e7d-616">A Impressão Universal da Microsoft já está disponível em alguns pacotes</span><span class="sxs-lookup"><span data-stu-id="a1e7d-616">Microsoft Universal Print now available in some suites</span></span>

### <a name="categories"></a><span data-ttu-id="a1e7d-617">Categorias</span><span class="sxs-lookup"><span data-stu-id="a1e7d-617">Categories</span></span>

- <span data-ttu-id="a1e7d-618">Data: 03/03/2021</span><span class="sxs-lookup"><span data-stu-id="a1e7d-618">Date: 2021-03-33</span></span>
- <span data-ttu-id="a1e7d-619">Funcionalidades</span><span class="sxs-lookup"><span data-stu-id="a1e7d-619">Capabilities</span></span>

### <a name="summary"></a><span data-ttu-id="a1e7d-620">Resumo</span><span class="sxs-lookup"><span data-stu-id="a1e7d-620">Summary</span></span>

<span data-ttu-id="a1e7d-621">A Impressão Universal da Microsoft está disponível para transações em pacotes do Microsoft 365 selecionados e como um complemento autônomo desde 1º de março de 2021.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-621">Microsoft Universal Print will be available to transact within select Microsoft 365 suites and as a standalone add-on from March 1, 2021.</span></span>

### <a name="impacted-audience"></a><span data-ttu-id="a1e7d-622">Público-alvo afetado</span><span class="sxs-lookup"><span data-stu-id="a1e7d-622">Impacted audience</span></span>

<span data-ttu-id="a1e7d-623">Todos os parceiros que fazem transações pelo programa CSP (Provedor de Soluções na Nuvem)</span><span class="sxs-lookup"><span data-stu-id="a1e7d-623">All partners transacting through the Cloud Solution Provider (CSP) program</span></span>

### <a name="details"></a><span data-ttu-id="a1e7d-624">Detalhes</span><span class="sxs-lookup"><span data-stu-id="a1e7d-624">Details</span></span>

<span data-ttu-id="a1e7d-625">A [Impressão Universal](https://aka.ms/universalprint) é um serviço de impressão da Microsoft 365 que acaba com a necessidade de servidores de impressão locais e permite que dispositivos Windows imprimam em impressoras registradas no Azure.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-625">[Universal Print](https://aka.ms/universalprint) is a Microsoft 365 print service that removes the need for on-premises print servers, and enables Windows devices to print to Azure-registered printers.</span></span> <span data-ttu-id="a1e7d-626">Ela está disponível para transações desde 1º de março de 2021.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-626">It will be available to transact from March 1, 2021.</span></span>

<span data-ttu-id="a1e7d-627">Os trabalhadores se beneficiam da impressão sem driver, da descoberta simplificada de impressoras baseada em local e de uma experiência de impressão intuitiva, com nenhuma curva de aprendizado.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-627">Workers benefit from driverless printing, streamlined location-based printer discovery, and an intuitive printing experience with no learning curve.</span></span> <span data-ttu-id="a1e7d-628">Os dispositivos que ingressaram no Azure AD (Active Directory) usam credenciais do Azure AD existentes para imprimir com segurança.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-628">Devices that are joined to Azure Active Directory (Azure AD) use existing Azure AD credentials to print securely.</span></span> <span data-ttu-id="a1e7d-629">Os administradores gerenciam a impressão usando o portal do Azure e podem facilmente conectar impressoras com suporte nativo para Impressão Universal.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-629">Administrators manage printing by using the Azure portal, and can easily connect printers with native support for Universal Print.</span></span> <span data-ttu-id="a1e7d-630">A Impressão Universal pode ser implantada com impressoras não compatíveis usando o software do conector da Impressão Universal.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-630">Universal Print can be deployed with non-compatible printers by using Universal Print connector software.</span></span>

<span data-ttu-id="a1e7d-631">A Impressão Universal será acrescida ao Windows E3, A3, E5 e A5 e ao Microsoft 365 BP, F3, E3, A3, E5 e A5 no lançamento.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-631">Universal Print will be backfilled at launch to Windows E3, A3, E5, and A5, and Microsoft 365 BP, F3, E3, A3, E5, and A5.</span></span>  

<span data-ttu-id="a1e7d-632">**Detalhes da oferta**</span><span class="sxs-lookup"><span data-stu-id="a1e7d-632">**Offer details**</span></span>

<span data-ttu-id="a1e7d-633">Observe que o nome da oferta difere ligeiramente da visualização da lista de preços.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-633">Note that the offer name differs slightly from the price list preview.</span></span>

| <span data-ttu-id="a1e7d-634">Nome da oferta</span><span class="sxs-lookup"><span data-stu-id="a1e7d-634">Offer name</span></span> | <span data-ttu-id="a1e7d-635">ID da oferta</span><span class="sxs-lookup"><span data-stu-id="a1e7d-635">Offer ID</span></span> | <span data-ttu-id="a1e7d-636">ID do material</span><span class="sxs-lookup"><span data-stu-id="a1e7d-636">Material ID</span></span> |
| ------ |----------- |----------- |  
| <span data-ttu-id="a1e7d-637">Complemento de volume da Impressão Universal (500 trabalhos) – Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="a1e7d-637">Universal Print volume add-on (500 jobs) - Microsoft 365</span></span>  | <span data-ttu-id="a1e7d-638">cb131356-45ee-4ae2-8537-873b706c8e75</span><span class="sxs-lookup"><span data-stu-id="a1e7d-638">cb131356-45ee-4ae2-8537-873b706c8e75</span></span>     | <span data-ttu-id="a1e7d-639">9BI-00004</span><span class="sxs-lookup"><span data-stu-id="a1e7d-639">9BI-00004</span></span>   |
| <span data-ttu-id="a1e7d-640">Complemento de volume da Impressão Universal (500 trabalhos) para docentes – Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="a1e7d-640">Universal Print volume add-on (500 jobs) for faculty - Microsoft 365</span></span>   | <span data-ttu-id="a1e7d-641">477bee81-9872-43d6-91d3-c72390bfcf49</span><span class="sxs-lookup"><span data-stu-id="a1e7d-641">477bee81-9872-43d6-91d3-c72390bfcf49</span></span>   | <span data-ttu-id="a1e7d-642">9BK-00004</span><span class="sxs-lookup"><span data-stu-id="a1e7d-642">9BK-00004</span></span>   |
| <span data-ttu-id="a1e7d-643">Complemento de volume da Impressão Universal (500 trabalhos) – Windows</span><span class="sxs-lookup"><span data-stu-id="a1e7d-643">Universal Print volume add-on (500 jobs) - Windows</span></span>    | <span data-ttu-id="a1e7d-644">d3ddc493-5741-4e0d-a02d-07edbb0bb72e</span><span class="sxs-lookup"><span data-stu-id="a1e7d-644">d3ddc493-5741-4e0d-a02d-07edbb0bb72e</span></span>   | <span data-ttu-id="a1e7d-645">9BI-00002</span><span class="sxs-lookup"><span data-stu-id="a1e7d-645">9BI-00002</span></span>   |
| <span data-ttu-id="a1e7d-646">Complemento de volume da Impressão Universal (500 trabalhos) para docentes – Windows</span><span class="sxs-lookup"><span data-stu-id="a1e7d-646">Universal Print volume add-on (500 jobs) for faculty - Windows</span></span>   |  <span data-ttu-id="a1e7d-647">d0862f05-80f5-4fd4-8432-fe72dd893cc7</span><span class="sxs-lookup"><span data-stu-id="a1e7d-647">d0862f05-80f5-4fd4-8432-fe72dd893cc7</span></span>  | <span data-ttu-id="a1e7d-648">9BK-00002</span><span class="sxs-lookup"><span data-stu-id="a1e7d-648">9BK-00002</span></span>   |

### <a name="next-steps"></a><span data-ttu-id="a1e7d-649">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="a1e7d-649">Next steps</span></span>

<span data-ttu-id="a1e7d-650">Familiarize-se com a lista de preços e a [visão geral da Impressão Universal](/universal-print/fundamentals/universal-print-whatis).</span><span class="sxs-lookup"><span data-stu-id="a1e7d-650">Familiarize yourself with the price list and the [Universal Print overview](/universal-print/fundamentals/universal-print-whatis).</span></span> <span data-ttu-id="a1e7d-651">Compartilhe essas informações com todos os contatos adequados na sua organização.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-651">Share this information with all appropriate contacts in your organization.</span></span>

### <a name="questions"></a><span data-ttu-id="a1e7d-652">Perguntas?</span><span class="sxs-lookup"><span data-stu-id="a1e7d-652">Questions?</span></span>

<span data-ttu-id="a1e7d-653">Caso tenha dúvidas sobre essas ofertas, confira as comunidades relevantes no Yammer.</span><span class="sxs-lookup"><span data-stu-id="a1e7d-653">For any questions about these offers, check your relevant Yammer communities.</span></span>
