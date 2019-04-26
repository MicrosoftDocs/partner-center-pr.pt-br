---
title: Transferir assinaturas do Azure | Partner Center
ms.topic: article
ms.date: 03/15/2019
description: Um cliente pode mudar o parceiro do programa Provedor de Soluções na Nuvem que usa para os serviços do Microsoft Azure. No entanto, esse é um processo manual que exige ações do parceiro e do cliente.
ms.assetid: 42D1D9AB-613D-4FC1-A846-EE769923E699
author: MaggiePucciEvans
ms.author: evansma
keywords: assinatura do Azure, mudar de parceiro, alterar parceiro, obter novo parceiro, outro parceiro
ms.localizationpriority: medium
ms.openlocfilehash: 2298763cd01ebc2f1b3849db27363b0a39eb78bf
ms.sourcegitcommit: b1ab80345b4e4af649fb8cc51d96d798e0791ade
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/23/2019
ms.locfileid: "62133847"
---
# <a name="transfer-azure-subscriptions"></a>Transferir assinaturas do Azure 

**Aplica-se a**

-  Partner Center

Um cliente pode decidir mudar para um parceiro do Provedor de Soluções na Nuvem ou um parceiro para obter os serviços do Microsoft Azure. Trata-se, porém, de um processo manual que exige ações do parceiro e do cliente.

>[!Note]  
>No momento apenas direta ou indireta provedores são capazes de transferir assinaturas.
>Atualmente, não é possível mudar os parceiros para assinaturas de Provedor de Soluções na Nuvem do Office 365, Enterprise Mobility Suite ou Microsoft Dynamics CRM.



**Parceiros de switch para assinaturas do Azure**

1. Para transferir uma assinatura do Azure para um novo parceiro, o cliente deve iniciar o processo e entrar em contato com seu parceiro atual de registro por escrito. 
>[!Note]
>É responsabilidade do parceiro atual criar o tíquete de serviço que inicia o processo de transferência. A Microsoft não pode interferir em nome do cliente ou do novo parceiro. O cliente deve planejar trabalhar em conjunto com o parceiro atual para que a transição ocorra sem problemas.

2. O parceiro da assinatura deve executar as seguintes tarefas:

Crie um tíquete de serviço do Azure no Partner Center para solicitar uma transferência de assinatura:
-   No menu do Partner Center, selecione **clientes**, selecione o cliente da lista e, em seguida, selecione **gerenciamento de serviço**. Na seção **Tíquetes de suporte**, selecione a lista suspensa **Novo tíquete** e escolha **Microsoft Azure**.

-   No portal do Azure, selecione **Nova solicitação de suporte**.

Na Etapa 1, escolha **Gerenciar assinatura** como o tipo de problema, especifique a ID da assinatura que você deseja transferir e escolha **Provedor de Soluções na Nuvem** como o plano de suporte.

Na etapa 2, selecione **Impacto mínimo C** e escolha **Outras Perguntas Gerais** como o tipo de problema.

Baixe o [formulário de transferência de assinatura de CSP](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip).

3. O parceiro para a assinatura: Preencha a [formulário de transferência de assinatura de CSP](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip), assiná-lo e, em seguida, enviá-lo para o cliente. Para preencher o formulário, você precisará das informações a seguir:

- Informações de contato do parceiro atual e a ID da Microsoft. No menu do Partner Center, selecione **configurações de conta** &gt; **perfil de organização**e usar o **ID da Microsoft**, **nome da organização** , e **endereço** listados lá.

- A ID da Microsoft do cliente. No menu Partner Center, selecione **Clientes**, em seguida, expanda a listagem de clientes para ver a **ID da Microsoft**.

- A ID de assinatura a ser transferida. Na listagem de clientes expandida, selecione **Exibir Assinaturas**, em seguida, expanda a assinatura escolhida para ver a **ID de Assinatura**.

>[!Note]
>Transferindo uma assinatura resulta em duas IDs que você verá da assinatura do **Editar assinatura** página da assinatura transferida: **1**-a ID de assinatura do Partner Center é usado para fins de cobrança. 
**2**- A ID da assinatura do Azure original será mantida e aparecerá no Partner Center, bem como no Portal de Gerenciamento do Azure. Essa ID aparecerá no arquivo de reconciliação.  **Ao fazer logon tíquetes de suporte, você precisa usar ambas as IDs.**

4. O cliente e novo parceiro da assinatura:

Examine o formulário, preencha as informações sobre o novo parceiro e assine-o. Confirme se o novo cliente tem um contrato em vigor. Envie o formulário de volta para o parceiro de registro atual.

*Importante*: Se o novo parceiro CSP não tem uma relação de revendedor com o cliente, elas precisam estabelecer antes da assinatura que estão sendo transferida. [Você pode encontrar informações sobre como fazer isso aqui](request-a-relationship-with-a-customer.md).

>[!Note]
>O novo parceiro CSP e o locatário do cliente devem estar no mesmo país. 

5. Parceiro atual:

Certifique-se de que o formulário inclui informações de contato de ambos parceiros administradores. O Suporte da Microsoft entrará em contato com ambos os administradores para verificar a transferência. Garanta que todas as três assinaturas estejam em vigor e, em seguida, anexe o formulário preenchido à sua solicitação de serviço existente usando a opção **Carregamento de Arquivo**. Um engenheiro de suporte da Microsoft entrará em contato com você dentro de 8 horas úteis para validar o recebimento e a conclusão.

6. Novo parceiro:

Atualize as configurações de assinatura do Azure para remover o antigo parceiro da conta. Para ver quais atribuições de função são provisionadas, execute dois Commandlets do Powershell.

-   Adicionar o novo parceiro como o revendedor na conta:

**PS C:\\&gt; Add-AzureRMAccount-"CustomerDomainName" do locatário**

Para encontrar o customerDomainName: no menu Partner Center, selecione **Clientes**. Na lista de clientes, selecione o cliente. No menu do cliente, selecione **Conta** e use o **Nome de domínio**.

-   Exibir funções na conta, incluindo parceiros CSP anteriores:

**PS C:\\&gt; Get-AzureRMRoleAssignment**

7. Remover permissões de acesso desatualizadas

-  No menu Partner Center, selecione **Clientes**. 
-  Expanda a listagem de clientes e selecione **Exibir assinaturas**. 
-  No menu do cliente, selecione **Gerenciamento de serviços**. 
-  Em **Microsoft Azure**, clique no link para ir para o **Portal de Gerenciamento do Microsoft Azure**.

 

 



