---
title: Principal de serviço do Azure AD
ms.topic: article
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Descubra como adicionar uma entidade de serviço ao seu inquilino do Azure AD. Fazer isso significa adicionar um aplicativo do Azure AD (principal de serviço) no Partner Center.
author: dhirajgandhi
ms.author: dhgandhi
ms.localizationpriority: High
ms.custom: SEOMAY.20
ms.openlocfilehash: 7d75c5c7311feaa3ca53139f2abf2702035b1069
ms.sourcegitcommit: 2e206627323ff175c0e0d10646cdba80e9881891
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/29/2020
ms.locfileid: "87365752"
---
# <a name="add-an-azure-ad-application-service-principal-in-partner-center"></a><span data-ttu-id="e044d-104">Adicionar um aplicativo do Azure AD (entidade de serviço) no Partner Center</span><span class="sxs-lookup"><span data-stu-id="e044d-104">Add an Azure AD application (service principal) in Partner Center</span></span>

<span data-ttu-id="e044d-105">**Aplica-se a**</span><span class="sxs-lookup"><span data-stu-id="e044d-105">**Applies to**</span></span>

- <span data-ttu-id="e044d-106">Partner Center</span><span class="sxs-lookup"><span data-stu-id="e044d-106">Partner Center</span></span>

<span data-ttu-id="e044d-107">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="e044d-107">**Appropriate roles**</span></span>

- <span data-ttu-id="e044d-108">Administrador global</span><span class="sxs-lookup"><span data-stu-id="e044d-108">Global admin</span></span>

<span data-ttu-id="e044d-109">No programa Marketplace Comercial no Partner Center agora é possível adicionar um aplicativo do Azure AD (entidade de serviço) como um usuário em sua conta do Partner Center.</span><span class="sxs-lookup"><span data-stu-id="e044d-109">In the Commercial Marketplace program in Partner Center, you are now able to add an Azure AD application (service principal) as a user in your Partner Center account.</span></span> <span data-ttu-id="e044d-110">(Você conseguiu fazer isso anteriormente em sua conta do Cloud Partner Portal ou CPP.</span><span class="sxs-lookup"><span data-stu-id="e044d-110">(You were able to do so previously in your Cloud Partner Portal, or CPP, account.</span></span> <span data-ttu-id="e044d-111">Agora que você migrou para o Partner Center, a conta do CPP é somente leitura.)</span><span class="sxs-lookup"><span data-stu-id="e044d-111">Now that you have migrated to Partner Center, the CPP account is read-only.)</span></span>
 
>[!Note] 
><span data-ttu-id="e044d-112">A entidade de serviço equivale ao aplicativo do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e044d-112">Service principal is synonymous with Azure AD application.</span></span>

## <a name="add-an-azure-ad-application-service-principal"></a><span data-ttu-id="e044d-113">Adicionar um aplicativo do Azure AD (entidade de serviço)</span><span class="sxs-lookup"><span data-stu-id="e044d-113">Add an Azure AD application (service principal)</span></span>

1. <span data-ttu-id="e044d-114">No painel do Partner Center, selecione **Configurações** e, em seguida, selecione **Configurações do desenvolvedor**.</span><span class="sxs-lookup"><span data-stu-id="e044d-114">From the Partner Center dashboard, select **Settings** and then select **Developer settings**.</span></span>

2. <span data-ttu-id="e044d-115">Selecione **Usuários** e, em seguida, selecione **Adicionar Aplicativos do Azure AD**.</span><span class="sxs-lookup"><span data-stu-id="e044d-115">Select **Users** and then select **Add Azure AD Applications**.</span></span>

3. <span data-ttu-id="e044d-116">Crie um aplicativo do Azure AD ou selecione um existente.</span><span class="sxs-lookup"><span data-stu-id="e044d-116">Select an existing Azure AD application or create a new one.</span></span>

4. <span data-ttu-id="e044d-117">Se você criar um aplicativo do Azure AD, inclua as seguintes informações:</span><span class="sxs-lookup"><span data-stu-id="e044d-117">If you create a new Azure AD Application, include the following information:</span></span>  

   - <span data-ttu-id="e044d-118">**URL de resposta**: A URL em que os usuários podem entrar para usar seu aplicativo Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e044d-118">**Reply URL**: The URL where users can sign in to use your Azure AD application.</span></span>

   - <span data-ttu-id="e044d-119">**URI da ID do aplicativo**: Um identificador lógico do aplicativo Azure AD que é apresentado quando ele envia uma solicitação de logon único para o Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e044d-119">**App ID URI**: A logical identifier for the Azure AD application that is presented when it sends a single sign-on request to Azure AD.</span></span>

   - <span data-ttu-id="e044d-120">**Funções de segurança**: As funções de **Gerente** (equivalente à função de 'Proprietário' no CPP) e de **Desenvolvedor** (equivalente à função 'Colaborador' no CPP) se aplicam ao programa Marketplace Comercial no Partner Center e podem ser associadas a este aplicativo do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e044d-120">**Security roles**: The roles **Manager** (the same as  ‘Owner’ role in CPP) and **Developer** (the same as ‘Contributor’ role in CPP) apply to the Commercial Marketplace program in Partner Center, and they can be associated with this Azure AD Application.</span></span>  

## <a name="next-steps"></a><span data-ttu-id="e044d-121">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="e044d-121">Next steps</span></span>

- [<span data-ttu-id="e044d-122">Visão geral do marketplace comercial no Partner Center</span><span class="sxs-lookup"><span data-stu-id="e044d-122">Overview of the commercial marketplace in Partner Center</span></span>](csp-commercial-marketplace-overview.md)