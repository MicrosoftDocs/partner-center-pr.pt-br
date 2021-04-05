---
title: Como confirmar se o cliente aceitou o Contrato de Cliente da Microsoft para o programa CSP
description: Os parceiros do CSP (Provedor de Soluções na Nuvem) precisam confirmar a aceitação do Contrato de Cliente da Microsoft pelo cliente antes de solicitar os serviços Microsoft para os clientes.
ms.topic: how-to
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.date: 03/24/2021
ms.openlocfilehash: ebb52a3a8223d3b1101e3a8e78728fcc167e25e3
ms.sourcegitcommit: a691d4cbe144a8fd71e344fd293cc658ac11d6f3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/27/2021
ms.locfileid: "105633770"
---
# <a name="how-to-confirm-that-your-customer-has-accepted-the-microsoft-customer-agreement-to-the-csp-program"></a>Como confirmar se o cliente aceitou o Contrato de Cliente da Microsoft para o programa CSP

**Funções apropriadas**

- Agente administrativo
- Agente de vendas


Os clientes têm duas opções para aceitar o Contrato de Cliente da Microsoft.

**Opção 1**: Atestado do parceiro da aceitação do cliente – o parceiro pode confirmar a aceitação do cliente usando o SDK/a API do Partner Center ou pelo painel do Partner Center.

**Opção 2**: Aceitação direta do cliente – o parceiro pode convidar o cliente por uma URL para examinar e aceitar o contrato no Centro de administração do Microsoft 365.

## <a name="access-microsoft-customer-agreement-template"></a>Acessar o modelo do Contrato de Cliente da Microsoft

Você pode baixar manualmente a última versão do modelo do Contrato de Cliente da Microsoft [aqui](https://aka.ms/customeragreement). O Contrato de Cliente da Microsoft é específico para cada país. Ao solicitar o modelo do Contrato de Cliente da Microsoft, selecione o país correto com base no local do cliente.

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a>Opção 1: Confirmar a aceitação do cliente no Partner Center

Os parceiros de fatura direta podem confirmar a aceitação do Contrato de Cliente da Microsoft pelo cliente no Partner Center para clientes novos e existentes. Os revendedores indiretos não podem atestar em nome de seus clientes e precisam trabalhar com seu Provedor Indireto para que o atestado seja concluído.

### <a name="confirm-customer-acceptance-for-new-customers"></a>Confirmar a aceitação do cliente para novos clientes

Ao criar um novo locatário do cliente no Partner Center, use as etapas a seguir para confirmar a aceitação do cliente do contrato do cliente da Microsoft. Você deve ser um agente de administração ou um agente de vendas para executar essas etapas.

1. Selecione **Clientes** e então **Novo cliente**.

2. Em **informações da conta**, insira informações para a empresa e seu contato principal.

3. Em **Contrato da Microsoft**, marque a caixa para atestar que o cliente aceitou o Contrato de Cliente da Microsoft.

4. Em **Data de aceitação do contrato**, insira a data apropriada. Você não pode definir isso como uma data futura.

5. Verifique se as informações de contato do usuário primário exibidas estão corretas. Se estiver incorreto, selecione **Atualizar** e insira as informações corretas da pessoa que aceitou o contrato.

6. Selecione **Avançar** para continuar criando o locatário do cliente.

   :::image type="content" source="images/mca/newcustomeragreement.jpg" alt-text="Novo cliente":::  

### <a name="confirm-customer-acceptance-for-existing-customers"></a>Confirmar a aceitação do cliente para clientes existentes

Você deve ser um Agente administrativo ou Agente de vendas para fazer isto:

1. Selecione **Clientes**. Localize e selecione o cliente.

2. Selecione **Informações da Conta**.

3. Em **Contrato de Cliente da Microsoft**, selecione **Atualizar**.

4. Insira o **Nome**, **Sobrenome**, **E-mail** e **Número de telefone** (opcional) do usuário que aceitou o contrato. Em **Data de aceitação do contrato**, insira a data apropriada. Você não pode definir isso como uma data futura.

5. Selecione **Salvar** e continue.

   :::image type="content" source="images/mcua2-update2.png" alt-text="Cliente existente":::

### <a name="retrieve-confirmation-of-customer-acceptance"></a>Recuperar confirmação de aceitação do cliente

Para recuperar a confirmação de que um cliente existente aceitou o Contrato de Cliente da Microsoft, use as etapas a seguir. Você deve ser um Agente administrativo ou Agente de vendas para fazer isso.

1. Selecione **Clientes** e então localize e selecione o cliente que você deseja ver.

2. Selecione **Informações da Conta**.

3. Em **contrato de cliente da Microsoft**, veja se a confirmação tem ou não foi fornecida por este cliente.

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>Confirmar a aceitação do cliente usando o SDK/a API do Partner Center

Você pode usar o SDK/a API do Partner Center para confirmar a aceitação do cliente do Contrato de Cliente da Microsoft. Para obter detalhes sobre a API ou o SDK, confira:

- [Obter metadados do Contrato de Cliente da Microsoft](/partner-center/develop/get-customer-agreement-metadata)

- [Confirmar a aceitação do cliente do Contrato de Cliente da Microsoft](/partner-center/develop/confirm-customer-consent-customer-agreement)

- [Obter a confirmação da aceitação do Contrato de Cliente da Microsoft pelo cliente](/partner-center/develop/get-confirmation-of-customer-agreement)

- [Obter um link de download para o modelo do Contrato de Cliente da Microsoft](/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a>Opção 2: Aceitação do cliente no Centro de administração do Microsoft 365

Os parceiros podem convidar clientes novos e existentes, por meio de uma URL, para revisar e aceitar o contrato dentro do Centro de administração do Microsoft 365. As próximas seções mostram como:

- Criar um cliente e convidá-lo a examinar e aceitar o contrato.

- Convidar um novo cliente para examinar e aceitar a relação e o contrato do revendedor.

- Convidar um cliente existente para examinar e aceitar o contrato.

>[!NOTE]
> Você pode usar [o SDK ou a API do Partner Center](/partner-center/develop/get-direct-sign-status-of-customer-agreement) para confirmar o status da aceitação direta do cliente do Contrato de Cliente da Microsoft.  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a>Criar um cliente e convidá-lo a examinar e aceitar o contrato

Use as etapas a seguir para criar um cliente no Partner Center e convidá-lo a revisar e aceitar o Contrato de Cliente da Microsoft dentro do Centro de administração do Microsoft 365.

1. Na guia **Clientes** no Partner Center, selecione **Adicionar cliente**.

2. Em **Informações sobre a conta**, insira as informações sobre o novo cliente em todos os campos obrigatórios, incluindo o nome da empresa e o contato principal do cliente.

3. Em **Contrato de Cliente**, selecione a opção **Será solicitado que o cliente aceite o Contrato de Cliente da Microsoft no Centro de Administração do Microsoft 365**. Preencha todos os outros campos obrigatórios na página.

4. Selecione **Avançar: Examinar**. Em seguida, prossiga com as etapas para criar o locatário do cliente. 

>[!NOTE] 
>Novos clientes não podem fazer uma compra até aceitarem o Contrato de Cliente da Microsoft.  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Criar cliente":::

5. Ao acessar a tela de **Confirmação** no novo fluxo de trabalho do cliente, salve as credenciais dele. Você precisará fornecer essas credenciais para o cliente mais tarde.

6. Fora do Partner Center, crie e envie um email que convida o cliente a aceitar o Contrato de Cliente da Microsoft no Centro de administração do Microsoft 365. Inclua estes itens no email:

   - Um link para esta [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (é necessário se conectar)

   - As credenciais do cliente que você salvou na Etapa 5.

7. O cliente receberá o convite por email do parceiro e selecionará a [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).

8. O cliente entra no Centro de Administração do Microsoft 365 usando as credenciais do cliente que você forneceu.

9. O cliente marca a caixa para aceitar o Contrato de Cliente da Microsoft.

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a>Convidar um novo cliente para revisar e aceitar a relação de revendedor e o Contrato de Cliente da Microsoft 

Use as etapas a seguir para convidar um novo cliente a revisar e aceitar a relação de revendedor e o Contrato de Cliente da Microsoft. 

1. Na guia **Clientes** no Partner Center, selecione o link **Solicitar uma relação de revendedor**. 

2. Um modelo de email automático será gerado, incluindo um texto e uma URL parametrizada que direcionará o cliente para o Centro de Administração do Microsoft 365.

3. Você pode personalizar o modelo de email gerado automaticamente e, em seguida, selecionar **Copiar para a área de transferência** ou **Abrir no email**.

4. Use este modelo de email para convidar o cliente a aceitar a solicitação de **relação de revendedor** e o **Contrato de Cliente da Microsoft**. (Observação: no convite por email, verifique se o parceiro também inclui a URL fornecida automaticamente, assim como as credenciais do cliente criadas recentemente.)

   :::image type="content" source="images/mca/createrelationship.png" alt-text="criar uma relação":::

5. O cliente recebe o convite por email e clica na URL parametrizada. 

6. O cliente usa as credenciais fornecidas por você no email para entrar no Centro de Administração do Microsoft 365.

7. O cliente marca a caixa para aceitar a **relação de revendedor** e o **Contrato de Cliente da Microsoft**. 

8. Na mesma URL, o cliente pode ver uma lista consolidada de diferentes parceiros com os quais ele está trabalhando. Ele pode selecionar um parceiro para ver os detalhes.

   :::image type="content" source="images/mca/accept.jpg" alt-text="Aceitar o contrato":::


## <a name="invite-an-existing-customer-to-review-and-accept-the-agreement"></a>Convidar um cliente existente para revisar e aceitar o contrato

Use as etapas a seguir para convidar um cliente existente a revisar e aceitar o Contrato de Cliente da Microsoft. 

1. Crie o email do cliente com a URL inserida que convida seu cliente a aceitar o Contrato de Cliente da Microsoft.

2. O cliente recebe o convite por email e clica na [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement). 

3. O cliente insere as credenciais dele no Centro de administração do Microsoft 365.

4. Seu cliente marca a caixa para aceitar o Contrato de Cliente da Microsoft. 

5. Na mesma URL, o cliente pode ver a lista consolidada de diferentes parceiros com os quais eles estão trabalhando. Ele pode selecionar um parceiro para ver os detalhes.

   :::image type="content" source="images/mca/customeraccept.png" alt-text="cliente":::

>[!NOTE]
>Em determinados cenários, os clientes talvez não possam aceitar diretamente o Contrato de Cliente da Microsoft. Para saber mais sobre essas situações, leia a próxima seção: Dois cenários em que você precisa atestar em nome do cliente.

## <a name="two-scenarios-where-you-need-to-attest-on-behalf-of-your-customer"></a>Dois cenários em que você precisa atestar em nome do seu cliente

Há dois cenários em que os clientes talvez não possam aceitar diretamente o Contrato de Cliente da Microsoft dentro do Centro de Administração do Microsoft 365.

**Cenário 1**: um cliente existente comprou qualquer um dos seguintes itens por meio de um relacionamento com o parceiro existente: ofertas, software ou assinaturas de software, Instâncias Reservadas ou o Plano do Azure. Agora, o cliente está tentando fazer qualquer nova compra (excluindo a renovação automática). Quando esse cliente clicar na URL, receberá a mensagem “Entre em contato com seu Parceiro para confirmar a aceitação do Contrato de Cliente da Microsoft”.  

**Para resolver**: você deve atestar em nome do cliente.

:::image type="content" source="images/mca/accept-scenario-1.png" alt-text="Captura de tela da página do Centro de administração do Microsoft 365 solicitando que você entre em contato com seu parceiro para confirmar a aceitação do Contrato de Cliente da Microsoft.":::

**Cenário 2**: um cliente comprou uma das seguintes ofertas, softwares ou assinaturas de software, Instâncias Reservadas ou Plano do Azure. Agora, o cliente está tentando fazer qualquer nova compra com um novo parceiro.

Quando o cliente clicar na URL para o Centro de administração do Microsoft 365 para aceitar o novo relacionamento com o parceiro e o contrato, ele receberá a mensagem “Entre em contato com seu Parceiro para confirmar sua aceitação do Contrato de Cliente da Microsoft”.  

**Para resolver**: você deve atestar em nome do cliente.  

## <a name="confirm-that-a-customer-has-accepted-the-agreement"></a>Confirmar que um cliente aceitou o contrato

Se você tentar criar um pedido para um cliente existente que não fez a confirmação antes, receberá um aviso para concluir a confirmação. Use o procedimento a seguir para fazer isso.

1. Insira o **Nome**, **Sobrenome**, **Endereço de email** e **Número de telefone** (opcional) do usuário que aceitou o contrato.

2. Em **Data de aceitação do contrato**, insira a data apropriada. Você não pode definir isso como uma data futura.

3. Selecione **Salvar e continuar**. 

## <a name="next-steps"></a>Próximas etapas

- [Verificar ou atualizar as informações de perfil da sua empresa](update-your-partner-profile.md)
- [Contratos de Cliente da Microsoft (por região e idioma)](Agreements.md)
