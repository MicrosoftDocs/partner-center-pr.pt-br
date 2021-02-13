---
title: Como vender ofertas para clientes educacionais
description: Saiba como criar um cliente educativo e vender ofertas para eles no Partner Center. Inclui a confirmação do status de verificação para o cliente de educação.
ms.topic: how-to
ms.date: 12/17/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: alikhaki
ms.author: alikhaki
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: a101c3d29b947950179ca0ae446f049ccf785bb8
ms.sourcegitcommit: 64b43ad8fb7bb56628450bea06b9cd2606c36b03
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/12/2021
ms.locfileid: "100281315"
---
# <a name="how-to-sell-offers-to-education-customers-and-how-to-create-an-education-customer-in-partner-center"></a>Como vender ofertas para clientes educativos e como criar um cliente de educação no Partner Center


**Funções apropriadas**

- Administrador global
- Agente administrativo
- Agente de vendas

## <a name="create-an-education-customer"></a>Criar um cliente educacional

Este artigo explica como criar um cliente de educação no Partner Center e vender produtos educativos para eles. Ele também aborda como exibir o status de verificação e reenviar a solicitação de verificação, se necessário. As ofertas de educação estão atualmente **disponíveis apenas para serviços baseados em licença** , como Microsoft 365, Dynamics, Intune etc. Ele não está disponível para outros tipos (assinaturas de software, software permanente ou produtos do Azure).

> [!IMPORTANT]
> A Microsoft verifica cada locatário de cliente educativo recém-criado para garantir que eles sejam qualificados para ofertas educacionais.  Certifique-se de inserir as informações necessárias de forma mais precisa e total possível para evitar atrasos no processo de verificação.

1. Conecte-se ao Partner Center.

2. Selecione **clientes** e, em seguida, selecione **Adicionar um cliente**. Selecione **educação** na lista suspensa **qualificações especiais** .  Preencha o restante das informações da conta, conforme necessário.  Os campos de chave que auxiliam o processo de verificação incluem:

   - **Nome da empresa**: Insira o nome da entidade legal – obrigatório para verificação
   - **País/região e linhas de endereço**: Insira o endereço para correspondência de entidade completa – necessário para verificação
   - **Endereço de email**: Insira o email de propriedade da entidade – não é um email gratuito ou on.Microsoft.com – necessário para verificação
   - **Informações de contato do cliente**: esses detalhes serão usados como parte do processo de verificação
   - **Nome de domínio primário**: usado para criar a conta e os endereços de email do cliente.  Escolha um nome semelhante ao nome da empresa sem espaços ou caracteres especiais.  Esse nome não pode ser alterado posteriormente.

3. Quando tiver terminado, selecione **examinar**.

   :::image type="content" source="images/eduaccountinfo.png" alt-text="Conta do cliente de educação":::

4. Depois de confirmar a **revisão**, você receberá um status de **inanálise** se as informações enviadas forem válidas. 

    :::image type="content" source="images/edu/create-review.png" alt-text="Conta do cliente de educação em análise"lightbox="images/edu/create-review-expanded.png":::

### <a name="confirm-your-education-customers-verification-status"></a>Confirmar o status de verificação do seu cliente de educação

Na página **conta** do cliente, consulte **status de qualificação especial**.
Exemplos de status:

- Se o cliente tiver passado a verificação: educação

   :::image type="content" source="images/edupassedvetting.png" alt-text="A verificação da educação foi bem-sucedida":::

- Se o cliente não passou na verificação: não é um cliente de educação

   :::image type="content" source="images/edu/fail-reason.png" alt-text="A verificação da educação não foi bem-sucedida" lightbox="images/edu/fail-reason-expanded.png":::

- Se o cliente não tiver sido marcado como um cliente de educação: nenhum

   :::image type="content" source="images/edu/account-one.png" alt-text="o cliente de educação não está marcado como tal" lightbox="images/edu/account-one-expanded.png":::

- Se o cliente estiver em análise como um cliente de educação: em análise

    :::image type="content" source="images/edu/in-review.png" alt-text="o cliente de educação está em análise" lightbox="images/edu/in-review-expanded.png":::

## <a name="correct-the-customer-account-info-and-resubmit-for-verification"></a>Corrigir as informações da conta do cliente e reenviar para verificação

Se o cliente falhar na verificação inicial, agora você poderá corrigir as informações e reenviá-las.

### <a name="correct-the-customer-account-information"></a>Corrigir as informações da conta do cliente

Você deve ter privilégios de administrador global para atualizar as informações do cliente. Você atualiza as informações no portal do Office 365 porque esses dados não podem ser atualizados no portal do Partner Center.

1. Na página **conta** , você verá informações informando que a qualificação do cliente é considerada "não é um cliente educacional".

2. Atualize o navegador para redefinir a página. Haverá um botão de **atualização** e o **status de qualificações especiais** será definido como **nenhum**.

3. Selecione **Atualizar**. Na página **Gerenciamento de serviços** , selecione **Office 365**.

4. Você será redirecionado para o centro de administração do Office 365 em uma nova guia do seu navegador. Talvez seja solicitado que você entre com suas credenciais.

5. Selecione **Configurações**.

6. Selecione a guia **perfil da organização** na parte superior da tela e, em seguida, informações da **organização**. Agora você pode atualizar os detalhes do cliente.

7. Selecione **salvar alterações** na parte inferior da barra lateral.  

### <a name="resubmit-for-verification"></a>Reenviar para verificação

1. Navegue até a guia do centro do parceiro e para a página **conta** do cliente. Atualize o navegador e verifique se a página da empresa foi atualizada para as novas informações. Selecione o botão **Atualizar** para solicitar a nova verificação de educação.

2. Se os detalhes atualizados do cliente estiverem qualificados para ofertas educacionais, você verá as **qualificações especiais** atualizadas para **educação**. Se você ainda **não vir um cliente educativo**, entre em contato com o suporte para verificação manual.

## <a name="next-steps"></a>Próximas etapas

- [Vender para setores especializados](get-special-pricing-for-offers.md)

- [Adicionar um novo cliente](add-a-new-customer.md)

- [Vender assinaturas do Minecraft: Education Edition para clientes da área de educação](minecraft-subscriptions.md)
