---
title: Mudar assinaturas do Azure para outro parceiro | Partner Center
description: "Um cliente pode mudar o parceiro do programa Provedor de Soluções na Nuvem que usa para os serviços do Microsoft Azure. No entanto, esse é um processo manual que exige ações do parceiro e do cliente."
ms.assetid: 42D1D9AB-613D-4FC1-A846-EE769923E699
author: MaggiePucciEvans
translationtype: Human Translation
ms.sourcegitcommit: 14ba85c868e59dd1c77063f5b1b0e9ab8db7f82f
ms.openlocfilehash: 29ced9a3a7256f86f0f8708a4c72ac75b9269ffc

---

# Mudar assinaturas do Azure para outro parceiro


Um cliente pode mudar o parceiro do programa Provedor de Soluções na Nuvem que usa para os serviços do Microsoft Azure. No entanto, esse é um processo manual que exige ações do parceiro e do cliente.

**Observação**  Atualmente, não há um processo automático para os clientes do Azure mudarem do EA, Open ou outros programas de licenciamento para o CSP. Esse é um processo manual que exige ações do parceiro e do cliente. Além disso, não é possível mudar os parceiros para assinaturas de Provedor de Soluções na Nuvem do Office 365, Enterprise Mobility Suite ou Microsoft Dynamics CRM.

 

**Mudar de parceiro para assinaturas do Azure**

1.  Para transferir uma assinatura do Azure para um novo parceiro, o cliente deve iniciar o processo e entrar em contato com seu parceiro CSP atual de registro por escrito.

2.  O CSP da assinatura deve executar as seguintes tarefas:

    Crie um tíquete de serviço do Azure no Partner Center para solicitar uma transferência de assinatura:

    -   No menu do painel do Partner Center, selecione **Clientes**, selecione seu cliente na lista, em seguida, selecione **Gerenciamento de serviço**. Na seção **Tíquetes de suporte**, selecione a lista suspensa **Novo tíquete** e escolha **Microsoft Azure**.

    -   No portal do Azure, selecione **Nova solicitação de suporte**.

        Na Etapa 1, escolha **Gerenciar assinatura** como o tipo de problema, especifique a ID da assinatura que você deseja transferir e escolha **Provedor de Soluções na Nuvem** como o plano de suporte.

        Na etapa 2, selecione **Impacto mínimo C** e escolha **Outras Perguntas Gerais** como o tipo de problema.

        Baixe o [formulário de transferência de assinatura de CSP](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip).

3.  Parceiro CSP atual da assinatura: preencha o [formulário de transferência de assinatura de CSP](https://assets.windowsphone.com/5222c408-e546-4e01-b72a-2ec7d4c43d57/CSP_Subscription_Transfer_Form_Azure_InvariantCulture_Default.zip), assine-o e envie-o para o cliente. Para preencher o formulário, você precisará das informações a seguir:

    -   Informações de contato do parceiro atual e a ID da Microsoft. No menu Partner Center, selecione **Configurações da conta** &gt; **Perfil de organização**, e use a **ID da Microsoft**, o **Nome da organização** e o **Endereço** listados lá.

    -   A ID da Microsoft do cliente. No menu Partner Center, selecione **Clientes**, em seguida, expanda a listagem de clientes para ver a **ID da Microsoft**.

    -   A ID de assinatura a ser transferida. Na listagem de clientes expandida, selecione **Exibir Assinaturas**, em seguida, expanda a assinatura escolhida para ver a **ID de Assinatura**.

4.  Cliente e novo CSP da assinatura:

    Examine o formulário, preencha as informações sobre o novo parceiro e assine-o. Confirme se o novo cliente tem um contrato em vigor. Envie o formulário de volta para o parceiro de registro atual.

    *Importante*: se o novo parceiro CSP não tiver uma relação de revendedor com o cliente, ele deverá estabelecer uma antes para a assinatura que será transferida. [Você pode encontrar informações sobre como fazer isso aqui](https://int.msdn.microsoft.com/en-us/library/partnercenter/mt750320.aspx).

5.  Parceiro CSP atual:

    Certifique-se de que o formulário inclui informações de contato de ambos parceiros administradores. O Suporte da Microsoft entrará em contato com ambos os administradores para verificar a transferência. Garanta que todas as três assinaturas estejam em vigor e, em seguida, anexe o formulário preenchido à sua solicitação de serviço existente usando a opção **Carregamento de Arquivo**. Um engenheiro de suporte da Microsoft entrará em contato com você dentro de 8 horas úteis para validar o recebimento e a conclusão.

6.  Novo parceiro CSP:

    Atualize as configurações de assinatura do Azure para remover o antigo parceiro da conta. Para ver quais atribuições de função são provisionadas, execute dois Commandlets do Powershell.

    -   Adicionar o novo parceiro como o revendedor na conta:

        **PS C:\\&gt; Add-AzureRMAccount -tenant "CustomerDomainName"**

        Para encontrar o customerDomainName: no menu Partner Center, selecione **Clientes**. Na lista de clientes, selecione o cliente. No menu do cliente, selecione **Conta** e use o **Nome de domínio**.

    -   Exibir funções na conta, incluindo parceiros CSP anteriores:

        **PS C:\\&gt; Get-AzureRMRoleAssignment**

    Remova permissões de acesso desatualizadas para assinatura e os recursos, gerenciando a assinatura no Portal do Azure. No menu Partner Center, selecione **Clientes**. Expanda a listagem de clientes e selecione **Exibir assinaturas**. No menu do cliente, selecione **Gerenciamento de serviços**. Em **Microsoft Azure**, clique no link para ir para o **Portal de Gerenciamento do Microsoft Azure**.

 

 






<!--HONumber=Nov16_HO4-->


