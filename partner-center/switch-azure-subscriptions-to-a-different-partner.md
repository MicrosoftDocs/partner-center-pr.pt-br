---
title: Transferir assinatura do Azure para outro parceiro
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como alterar o parceiro Provedor de Soluções na Nuvem programa associado às assinaturas do Azure de um cliente.
ms.custom: SEOMAY.20
ms.localizationpriority: medium
author: dhirajgandhi
ms.author: dhgandhi
ms.date: 02/09/2021
ms.openlocfilehash: 94f79762e7fabb377b8d7b559ff9ba2623b135fe
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109856059"
---
# <a name="learn-how-to-transfer-a-customers-azure-subscriptions-to-another-partner"></a>Saiba como transferir as assinaturas do Azure de um cliente para outro parceiro

**Aplica-se a**: Partner Center | Partner Center for Microsoft Cloud for US Government

**Funções apropriadas:** Administrador global

Este artigo descreve como um cliente pode alternar seus serviços Microsoft Azure de um CSP (Provedor de Soluções na Nuvem) para outro.

Para alternar os serviços ou assinaturas do Azure de um cliente para um parceiro diferente, siga estas etapas manuais. O parceiro e o cliente precisam concluir as etapas.

>[!Note]  
>Atualmente, somente provedores diretos ou indiretos podem transferir assinaturas.
>Não é possível alterar parceiros para Provedor de Soluções na Nuvem assinaturas associadas ao plano do Azure, ao Office 365, ao Enterprise Mobility Suite ou às assinaturas do Microsoft Dynamics CRM.

## <a name="switch-partners-for-azure-subscriptions"></a>Mudar de parceiro para assinaturas do Azure

1. Para transferir uma assinatura do Azure para um novo parceiro, o cliente deve iniciar o processo e entrar em contato com seu parceiro atual de registro por escrito.

   >[!Note]
   > É responsabilidade do parceiro atual criar o tíquete de serviço que inicia o processo de transferência. A Microsoft não pode interferir em nome do cliente ou do novo parceiro. O cliente deve planejar trabalhar em conjunto com o parceiro atual para que a transição ocorra sem problemas.

2. O parceiro da assinatura precisa realizar as seguintes tarefas:

   Crie um tíquete de serviço do Azure no Partner Center para solicitar uma transferência de assinatura:

   1. No menu Partner Center, selecione **Clientes**, selecione seu cliente na lista e, em seguida, selecione **Gerenciamento de serviços**.

   2. Na seção **Tíquetes de suporte**, selecione a lista suspensa **Novo tíquete** e escolha **Microsoft Azure**.
   
   3. No [portal do Azure](https://portal.azure.com), selecione **Nova solicitação de suporte**.
   
   4. Na Etapa 1, escolha **Gerenciar assinatura** como o tipo de problema, especifique a ID da assinatura que você deseja transferir e escolha **Provedor de Soluções na Nuvem** como o plano de suporte.
   
   5. Na Etapa 2, selecione **C-Impacto mínimo** e escolha **Outras Perguntas Gerais** como o tipo de problema.
   
   6. Faça o download do [formulário de transferência de assinatura do CSP](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC).

3. O parceiro da assinatura: preencha o [formulário de transferência de assinatura de CSP](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RWwTWC), assine-o e envie-o para o cliente. 

   Para preencher o formulário, você precisará das informações a seguir:

   - Informações de contato do parceiro atual e a ID da Microsoft. No menu Partner Center, selecione **Configurações da conta** &gt; **Perfil de organização**, e use a **ID da Microsoft**, o **Nome da organização** e o **Endereço** listados lá.

   - ID Microsoft. do cliente. No menu Partner Center, selecione **Clientes**, em seguida, expanda a listagem de clientes para ver a **ID da Microsoft**.

   - A ID de assinatura a ser transferida. Na listagem de clientes expandida, selecione **Exibir Assinaturas**, em seguida, expanda a assinatura escolhida para ver a **ID de Assinatura**.

   >[!Note]
   >A transferência de uma assinatura resulta em duas IDs de assinaturas que você verá na página **Editar Assinatura** da assinatura transferida: **1**- A ID da assinatura do Partner Center é usada para fins de cobrança. **2**- A ID da assinatura do Azure original será mantida e aparecerá no Partner Center, bem como no Portal de Gerenciamento do Azure. Essa ID aparecerá no arquivo de reconciliação.  **Ao registrar os tíquetes de suporte em log, você precisará usar ambas as IDs.**

4. O cliente e novo parceiro da assinatura:

   Examine o formulário, preencha as informações sobre o novo parceiro e assine-o. Confirme se o novo cliente tem um contrato em vigor. Envie o formulário de volta para o parceiro de registro atual.

   *Importante:* se o novo Parceiro CSP não tiver uma relação de revendedor com o cliente, ele deverá estabelecer um antes que a assinatura seja transferida. [Você pode encontrar informações sobre como fazer isso aqui](request-a-relationship-with-a-customer.md).

   >[!Note]
   >O novo parceiro CSP e o locatário do cliente devem estar no mesmo país. 

5. Parceiro atual:

   Certifique-se de que o formulário inclua informações de contato para ambos os administradores de parceiros. Suporte da Microsoft contatará os dois administradores para verificar a transferência. Certifique-se de ter todas as três assinaturas. Em seguida, use **a opção Upload** de Arquivo para anexar o formulário concluído à sua solicitação de serviço existente. Um engenheiro de suporte da Microsoft retornará a você dentro de oito horas comerciais para validar o recebimento e a conclusão.

6. Novo parceiro:

   Atualize as configurações de assinatura do Azure para remover o antigo parceiro da conta. Para ver quais atribuições de função são provisionadas, execute dois commandlets do PowerShell.

   - Adicionar o novo parceiro como o revendedor na conta:

     ```powershell
     Connect-AzAccount -Tenant 'xxxx-xxxx-xxxx-xxxx'
     ```

     >[!NOTE]
     > A ID de **locatário** do cliente aparece no Partner Center como a **ID da Microsoft** do cliente. Para localizar a ID da Microsoft (ID do locatário) de um cliente específico, entre no [painel](https://partner.microsoft.com/dashboard)do Partner Center. Em seguida, selecione **clientes** no menu. Localize o cliente na lista. Selecione a seta para baixo para expandir a listagem do cliente. Você verá informações sobre o *nome de domínio* do cliente e a ID da **Microsoft** do cliente. Use a **ID da Microsoft** de 16 dígitos no commandlet do PowerShell.

   - Exibir funções na conta, incluindo parceiros CSP anteriores:

     ```powershell
     Get-AzRoleAssignment
     ```

7. Remover permissões de acesso desatualizadas:

   - No menu Partner Center, selecione **Clientes**.
   - Localize o cliente na lista. Selecione (clique duas vezes) o nome da empresa. Essa ação abre a página **assinaturas** de cliente.
   - No menu de detalhes do cliente, selecione **Gerenciamento de serviços**.
   - Em **Microsoft Azure**, selecione o link para acessar a **portal de gerenciamento do Microsoft Azure**.

## <a name="next-steps"></a>Próximas etapas

- Faça o download do [formulário de transferência de assinatura do CSP](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE4ATIA).

- Saiba mais sobre o [suporte a vários parceiros](multipartner.md).

- [suporte a vários parceiros](multipartner.md).
- [suporte a vários canais](multichannel.md).
- [Transferir as assinaturas do Azure](/azure/cost-management-billing/manage/transfer-subscriptions-subscribers-csp)