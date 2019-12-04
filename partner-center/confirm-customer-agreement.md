---
title: Confirmar a aceitação do cliente do contrato do cliente da Microsoft |Partner Center
ms.topic: article
ms.date: 11/25/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
Description: Saiba como confirmar a aceitação do cliente do contrato do cliente da Microsoft. Isso pode ser necessário para solicitar produtos e serviços da Microsoft para clientes.
author: LauraBrenner
ms.author: labrenne
keywords: cliente, clientes, consentimento, MCA, contrato de Microsoft Cloud, contrato de cliente da Microsoft, modelos de contrato de cliente
ms.localizationpriority: medium
ms.openlocfilehash: 8beee9ed9035ff846c6e9d84fefd0c5c2ba255de
ms.sourcegitcommit: c793c1b61f50fc0b0a12c95cedd9f57b31703093
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2019
ms.locfileid: "74721364"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement"></a>Confirmar a aceitação do cliente do contrato do cliente da Microsoft

**Funções apropriadas**

- Agente administrativo
- Agente de vendas

Atualmente, antes que um parceiro CSP possa fazer o pedido em nome de um cliente, o cliente deve aceitar e assinar o **contrato de Microsoft Cloud**aplicável. Em seguida, o parceiro deve confirmar a aceitação do cliente fornecendo informações sobre o assinante à Microsoft. Caso a confirmação não seja fornecida:
- Você não poderá criar novos pedidos para esse cliente.
- Você não poderá alterar a contagem de estações de assinaturas baseadas em assentos existentes para esse cliente.

Para obter detalhes sobre como confirmar a aceitação de um cliente do contrato de Microsoft Cloud usando o painel do Partner Center ou a API, confira [confirmar a aceitação do cliente do contrato de Microsoft Cloud](confirm-consent.md).

Em 1º de outubro de 2019, a Microsoft apresentará o **contrato do cliente da Microsoft** ao programa CSP para substituir o contrato de Microsoft Cloud. Para facilitar a migração dos parceiros para o novo contrato, haverá suporte para o Contrato do Microsoft Cloud atual no programa CSP até 31 de janeiro de 2020. Para obter mais detalhes do cronograma, consulte a tabela a seguir:

| Data | Marco | Detalhes |
|------------|------------|--------------------------------|
|1º de agosto de 2019|Visualização de UX disponível na área restrita|Os parceiros podem confirmar a aceitação do cliente do contrato de cliente da Microsoft usando o painel do Partner Center no ambiente de área restrita do CSP. Os parceiros com acesso ao ambiente de área restrita do CSP visualizam as alterações na experiência do usuário. Parceiros sem acesso à área restrita podem aprender sobre as alterações neste tópico.|
|3 de setembro de 2019|A visualização da API está disponível na área restrita.|O parceiro pode confirmar a aceitação do cliente do contrato do cliente da Microsoft usando a API do Partner Center no ambiente de área restrita do CSP. Os parceiros de API podem usar essa oportunidade para visualizar as alterações de API e começar a trabalhar na integração de API para dar suporte ao novo contrato.|
|20 de setembro de 2019|A versão prévia do SDK do .NET está disponível na área restrita.|O parceiro pode confirmar a aceitação do cliente do Contrato de Cliente da Microsoft usando o SDK do .NET do Partner Center no ambiente de área restrita do CSP. Os parceiros de API podem usar essa oportunidade para visualizar as alterações no SDK do .NET e começar a trabalhar na integração de API para oferecer suporte ao novo contrato.|
|1º de outubro de 2019|Contrato de cliente da Microsoft disponível em produção|A Microsoft apresenta o contrato do cliente da Microsoft ao programa CSP para substituir o contrato de Microsoft Cloud. Os parceiros podem confirmar a aceitação do cliente do contrato de cliente da Microsoft usando o painel do Partner Center e a API em produção. O contrato de Microsoft Cloud permanece com suporte no programa de parceiro CSP. No entanto, os parceiros são aconselhados a começar a migrar para o contrato do cliente da Microsoft. As novas compras e as alterações na contagem de estações para assinaturas existentes exigirão a confirmação do parceiro do contrato do cliente da Microsoft ou do contrato de Microsoft Cloud. Certas ofertas novas (por exemplo, o novo plano do Azure) exigirão a confirmação do contrato do cliente da Microsoft.|
|31 de janeiro de 2020|Contrato de Microsoft Cloud removido da produção|O contrato de Microsoft Cloud não é mais aceito no programa de parceiro CSP. As novas compras e as alterações na contagem de estações para assinaturas existentes exigirão que o parceiro forneça a confirmação do contrato com o cliente da Microsoft. Esse requisito se aplica a novos clientes e clientes existentes que podem ter aceitado anteriormente o contrato de Microsoft Cloud.|

## <a name="access-microsoft-customer-agreement-template"></a>Acessar o modelo de contrato do cliente Microsoft
Os parceiros podem baixar manualmente a versão mais recente do modelo de contrato do cliente da Microsoft [aqui](https://aka.ms/customeragreement). Observe que o contrato do cliente da Microsoft é específico ao país. Ao solicitar o modelo de contrato do cliente da Microsoft, certifique-se de selecionar o país correto com base no local do cliente. 

## <a name="confirm-customer-acceptance-using-partner-center-apisdk"></a>Confirmar a aceitação do cliente usando a API/SDK do Partner Center
Os parceiros podem usar a API/SDK do Partner Center para confirmar a aceitação do cliente do contrato do cliente da Microsoft. Para obter detalhes sobre a API/SDK, consulte:

- [Obter metadados do Contrato de Cliente da Microsoft](https://docs.microsoft.com/partner-center/develop/get-customer-agreement-metadata)

- [Confirmar a aceitação do cliente do Contrato de Cliente da Microsoft](https://docs.microsoft.com/partner-center/develop/confirm-customer-consent-customer-agreement)

- [Obter a confirmação da aceitação do cliente do Contrato de Cliente da Microsoft](https://docs.microsoft.com/partner-center/develop/get-confirmation-of-customer-agreement)

- [Obter um link de download para o modelo do Contrato de Cliente da Microsoft](https://docs.microsoft.com/partner-center/develop/download-customer-agreement-template)


## <a name="confirm-customer-acceptance-in-partner-center"></a>Confirmar a aceitação do cliente no Partner Center
Os parceiros podem confirmar a aceitação do cliente do contrato de cliente da Microsoft no Partner Center para novos clientes e clientes existentes.

### <a name="confirm-customer-acceptance-for-new-customers"></a>Confirmar a aceitação do cliente para novos clientes

Ao criar um novo locatário do cliente no Partner Center, use as etapas a seguir para confirmar a aceitação do cliente do contrato do cliente da Microsoft. Você deve ser um agente de administração ou um agente de vendas para executar essas etapas.

1. Selecione **Clientes**e então **Novo cliente**.

2. Em **informações da conta**, insira informações para a empresa e seu contato principal.

3. Em **contrato da Microsoft**, selecione o **Contrato do Cliente Microsoft**.

4. Em **Data de aceitação do contrato**, insira a data apropriada. Você não pode definir isso como uma data futura.

5. Verifique se as informações de contato do usuário primário exibidas estão corretas. Se isso não estiver correto, selecione **Atualizar** e insira o **Nome**, **Sobrenome**, **E-mail** e **Número de telefone** (opcional) da pessoa que aceitou o contrato.

6. Selecione **Avançar** para continuar com as etapas restantes para criar o locatário do cliente.

![Novo cliente](images/mcua1.png)

### <a name="confirm-customer-acceptance-for-existing-customers"></a>Confirmar a aceitação do cliente para clientes existentes

Você deve ser um Agente administrativo ou Agente de vendas para fazer isso:

1. Selecione **Clientes**. Localize e selecione o cliente.

2. Selecione **Informações da Conta**.

3. Em **Contrato de Cliente da Microsoft**, selecione **Atualizar**.

4. Insira o **Nome**, **Sobrenome**, **E-mail** e **Número de telefone** (opcional) do usuário que aceitou o contrato. Em **Data de aceitação do contrato**, insira a data apropriada. Você não pode definir isso como uma data futura.

5. Selecione **Salvar** e continue.

![Cliente existente](images/mcua2.png)

### <a name="retrieve-confirmation-of-customer-acceptance"></a>Recuperar confirmação de aceitação do cliente

Você pode recuperar a confirmação de que um cliente existente aceitou o contrato de cliente da Microsoft usando as etapas a seguir. Você deve ser um Agente administrativo ou Agente de vendas para fazer isso.

1. Selecione **Clientes** e então localize e selecione o cliente que você deseja ver.

2. Selecione **Informações da Conta**.

3. Em **contrato de cliente da Microsoft**, veja se a confirmação tem ou não foi fornecida por este cliente.
