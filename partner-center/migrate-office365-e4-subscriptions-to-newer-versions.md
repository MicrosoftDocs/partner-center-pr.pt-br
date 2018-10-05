---
title: Migrar assinaturas do Office 365 E4 para versões mais recentes do Office 365 | Partner Center
description: Edições do Microsoft Office 365 Enterprise E4 estarão desativadas a partir de 7 de abril de 2017. Saiba como migrar suas assinaturas de cliente para versões mais recentes do Office 365.
author: MaggiePucciEvans
ms.localizationpriority: medium
ms.openlocfilehash: e6efcc3227f426a9b83c7579534e0b6ad68188da
ms.sourcegitcommit: 5b720c2ad126ec52564ad5264596ca1cf6a12489
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/05/2018
ms.locfileid: "4377708"
---
# <a name="migrate-office-365-e4-subscriptions-to-newer-office-365-versions"></a>Migrar inscrições do Office 365 E4 para versões do Office 365 mais recentes

**Aplicável a**

-  Partner Center

O plano do Office 365 Enterprise E4 está desativado desde 7 de abril de 2017. Você não pode comprar novas assinaturas do Office 365 E4 após essa data, e assinaturas E4 existentes não serão renovadas automaticamente quando expirarem.

Quando as assinaturas E4 terminarem, elas serão canceladas. Para garantir a continuidade dos clientes, você deve fazer a transição de clientes com assinaturas E4 vencidas para uma opção de SKU com suporte, listada abaixo. É recomendável mover os clientes para novas assinaturas antes da data de término anual da assinatura, para evitar possíveis interrupções de serviço para os clientes. 

> [!NOTE]  
>  Tanto o Office 365 Enterprise E4 comercial quanto o governamental de SKUs está desativados.
 
Na página de detalhes da assinatura, o status da assinatura E4 foi alterado para "Expira em [data]" de "Renovação automática em [data]". 

Se você usar a API (CREST ou Partner Center), você pode descobrir assinaturas vencidas avaliando a data de término da assinatura juntamente com a propriedade de renovação automática = Falso. 

As inscrições do E4 serão definidas para renovação automática=Falso em 7 de abril de 2017. Você pode mover os clientes para um novo plano a qualquer momento. 

## <a name="office-365-enterprise-e4-edition-replacement-plans"></a>Planos de substituição da edição do Office 365 E4 Enterprise

Você pode optar por manter a mesma funcionalidade com E4 ou deixar seus clientes tirarem vantagem de novos recursos e funcionalidades no Office 365 e Skype for Business Online. Detalhes de preço são encontrados na lista de preços e oferecem a matriz de lista no Partner Center. Secure Product Enterprise E3 ou Secure Productive Enterprise E5 podem ser substituídos nas opções a seguir para Office 365 Enterprise E3 ou Office 365 Enterprise E5, respectivamente.

- Opção 1: Office 365 Enterprise E5

- Opção 2: Office 365 Enterprise E3 + Skype for Business Cloud PBX

- Opção 3: Office 365 Enterprise E3 + Skype for Business Plus CAL (preço e paridade funcional com E4)

- Opção 4: Office 365 Enterprise E3


| Recurso | Opção 1 | Opção 2 | Opção 3 | Opção 4 |
| :---    | :------: |   :---:  |   :---:  |   :---:  |
| Obter todos os recursos incluídos no Office 365 Enterprise E4? | Sim | Sim | Sim | Não |
| Números de telefone gerenciados no Office 365? | Sim | Sim | Não | Não |
| Números de telefone gerenciado no local e no Office 365 (implantação híbrida)? | Sim | Sim | Não | Não |
| Opção de adicionar um plano de chamada de voz PSTN? | Sim | Sim | Não | Não |
| Conferência por PSTN? | Sim | Não | Não | Não |
| Ferramentas avançadas de colaboração, análises e segurança? | Sim | Não | Não | Não |
| Visualizações de relatórios, painéis e dados interativos? | Sim | Não | Não | Não | 
| Mais controle sobre a segurança dos dados e a conformidade com privacidade interna, transparência e controles de usuário refinados? | Sim | Não | Não | Não | 

## <a name="transition-customers-to-new-product-plans"></a>Transição dos clientes para novos planos do produto

A Microsoft oferece continuamente novos produtos e serviços para nossos parceiros. Nesses casos, você pode precisar fazer o upgrade dos clientes para novos serviços ou migrar as assinaturas de SKUs que serão encerradas em breve. A migração dos clientes de SKUs desativadas para as mais recentes requer as seguintes etapas:

-   Comprar a nova assinatura
-   Reatribuir as licenças de usuário atuais
-   Cancelar a assinatura antiga

Siga estas etapas para migrar a assinatura do Office 365 Enterprise E4 de cliente para uma das opções na tabela acima.

### <a name="step-1---purchase-the-new-subscription"></a>Etapa 1 - Comprar a nova assinatura

1. No menu **Painel**, selecione **Clientes**, selecione o cliente para o qual você deseja fazer a migração e selecione **Adicionar assinaturas**.

2. Selecione a assinatura que deseja comprar no catálogo (nesse caso, uma das opções acima), insira o número de licenças e selecione **Enviar**.

   Seu cliente deve ter agora tanto assinaturas antigas quanto novas, a assinatura do Office 365 Enterprise E4 antiga e a de "alvo" nova, por exemplo, Opção 1 - Office 365 Enterprise E5.

### <a name="step-2---reassign-the-customers-users-licenses"></a>Etapa 2 - Reatribuir licenças dos usuários do cliente

1. No menu **Painel**, selecione **Clientes**, selecione o cliente para o qual deseja fazer a migração e selecione **Usuários e licenças**. A página Usuários e Licenças do cliente será aberta.

2. Para reatribuir licenças de usuário, selecione o usuário a ser reatribuído e selecione **Gerenciar licenças**.

3. Na página **Gerenciar licenças**, desmarque a caixa de seleção da licença do **Office 365 Enterprise E4** e selecione um novo plano de serviço para onde o cliente está movendo a assinatura.

4. Selecione **Enviar**. Uma página de confirmação lista as novas atribuições de licença.

5. Siga as mesmas etapas com outros usuários do cliente que precisam de reatribuição de licença.

Depois de migrar as licenças de usuário para o novo serviço, você pode cancelar com segurança a assinatura desativada no nível superior do cliente.

### <a name="step-3---cancel-the-old-subscription"></a>Etapa 3 - Cancelar a assinatura antiga

1. No menu **Painel**, selecione **Clientes**. Selecione o cliente que você deseja mover e selecione a assinatura que deseja cancelar.

2. Na página de detalhes da assinatura, defina o status da assinatura para **Suspensa**.

3. Selecione **Enviar**.

A assinatura antiga será suspensa e a nova assinatura será ativada. A assinatura suspensa será desprovisionada automaticamente após 120 dias. O cliente não pagará custos adicionais pela assinatura antiga.



 



