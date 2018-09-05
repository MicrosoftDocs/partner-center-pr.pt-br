---
title: Transferir assinaturas do Azure | Partner Center
description: Um cliente pode mudar o parceiro do programa Provedor de Soluções na Nuvem que usa para os serviços do Microsoft Azure. No entanto, esse é um processo manual que exige ações do parceiro e do cliente.
ms.assetid: 42D1D9AB-613D-4FC1-A846-EE769923E699
author: MaggiePucciEvans
keywords: assinatura do Azure, mudar de parceiro, alterar parceiro, obter novo parceiro, outro parceiro
ms.localizationpriority: medium
ms.openlocfilehash: 21737fd9b9633fb2a1c1fb05daba4d43dd50444d
ms.sourcegitcommit: 92629114d5081103bfe555081f69997af4ed56f2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2018
ms.locfileid: "2877556"
---
# <a name="transfer-azure-subscriptions"></a>Transferir assinaturas do Azure 

**Aplicável a**

-  Partner Center

Um cliente pode decidir mudar para um parceiro do Provedor de Soluções na Nuvem ou um parceiro para obter os serviços do Microsoft Azure. Trata-se, porém, de um processo manual que exige ações do parceiro e do cliente.

**Observação**  Neste momento apenas direta ou provedores indiretos são capazes de transferir assinaturas.

**Observação:** atualmente, não é possível mudar os parceiros para assinaturas de Provedor de Soluções na Nuvem do Office 365, Enterprise Mobility Suite ou Microsoft Dynamics CRM.



**Mudar de parceiro para assinaturas do Azure**

1.  Para transferir uma assinatura do Azure para um novo parceiro, o cliente deve iniciar o processo e entrar em contato com seu parceiro atual de registro por escrito. 

    >**Observação**<br> É responsabilidade do parceiro atual criar o tíquete de serviço que inicia o processo de transferência. A Microsoft não pode interferir em nome do cliente ou do novo parceiro. O cliente deve planejar trabalhar em conjunto com o parceiro atual para que a transição ocorra sem problemas.

2.  O parceiro da assinatura deve executar as seguintes tarefas:

    Crie um tíquete de serviço do Azure no Partner Center para solicitar uma transferência de assinatura:

    -   No menu do painel, selecione **Clientes**, selecione seu cliente na lista, em seguida, selecione **Gerenciamento de serviços**. Na seção **Tíquetes de suporte**, selecione a lista suspensa **Novo tíquete** e escolha **Microsoft Azure**.

    -   No portal do Azure, selecione **Nova solicitação de suporte**.

        Na Etapa 1, escolha **Gerenciar assinatura** como o tipo de problema, especifique a ID da assinatura que você deseja transferir e escolha **Provedor de Soluções na Nuvem** como o plano de suporte.

        Na etapa 2, selecione **Impacto mínimo C** e escolha **Outras Perguntas Gerais** como o tipo de problema.

        Baixe o [formulário de transferência de assinatura de CSP](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip).

3.  O parceiro da assinatura: preencha o [formulário de transferência de assinatura de CSP](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip), assine-o e envie-o para o cliente. Para preencher o formulário, você precisará das informações a seguir:

    -   Informações de contato do parceiro atual e a ID da Microsoft. No menu Partner Center, selecione **Configurações da conta** &gt; **Perfil de organização**, e use a **ID da Microsoft**, o **Nome da organização** e o **Endereço** listados lá.

    -   A ID da Microsoft do cliente. No menu Partner Center, selecione **Clientes**, em seguida, expanda a listagem de clientes para ver a **ID da Microsoft**.

    -   A ID de assinatura a ser transferida. Na listagem de clientes expandida, selecione **Exibir Assinaturas**, em seguida, expanda a assinatura escolhida para ver a **ID de Assinatura**.

    >**Observação**<br> A transferência de uma assinatura resulta em duas IDs de assinaturas que você verá na página **Editar Assinatura** da assinatura transferida: **1**- A ID da assinatura do Partner Center é usada para fins de cobrança. 
    **2**- A ID da assinatura do Azure original será mantida e aparecerá no Partner Center, bem como no Portal de Gerenciamento do Azure. Essa ID aparecerá no arquivo de reconciliação.  **Ao registrar os tíquetes de suporte em log, você precisará usar ambas as IDs.**

4.  O cliente e novo parceiro da assinatura:

    Examine o formulário, preencha as informações sobre o novo parceiro e assine-o. Confirme se o novo cliente tem um contrato em vigor. Envie o formulário de volta para o parceiro de registro atual.

    *Importante*: se o novo parceiro CSP não tiver uma relação de revendedor com o cliente, ele deverá estabelecer uma antes para a assinatura que será transferida. [Você pode encontrar informações sobre como fazer isso aqui](request-a-relationship-with-a-customer.md).

5.  Parceiro atual:

    Certifique-se de que o formulário inclui informações de contato de ambos parceiros administradores. O Suporte da Microsoft entrará em contato com ambos os administradores para verificar a transferência. Garanta que todas as três assinaturas estejam em vigor e, em seguida, anexe o formulário preenchido à sua solicitação de serviço existente usando a opção **Carregamento de Arquivo**. Um engenheiro de suporte da Microsoft entrará em contato com você dentro de 8 horas úteis para validar o recebimento e a conclusão.

6.  Novo parceiro:

    Atualize as configurações de assinatura do Azure para remover o antigo parceiro da conta. Para ver quais atribuições de função são provisionadas, execute dois Commandlets do Powershell.

    -   Adicionar o novo parceiro como o revendedor na conta:

        **PS C:\\&gt; Add-AzureRMAccount -tenant "CustomerDomainName"**

        Para encontrar o customerDomainName: no menu Partner Center, selecione **Clientes**. Na lista de clientes, selecione o cliente. No menu do cliente, selecione **Conta** e use o **Nome de domínio**.

    -   Exibir funções na conta, incluindo parceiros CSP anteriores:

        **PS C:\\&gt; Get-AzureRMRoleAssignment**

7. Remover permissões de acesso desatualizadas

    -  No menu Partner Center, selecione **Clientes**. 
    -  Expanda a listagem de clientes e selecione **Exibir assinaturas**. 
    -  No menu do cliente, selecione **Gerenciamento de serviços**. 
    -  Em **Microsoft Azure**, clique no link para ir para o **Portal de Gerenciamento do Microsoft Azure**.

 

 



