---
title: Confirmar a aceitação do cliente do contrato do cliente da Microsoft | Centro de parceiros
ms.topic: article
ms.date: 04/16/2019
Description: Como parceiro, você precisa obter a aceitação do cliente do contrato do cliente da Microsoft antes de poder solicitar produtos e serviços da Microsoft para esse cliente. Para ajudar melhor os parceiros a atender aos requisitos de conformidade, a Microsoft solicita que os parceiros confirmem a aceitação fornecendo determinados detalhes sobre a pessoa que aceitou o contrato.
author: LauraBrenner
ms.author: labrenne
keywords: cliente, clientes, consentimento, MCA, contrato de Microsoft Cloud, contrato de cliente da Microsoft, modelos de contrato de cliente
ms.localizationpriority: medium
ms.openlocfilehash: 6ca8eb3acdee0114f01dbd5952e9c092859147a2
ms.sourcegitcommit: ee722dc2b9d82557d273738b64cec6d8cb435084
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "68681752"
---
# <a name="confirm-customer-acceptance-of-the-microsoft-customer-agreement-preview"></a>Confirmar a aceitação do cliente do contrato do cliente da Microsoft (versão prévia)

Atualmente, antes que um parceiro CSP possa fazer o pedido em nome de um cliente, o cliente deve aceitar e assinar o **contrato de Microsoft Cloud**aplicável. Em seguida, o parceiro deve confirmar a aceitação do cliente, fornecendo informações sobre o Assinante para a Microsoft. Se um cliente não confirmar sua aceitação do contrato de Microsoft Cloud:
- Você não conseguirá criar novos pedidos para esse cliente.
- Você não poderá alterar a contagem de estações de assinaturas baseadas em estação existentes para esse cliente.

Para obter detalhes sobre como confirmar a aceitação de um cliente do contrato de Microsoft Cloud usando o painel do Partner Center ou a API, confira [confirmar a aceitação do cliente do contrato de Microsoft Cloud](confirm-consent.md).

Em 1º de outubro de 2019, a Microsoft apresentará o **contrato do cliente da Microsoft** ao programa CSP para substituir o contrato de Microsoft Cloud. Para facilitar a migração dos parceiros para o novo contrato, o contrato de Microsoft Cloud atual terá suporte no programa CSP até 31 de janeiro de 2019. Para obter mais detalhes do cronograma, consulte a tabela a seguir:

| Date | Marco | Detalhes |
|------------|------------|--------------------------------|
|1º de agosto de 2019|Visualização de UX disponível na área restrita|Os parceiros podem confirmar a aceitação do cliente do contrato de cliente da Microsoft usando o painel do Partner Center no ambiente de área restrita do CSP. Os parceiros com acesso ao ambiente de área restrita do CSP visualizam as alterações na experiência do usuário. Parceiros sem acesso à área restrita podem aprender sobre as alterações neste tópico.|
|02 de setembro de 2019|A visualização da API está disponível na área restrita.|O parceiro pode confirmar a aceitação do cliente do contrato do cliente da Microsoft usando a API do Partner Center no ambiente de área restrita do CSP. Os parceiros de API podem usar essa oportunidade para visualizar as alterações de API e começar a trabalhar na integração de API para dar suporte ao novo contrato.|
|1º de outubro de 2019|Contrato de cliente da Microsoft disponível em produção|A Microsoft apresenta o contrato do cliente da Microsoft ao programa CSP para substituir o contrato de Microsoft Cloud. Os parceiros podem confirmar a aceitação do cliente do contrato de cliente da Microsoft usando o painel do Partner Center e a API em produção. O contrato de Microsoft Cloud permanece com suporte no programa de parceiro CSP. No entanto, os parceiros são aconselhados a começar a migrar para o contrato do cliente da Microsoft. As novas compras e as alterações na contagem de estações para assinaturas existentes exigirão a confirmação do parceiro do contrato do cliente da Microsoft ou do contrato de Microsoft Cloud. Certas ofertas novas (por exemplo, o novo plano do Azure) exigirão a confirmação do contrato do cliente da Microsoft.|
|31 de janeiro de 2019|Contrato de Microsoft Cloud removido da produção|O contrato de Microsoft Cloud não é mais aceito no programa de parceiro CSP. As novas compras e as alterações na contagem de estações para assinaturas existentes exigirão que o parceiro forneça a confirmação do contrato com o cliente da Microsoft. Esse requisito se aplica a novos clientes e clientes existentes que podem ter aceitado anteriormente o contrato de Microsoft Cloud.|


## <a name="confirm-customer-acceptance-for-new-customers"></a>Confirmar a aceitação do cliente para novos clientes

Ao criar um novo locatário do cliente no Partner Center, use as etapas a seguir para confirmar a aceitação do cliente do contrato do cliente da Microsoft. Você deve ser um agente de administração ou um agente de vendas para executar essas etapas.

1. Selecione **Clientes**e então **Novo cliente**.

2. Em **informações da conta**, insira informações para a empresa e seu contato principal.

3. Em **contrato da Microsoft**, selecione o **contrato do cliente da Microsoft**.

4. Em **Data de aceitação do contrato**, insira a data apropriada. Você não pode definir isso como uma data futura.

5. Verifique se as informações de contato do usuário primário exibidas estão corretas. Se não estiver correto, selecione **Atualizar** e insira o **nome**, o **sobrenome**, o **endereço de email**e o **número de telefone** (opcional) da pessoa que aceitou o contrato.

6. Selecione **Avançar** para continuar com as etapas restantes para criar o locatário do cliente.

![Novo cliente](images/mcua1.png)

## <a name="confirm-customer-acceptance-for-existing-customers"></a>Confirmar a aceitação do cliente para clientes existentes

Você deve ser um agente de administração ou um agente de vendas para fazer isso:

1. Selecione **clientes**. Localize e selecione o cliente.

2. Selecione **informações da conta**.

3. Em **contrato de cliente da Microsoft**, selecione **Atualizar**.

4. Insira o **nome**, **sobrenome**, endereço de **email**e número de **telefone** (opcional) da pessoa que aceitou o contrato. Em **Data de aceitação do contrato**, insira a data apropriada. Você não pode definir isso como uma data futura.

5. Selecione **salvar** e continuar.

![Cliente existente](images/mcua2.png)

## <a name="retrieve-confirmation-of-customer-acceptance"></a>Recuperar confirmação de aceitação do cliente

Você pode recuperar a confirmação de que um cliente existente aceitou o contrato de cliente da Microsoft usando as etapas a seguir. Você deve ser um Agente administrativo ou Agente de vendas para fazer isso.

1. Selecione **Clientes** e então localize e selecione o cliente que você deseja ver.

2. Selecione **informações da conta**.

3. Em **contrato de nuvem da Microsoft**, veja se a confirmação tem ou não foi fornecida por este cliente.


