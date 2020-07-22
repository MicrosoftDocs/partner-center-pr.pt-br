---
title: Confirmar a aceitação do cliente do Contrato de Cliente da Microsoft
ms.topic: article
ms.date: 05/05/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Aprenda a confirmar a aceitação do cliente do Contrato de Cliente da Microsoft. Os CSPs precisam disso para solicitar serviços e produtos da Microsoft para clientes.
author: aarzh-AaronZhang
ms.author: v-aarzh
ms.localizationpriority: high
ms.custom: SEOMAY.20
ms.openlocfilehash: 9df7dadbf9d2e6d1cc685b888ea2ae18436c8abf
ms.sourcegitcommit: 7153f0b8c67efd35f58695ca2a7e00e70da1c5e9
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/17/2020
ms.locfileid: "86435425"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement-in-the-csp-partner-program"></a>Confirmar a aceitação do Contrato de Cliente da Microsoft pelo cliente no programa de parceiro CSP

**Aplica-se a**

- Partner Center
- Centro de administração do Microsoft 365

**Funções apropriadas**

- Agente administrativo
- Agente de vendas

**Tipos de parceiros apropriados**

- Revendedores indiretos, cobrança direta, provedores indiretos

Em 1º de outubro de 2019, a Microsoft introduziu o **Contrato de Cliente da Microsoft** ao programa CSP para substituir o Contrato do Microsoft Cloud. Leia [diretrizes](indirect-reseller-tasks-in-partner-center.md) adicionais para revendedores indiretos. Para facilitar a migração dos parceiros para o novo contrato, os dois contratos coexistiram no programa CSP até 31 de janeiro de 2020. Em 1º de fevereiro de 2020, o Contrato de Cliente da Microsoft substituiu o Contrato do Microsoft Cloud.

Os clientes têm duas opções para aceitar o Contrato de Cliente da Microsoft. 

**Opção 1**: Atestado do parceiro da aceitação do cliente – o parceiro pode confirmar a aceitação do cliente usando o SDK/a API do Partner Center ou pelo painel do Partner Center.

**Opção 2**: Aceitação direta do cliente – o parceiro pode convidar o cliente por uma URL para examinar e aceitar o contrato no Centro de administração do Microsoft 365.

## <a name="access-microsoft-customer-agreement-template"></a>Acessar o modelo do Contrato de Cliente da Microsoft

Você pode baixar manualmente a última versão do modelo do Contrato de Cliente da Microsoft [aqui](https://aka.ms/customeragreement). O Contrato de Cliente da Microsoft é específico para cada país. Ao solicitar o modelo do Contrato de Cliente da Microsoft, selecione o país correto com base no local do cliente.

## <a name="option-1-confirm-customer-acceptance-in-partner-center"></a>Opção 1: Confirmar a aceitação do cliente no Partner Center

Os parceiros podem confirmar a aceitação do Contrato de Cliente da Microsoft pelo cliente na Central de Parceiros para clientes novos e existentes. Os revendedores não podem atestar em nome de seus clientes e precisam trabalhar com seu Provedor Indireto para que o atestado seja concluído.

### <a name="confirm-customer-acceptance-for-new-customers"></a>Confirmar a aceitação do cliente para novos clientes

Ao criar um novo locatário do cliente no Partner Center, use as etapas a seguir para confirmar a aceitação do cliente do contrato do cliente da Microsoft. Você deve ser um agente de administração ou um agente de vendas para executar essas etapas.

1. Selecione **Clientes**e então **Novo cliente**.

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

Você pode recuperar a confirmação de que um cliente existente aceitou o contrato de cliente da Microsoft usando as etapas a seguir. Você deve ser um Agente administrativo ou Agente de vendas para fazer isso.

1. Selecione **Clientes** e então localize e selecione o cliente que você deseja ver.

2. Selecione **Informações da Conta**.

3. Em **contrato de cliente da Microsoft**, veja se a confirmação tem ou não foi fornecida por este cliente.

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>Confirmar a aceitação do cliente usando o SDK/a API do Partner Center

Você pode usar o SDK/a API do Partner Center para confirmar a aceitação do cliente do Contrato de Cliente da Microsoft. Para obter detalhes sobre a API ou o SDK, confira:

- [Obter metadados do Contrato de Cliente da Microsoft](https://docs.microsoft.com/partner-center/develop/get-customer-agreement-metadata)

- [Confirmar a aceitação do cliente do Contrato de Cliente da Microsoft](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent-customer-agreement)

- [Obter a confirmação da aceitação do Contrato de Cliente da Microsoft pelo cliente](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-agreement)

- [Obter um link de download para o modelo do Contrato de Cliente da Microsoft](https://docs.microsoft.com/partner-center/develop/download-customer-agreement-template)

## <a name="option-2-customer-acceptance-in-microsoft-365-admin-center"></a>Opção 2: Aceitação do cliente no Centro de administração do Microsoft 365

Os parceiros podem convidar clientes novos e existentes, por meio de uma URL, para revisar e aceitar o contrato dentro do Centro de administração do Microsoft 365. As próximas seções mostram como:

- Criar um cliente e convidá-lo a examinar e aceitar o contrato.

- Convidar um novo cliente para examinar e aceitar a relação e o contrato do revendedor.

- Convidar um cliente existente para examinar e aceitar o contrato.

>[!NOTE]
> Você pode usar [o SDK ou a API do Partner Center](https://docs.microsoft.com/partner-center/develop/get-direct-sign-status-of-customer-agreement) para confirmar o status da aceitação direta do cliente do Contrato de Cliente da Microsoft.  

## <a name="create-a-new-customer-and-invite-the-customer-to-review-and-accept-the-agreement"></a>Criar um cliente e convidá-lo a examinar e aceitar o contrato

Use as etapas a seguir para criar um cliente no Partner Center e convidá-lo a revisar e aceitar o Contrato de Cliente da Microsoft dentro do Centro de administração do Microsoft 365.

1. Na guia **Clientes** no Partner Center, selecione **Adicionar cliente**.

2. Em **Informações sobre a conta**, insira as informações sobre o novo cliente em todos os campos obrigatórios, incluindo o nome da empresa e o contato principal do cliente.

3. Em **Contrato de Cliente**, selecione a primeira opção, **Será solicitado que o cliente aceite o Contrato de Cliente da Microsoft no Centro de administração do Microsoft 365**. Preencha todos os outros campos obrigatórios na página.

4. Selecione **Avançar: Examinar**. Em seguida, prossiga com as etapas para criar o locatário do cliente. 

>[!NOTE] 
>Novos clientes não podem fazer uma nova compra até aceitarem o Contrato de Cliente da Microsoft.  

   :::image type="content" source="images/mca/create-new-customer.jpg" alt-text="Criar cliente":::

5. Ao acessar a tela de **Confirmação** no novo fluxo de trabalho do cliente, salve as credenciais dele. Você precisará fornecer essas credenciais para o cliente mais tarde.

6. Fora do Partner Center, crie e envie um email que convida o cliente a aceitar o Contrato de Cliente da Microsoft no Centro de administração do Microsoft 365. Inclua estes itens no email:

   - Um link para esta [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement) (é necessário se conectar)

   - As credenciais do cliente que você salvou na Etapa 5.

7. O cliente receberá o convite por email do parceiro e selecionará a [URL](https://admin.microsoft.com/AdminPortal/Home?ref=/BillingAccounts/agreement).

8. O cliente entra no Centro de administração do Microsoft 365 usando as credenciais do cliente recebidas anteriormente do parceiro.

9. O cliente marca a caixa para aceitar o Contrato de Cliente da Microsoft.

## <a name="invite-a-new-customer-to-review-and-accept-the-reseller-relationship-and-microsoft-customer-agreement"></a>Convidar um novo cliente para revisar e aceitar a relação de revendedor e o Contrato de Cliente da Microsoft 

Use as etapas a seguir para convidar um novo cliente a revisar e aceitar a relação de revendedor e o Contrato de Cliente da Microsoft. 

1. Na guia **Clientes** no Partner Center, selecione o link **Solicitar uma relação de revendedor**. 

2. Um modelo de email automático será gerado, incluindo um texto e uma URL parametrizada que direcionará o cliente para o Centro de administração do Microsoft 365.

3. Você pode personalizar o modelo de email gerado automaticamente e, em seguida, selecionar **Copiar para a área de transferência** ou **Abrir no email**.

4. Use este modelo de email para convidar o cliente a aceitar a solicitação de **relação de revendedor** e o **Contrato de Cliente da Microsoft**. (Observação: no convite por email, verifique se o parceiro também inclui a URL fornecida automaticamente, assim como as credenciais do cliente criadas recentemente.)

   :::image type="content" source="images/mca/createrelationship.png" alt-text="criar uma relação":::

5. O cliente recebe o convite por email e clica na URL parametrizada. 

6. O cliente usa as credenciais fornecidas pelo parceiro no email para entrar no Centro de administração do Microsoft 365.

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
>Em determinados cenários, os clientes talvez não possam aceitar diretamente o Contrato de Cliente da Microsoft. Para saber mais sobre essas situações, confira [Dois cenários em que você precisa atestar em nome do cliente](attest-acceptance-customer-agreement.md).

### <a name="historical-timeline-details"></a>Detalhes do cronograma histórico

| Data | Marco | Detalhes |
|------------|------------|--------------------------------|
|1º de agosto de 2019|Visualização de UX disponível na área restrita|Os parceiros podem confirmar a aceitação do cliente do contrato de cliente da Microsoft usando o painel do Partner Center no ambiente de área restrita do CSP. Os parceiros com acesso ao ambiente de área restrita do CSP visualizam as alterações na experiência do usuário. Parceiros sem acesso à área restrita podem aprender sobre as alterações neste tópico.|
|3 de setembro de 2019|A visualização da API está disponível na área restrita.|O parceiro pode confirmar a aceitação do cliente do contrato do cliente da Microsoft usando a API do Partner Center no ambiente de área restrita do CSP. Os parceiros de API podem usar essa oportunidade para visualizar as alterações de API e começar a trabalhar na integração de API para dar suporte ao novo contrato.|
|20 de setembro de 2019|A versão prévia do SDK do .NET está disponível na área restrita.|O parceiro pode confirmar a aceitação do cliente do Contrato de Cliente da Microsoft usando o SDK do .NET do Partner Center no ambiente de área restrita do CSP. Os parceiros de API podem usar essa oportunidade para visualizar as alterações no SDK do .NET e começar a trabalhar na integração de API para oferecer suporte ao novo contrato.|
|1º de outubro de 2019|Contrato de cliente da Microsoft disponível em produção|A Microsoft apresenta o contrato do cliente da Microsoft ao programa CSP para substituir o contrato de Microsoft Cloud. Os parceiros podem confirmar a aceitação do cliente do contrato de cliente da Microsoft usando o painel do Partner Center e a API em produção. O contrato de Microsoft Cloud permanece com suporte no programa de parceiro CSP. No entanto, os parceiros são aconselhados a começar a migrar para o contrato do cliente da Microsoft. As novas compras e as alterações na contagem de estações para assinaturas existentes exigirão a confirmação do parceiro do contrato do cliente da Microsoft ou do contrato de Microsoft Cloud. Certas ofertas novas (por exemplo, o novo plano do Azure) exigirão a confirmação do contrato do cliente da Microsoft.|
|31 de janeiro de 2020|Contrato de Microsoft Cloud removido da produção|O contrato de Microsoft Cloud não é mais aceito no programa de parceiro CSP. As novas compras e as alterações na contagem de estações para assinaturas existentes exigirão que o parceiro forneça a confirmação do contrato com o cliente da Microsoft. Esse requisito se aplica a novos clientes e clientes existentes que podem ter aceitado anteriormente o contrato de Microsoft Cloud.|
|3 de fevereiro de 2020|Agora o parceiro tem a opção de convidar o cliente por uma URL para revisar e aceitar o contrato no Centro de administração do Microsoft 365 autenticado. | O cliente pode aceitar o Contrato de Cliente da Microsoft no Centro de administração do Microsoft 365. A aceitação direta do cliente do contrato no Centro de administração do Microsoft 365 confirma a aprovação dos termos. 
