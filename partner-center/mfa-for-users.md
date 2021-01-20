---
title: Configurar os usuários com a autenticação multifator
ms.topic: how-to
ms.date: 12/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-mpn
description: Saiba como fazer a configuração da MFA para seus funcionários
author: vijvala
ms.author: vijvala
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: f42c97be88a1a505f7e0ae9b8af0d4a9167d8447
ms.sourcegitcommit: 531151a5dbc999b8b7de478d72ea115e6d579ff1
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/13/2021
ms.locfileid: "98182368"
---
# <a name="set-up-your-users-with-multi-factor-authentication"></a><span data-ttu-id="a7062-103">Configurar os usuários com a autenticação multifator</span><span class="sxs-lookup"><span data-stu-id="a7062-103">Set up your users with multi-factor authentication</span></span>

<span data-ttu-id="a7062-104">**Funções apropriadas**</span><span class="sxs-lookup"><span data-stu-id="a7062-104">**Appropriate roles**</span></span>

- <span data-ttu-id="a7062-105">Administrador global</span><span class="sxs-lookup"><span data-stu-id="a7062-105">Global admin</span></span>

<span data-ttu-id="a7062-106">As maiores proteções de privacidade e segurança estão entre nossas principais prioridades.</span><span class="sxs-lookup"><span data-stu-id="a7062-106">Greater privacy safeguards and security are among our top priorities.</span></span> <span data-ttu-id="a7062-107">Sabemos que a melhor defesa é a prevenção e que somos tão fortes quanto nosso vínculo mais fraco.</span><span class="sxs-lookup"><span data-stu-id="a7062-107">We know that the best defense is prevention and that we are only as strong as our weakest link.</span></span> <span data-ttu-id="a7062-108">É por isso que precisamos de todos em nosso ecossistema, para agir e garantir que as proteções de segurança adequadas estejam em vigor.</span><span class="sxs-lookup"><span data-stu-id="a7062-108">That is why we need everyone in our ecosystem to act and ensure appropriate security protections are in place.</span></span> <span data-ttu-id="a7062-109">É altamente recomendável que todos os parceiros habilitem a MFA (autenticação multifator) para seus usuários em seus locatários parceiros.</span><span class="sxs-lookup"><span data-stu-id="a7062-109">We strongly recommend all partners enable multi-factor authentication (MFA) for their users in their partner tenant.</span></span> 

## <a name="add-multi-factor-authentication-for-your-users"></a><span data-ttu-id="a7062-110">Adicionar a autenticação multifator aos seus dispositivos</span><span class="sxs-lookup"><span data-stu-id="a7062-110">Add multi-factor authentication for your users</span></span>

<span data-ttu-id="a7062-111">Você precisará ser o administrador global da sua empresa para concluir esta tarefa.</span><span class="sxs-lookup"><span data-stu-id="a7062-111">You must be the global admin for your company to complete this task.</span></span>

<span data-ttu-id="a7062-112">É mais fácil habilitar a MFA para os usuários conforme você os adiciona ao seu locatário do Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a7062-112">It is easiest to enable MFA for your users as you add them to your Azure AD tenant.</span></span>

1. <span data-ttu-id="a7062-113">Entre no [portal do Azure](https://portal.azure.com) e acesse **Gerenciamento de usuários**.</span><span class="sxs-lookup"><span data-stu-id="a7062-113">Sign into the [Azure portal](https://portal.azure.com) and then go to **User management**.</span></span>
1. <span data-ttu-id="a7062-114">Selecione **Autenticação multifator**.</span><span class="sxs-lookup"><span data-stu-id="a7062-114">Select **Multi-factor authentication**.</span></span>
1. <span data-ttu-id="a7062-115">Escolha o usuário que deseja habilitar e selecione **Habilitar**.</span><span class="sxs-lookup"><span data-stu-id="a7062-115">Select the user you want to enable and then select **Enable**.</span></span>

<span data-ttu-id="a7062-116">Isso habilitará a MFA para o usuário.</span><span class="sxs-lookup"><span data-stu-id="a7062-116">This will enable MFA for this user.</span></span> <span data-ttu-id="a7062-117">A indicação Habilitado significa que o usuário precisará configurar a verificação da MFA quando ele se conectar pela primeira vez.</span><span class="sxs-lookup"><span data-stu-id="a7062-117">Enabled means that the user will be asked to set up their MFA verification when they sign in for the first time.</span></span> <span data-ttu-id="a7062-118">Depois disso, ao entrar, será solicitado que forneça um código enviado a eles por email ou mensagem de texto (dependendo da configuração efetuada).</span><span class="sxs-lookup"><span data-stu-id="a7062-118">Thereafter, at sign in, they will be asked to provide a code sent to them either through email or text message (depending on which they set up).</span></span>  

:::image type="content" source="images/MFA/securityverification.png" alt-text="Especificar a confirmação":::

>[!NOTE]
><span data-ttu-id="a7062-120">Você pode **Impor** aos usuários o uso da MFA usando as mesmas etapas acima e selecionando **Impor**.</span><span class="sxs-lookup"><span data-stu-id="a7062-120">You can **Enforce** your users to use MFA by using same steps as above and selecting **Enforce**.</span></span> <span data-ttu-id="a7062-121">Para saber mais, leia [Habilitar a Autenticação Multifator do Azure por usuário para proteger eventos de entrada](/azure/active-directory/authentication/howto-mfa-userstates).</span><span class="sxs-lookup"><span data-stu-id="a7062-121">To learn more, read [Enable per-user Azure Multi-Factor Authentication to secure sign-in events](/azure/active-directory/authentication/howto-mfa-userstates).</span></span> 

<span data-ttu-id="a7062-122">Todos os usuários começam com o estado **Desabilitado**.</span><span class="sxs-lookup"><span data-stu-id="a7062-122">All users start out **Disabled**.</span></span> <span data-ttu-id="a7062-123">Quando você registra os usuários na Autenticação Multifator do Azure por usuário, o estado deles passa a ser **Habilitado**.</span><span class="sxs-lookup"><span data-stu-id="a7062-123">When you enroll users in per-user Azure Multi-Factor Authentication, their state changes to **Enabled**.</span></span> <span data-ttu-id="a7062-124">Quando os usuários habilitados se conectam e concluem o processo de registro, o estado deles passa a ser **Imposto**.</span><span class="sxs-lookup"><span data-stu-id="a7062-124">When enabled users sign in and complete the registration process, their state changes to **Enforced**.</span></span> 

## <a name="next-steps"></a><span data-ttu-id="a7062-125">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="a7062-125">Next steps</span></span>

- [<span data-ttu-id="a7062-126">Atribuir funções e permissões a usuários</span><span class="sxs-lookup"><span data-stu-id="a7062-126">Assign roles and permissions to users</span></span>](permissions-overview.md)