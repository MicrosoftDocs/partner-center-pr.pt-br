---
title: Transferir a assinatura do Azure para outro parceiro
ms.topic: article
ms.date: 06/03/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como ajudar um cliente a alterar o parceiro do programa CSP associado às assinaturas do Azure do cliente.
author: dhirajgandhi
ms.author: dhgandhi
keywords: assinatura do Azure, mudar de parceiro, alterar parceiro, obter novo parceiro, outro parceiro
ms.custom: SEOMAY.20
ms.localizationpriority: medium
ms.openlocfilehash: 65278a9c597fb240f87c04f215a8195a0cff3e19
ms.sourcegitcommit: 36a60f672c1c3d6b63fd225d04c5ffa917694ae0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/03/2020
ms.locfileid: "85949099"
---
# <a name="learn-how-to-transfer-a-customers-azure-subscriptions-to-another-partner"></a>Saiba como transferir as assinaturas do Azure de um cliente para outro parceiro

**Aplica-se a**

- Partner Center do Microsoft Cloud for US Government
- Partner Center para Microsoft global Cloud
- Parceiros no programa CSP (Provedor de Soluções na Nuvem)

Este artigo descreve como um cliente pode mudar seus serviços de Microsoft Azure de um CSP (provedor de soluções de nuvem) para outro.

Para alternar os serviços ou assinaturas do Azure de um cliente para um parceiro diferente, siga estas etapas manuais. O parceiro e o cliente precisam concluir as etapas.

>[!Note]  
>Atualmente, somente provedores diretos ou indiretos podem transferir assinaturas.
>Você não pode alterar parceiros para assinaturas do provedor de soluções na nuvem associadas ao plano do Azure, Office 365, Enterprise Mobility Suite ou assinaturas do Microsoft Dynamics CRM.

**Mudar de parceiro para assinaturas do Azure**

1. Para transferir uma assinatura do Azure para um novo parceiro, o cliente deve iniciar o processo e entrar em contato com seu parceiro atual de registro por escrito.

   >[!Note]
   >É responsabilidade do parceiro atual criar o tíquete de serviço que inicia o processo de transferência. A Microsoft não pode interferir em nome do cliente ou do novo parceiro. O cliente deve planejar trabalhar em conjunto com o parceiro atual para que a transição ocorra sem problemas.

2. O parceiro para a assinatura precisa executar as seguintes tarefas:

   Crie um tíquete de serviço do Azure no Partner Center para solicitar uma transferência de assinatura:

   - No menu do centro de parceiros, selecione **clientes**, selecione o cliente na lista e, em seguida, selecione **Gerenciamento de serviços**. Na seção **Tíquetes de suporte**, selecione a lista suspensa **Novo tíquete** e escolha **Microsoft Azure**.

   - No [portal do Azure](https://portal.azure.com), selecione **nova solicitação de suporte**.

     Na Etapa 1, escolha **Gerenciar assinatura** como o tipo de problema, especifique a ID da assinatura que você deseja transferir e escolha **Provedor de Soluções na Nuvem** como o plano de suporte.

     Na etapa 2, selecione **C-impacto mínimo** e escolha **outras perguntas gerais** como o tipo de problema.

     Faça o download do [formulário de transferência de assinatura do CSP](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip).

3. O parceiro da assinatura: preencha o [formulário de transferência de assinatura de CSP](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip), assine-o e envie-o para o cliente. Para preencher o formulário, você precisará das informações a seguir:

   - Informações de contato do parceiro atual e a ID da Microsoft. No menu Partner Center, selecione **Configurações da conta** &gt; **Perfil de organização**, e use a **ID da Microsoft**, o **Nome da organização** e o **Endereço** listados lá.

   - ID Microsoft. do cliente. No menu Partner Center, selecione **Clientes**, em seguida, expanda a listagem de clientes para ver a **ID da Microsoft**.

   - A ID de assinatura a ser transferida. Na listagem de clientes expandida, selecione **Exibir Assinaturas**, em seguida, expanda a assinatura escolhida para ver a **ID de Assinatura**.

   >[!Note]
   >A transferência de uma assinatura resulta em duas IDs de assinaturas que você verá na página **Editar Assinatura** da assinatura transferida: **1**- A ID da assinatura do Partner Center é usada para fins de cobrança. **2**- A ID da assinatura do Azure original será mantida e aparecerá no Partner Center, bem como no Portal de Gerenciamento do Azure. Essa ID aparecerá no arquivo de reconciliação.  **Ao registrar os tíquetes de suporte em log, você precisará usar ambas as IDs.**

4. O cliente e novo parceiro da assinatura:

   Examine o formulário, preencha as informações sobre o novo parceiro e assine-o. Confirme se o novo cliente tem um contrato em vigor. Envie o formulário de volta para o parceiro de registro atual.

   *Importante*: se o novo parceiro CSP não tiver um relacionamento de revendedor com o cliente, ele deverá estabelecer um antes que a assinatura seja transferida. [Você pode encontrar informações sobre como fazer isso aqui](request-a-relationship-with-a-customer.md).

   >[!Note]
   >O novo parceiro CSP e o locatário do cliente devem estar no mesmo país. 

5. Parceiro atual:

   Verifique se o formulário inclui informações de contato para os administradores do parceiro. Suporte da Microsoft entrará em contato com ambos os administradores para verificar a transferência. Verifique se você tem todas as três assinaturas. Em seguida, use a opção de **carregamento de arquivo** para anexar o formulário concluído à sua solicitação de serviço existente. Um engenheiro de suporte da Microsoft chegará a você dentro de oito horas de trabalho para validar o recebimento e a conclusão.

6. Novo parceiro:

   Atualize as configurações de assinatura do Azure para remover o antigo parceiro da conta. Para ver quais atribuições de função são provisionadas, execute dois commandlets do PowerShell.

   - Adicionar o novo parceiro como o revendedor na conta:

     ```powershell
     Add-AzureRMAccount -tenant "CustomerDomainName"
     ```

     Para encontrar o customerDomainName: no menu Partner Center, selecione **Clientes**. Na lista de clientes, selecione o cliente. No menu do cliente, selecione **Conta** e use o **Nome de domínio**.

   - Exibir funções na conta, incluindo parceiros CSP anteriores:

     ```powershell
     Get-AzureRMRoleAssignment
     ```

7. Remover permissões de acesso desatualizadas

   - No menu Partner Center, selecione **Clientes**.
   - Expanda a listagem de clientes e selecione **Exibir assinaturas**.
   - No menu do cliente, selecione **Gerenciamento de serviços**.
   - Em **Microsoft Azure**, clique no link para ir para o **Portal de Gerenciamento do Microsoft Azure**.
