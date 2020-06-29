---
title: Principal de serviço do Azure AD
ms.topic: article
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Descubra como adicionar uma entidade de serviço ao seu inquilino do Azure AD. Fazer isso significa adicionar um aplicativo do Azure AD (principal de serviço) no Partner Center.
author: LauraBrenner
ms.author: labrenne
Keywords: Azure, plano do Azure, entidade de serviço, aplicativo do Azure AD
robots: ''
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: d37fe2134d02063819abeb89e2f1b6a63e0ba505
ms.sourcegitcommit: ecc5472c986e67525dbfcc6fc328c991d6db77ba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2020
ms.locfileid: "84679383"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="82bf9-105">Adicionar um aplicativo do Azure AD (entidade de serviço) no Partner Center</span><span class="sxs-lookup"><span data-stu-id="82bf9-105">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="82bf9-106">No programa Marketplace Comercial no Partner Center agora é possível adicionar um aplicativo do Azure AD (entidade de serviço) como um usuário em sua conta do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="82bf9-106">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="82bf9-107">(Você conseguiu fazer isso anteriormente em sua conta do Cloud Partner Portal ou CPP.</span><span class="sxs-lookup"><span data-stu-id="82bf9-107">(You were able to do so previously in your Cloud Partner Portal, or CPP, account.</span></span> <span data-ttu-id="82bf9-108">Agora que você migrou para o Partner Center, a conta do CPP é somente leitura.)</span><span class="sxs-lookup"><span data-stu-id="82bf9-108">Now that you have migrated to Partner Center, the CPP account is read-only.)</span></span>
 
>[!Note] 
><span data-ttu-id="82bf9-109">A entidade de serviço equivale ao aplicativo do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="82bf9-109">Service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="82bf9-110">Adicionar um aplicativo do Azure AD (entidade de serviço)</span><span class="sxs-lookup"><span data-stu-id="82bf9-110">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="82bf9-111">No painel do Partner Center, selecione **Configurações** e, em seguida, selecione **Configurações do desenvolvedor**.</span><span class="sxs-lookup"><span data-stu-id="82bf9-111">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="82bf9-112">Selecione **Usuários** e, em seguida, selecione **Adicionar Aplicativos do Azure AD**.</span><span class="sxs-lookup"><span data-stu-id="82bf9-112">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="82bf9-113">Crie um aplicativo do Azure AD ou selecione um existente.</span><span class="sxs-lookup"><span data-stu-id="82bf9-113">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="82bf9-114">Se você criar um aplicativo do Azure AD, inclua as seguintes informações:</span><span class="sxs-lookup"><span data-stu-id="82bf9-114">If you create a new Azure AD Application, include the following information:</span></span>  

   - <span data-ttu-id="82bf9-115">**URL de resposta**: A URL em que os usuários podem entrar para usar seu aplicativo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="82bf9-115">**Reply URL**: The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="82bf9-116">**URI da ID do aplicativo**: Um identificador lógico do aplicativo Azure AD que é apresentado quando ele envia uma solicitação de logon único para o Azure AD.</span><span class="sxs-lookup"><span data-stu-id="82bf9-116">**App ID URI**: A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="82bf9-117">**Funções de segurança**: As funções de **Gerente** (equivalente à função de 'Proprietário' no CPP) e de **Desenvolvedor** (equivalente à função 'Colaborador' no CPP) se aplicam ao programa Marketplace Comercial no Partner Center e podem ser associadas a este aplicativo do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="82bf9-117">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  
