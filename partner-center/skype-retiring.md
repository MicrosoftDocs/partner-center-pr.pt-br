---
title: Migrar algumas assinaturas do Skype for Business
description: Saiba como e quando migrar determinados clientes com assinaturas expiradas do Skype for Business Online Plano 1 para novas versões do Office 365.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: BrentSerbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 06/03/2020
ms.openlocfilehash: 0e8289ad06dbc8a95f5cff22ca386176d6ba65ab
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109854818"
---
# <a name="migrate-skype-for-business-online-plan-1-subscriptions-to-newer-office-365-versions"></a>Migrar assinaturas do Skype for Business Online Plano 1 para versões mais novas do Office 365

**Funções apropriadas:** Agente de vendas

O Plano 1 do Skype for Business Online será retirado, a partir de 1º de agosto de 2018. Após essa data, os clientes não poderão mais adquirir novas assinaturas do Skype for Business Plano 1. As assinaturas existentes não serão renovadas automaticamente quando expirarem, e não haverá uma opção de renovação. Na página de detalhes da assinatura, o status da assinatura do Skype for Business Online Plano 1 foi alterado para "Expira em [data]" de "Renovação automática em [data]".  

Para garantir a continuidade dos clientes, você deve fazer a transição de clientes com assinaturas do Skype for Business Online Plano 1 que vão expirar para uma opção de SKU com suporte, listada abaixo. É recomendável mover clientes para novas assinaturas antes da data de término anual da assinatura para evitar qualquer paralisação de serviço para os clientes. 

>[!NOTE]
>As SKUs do Skype for Business Online Plano 1 comerciais e governamentais estão sendo desativadas.

Se você usar a API (CREST ou Partner Center), encontre as assinaturas que vão expirar avaliando a data de término da assinatura juntamente com a propriedade de renovação automática = Falso. As assinaturas do Skype for Business Online Plano 1 serão definidas como renovação automática=Falso em 1º de setembro de 2018. Você pode mover os clientes para um novo plano a qualquer momento. 

## <a name="skype-for-business-online-plan-1-replacement-plans"></a>Planos de substituição do Skype for Business Online Plano 1

Com os novos planos, seus os clientes podem aproveitar novos recursos e funcionalidades no Office 365. Detalhes de preço são encontrados na lista de preços e oferecem a matriz de lista no Partner Center. 

- Opção 1: Office 365 Enterprise F1
- Opção 2: Microsoft 365 Enterprise F1
- Opção 3: outros planos do Office 365

|**Recurso**    |**Opção 1**   |**Opção 2**   |**Opção 3**   |
|:-----------------|:-----------------|:-------------|:------------|
|Obtenha todos os recursos incluídos no Skype for Business Online Plano 1|Sim   |Sim   |Sim   |
|Mensagens Instantâneas e presença |Sim   |Sim   |Sim   |
|Áudio e vídeo ponto a ponto sobre IP|Sim   |Sim   |Sim   
|Participar de reuniões como um usuário autenticado| Sim   |Sim   |Sim   |

## <a name="transition-customers-to-new-product-plans"></a>Transição dos clientes para novos planos do produto

A Microsoft oferece continuamente novos produtos e serviços para nossos parceiros. Nesses casos, você pode precisar fazer o upgrade dos clientes para novos serviços ou migrar as assinaturas de SKUs que serão encerradas em breve. A migração dos clientes de SKUs desativadas para as mais recentes requer as seguintes etapas:

- Comprar a nova assinatura
- Reatribuir as licenças de usuário atuais
- Cancelar a assinatura antiga

### <a name="migrate-your-customers-to-new-plans"></a>Migrar seus clientes para novos planos

1. Para comprar a nova assinatura, no **menu Partner Center**, selecione **Clientes**, selecione o cliente que você deseja mover e, em seguida, selecione **Adicionar assinaturas**.

2. Selecione a assinatura que deseja comprar no catálogo (nesse caso, uma das opções acima), insira o número de licenças e selecione **Enviar**. 

Agora, seu cliente deve ter assinaturas antigas e novas, a assinatura antiga do Plano 1 do Skype for Business Online e a nova assinatura de "destino", por exemplo, Opção 1 – Office 365 Enterprise F1.

3. Para reatribuir as licenças dos usuários do cliente, no menu **Partner Center,** selecione Clientes **,** selecione o cliente que você está movendo e, em seguida, selecione Usuários **e licenças**. A página Usuários e Licenças do cliente é aberta.

4. Para reatribuir a licença do usuário, selecione o usuário a ser reatribuído e selecione **Gerenciar licenças**.

5. Na página **Gerenciar licenças**, desmarque a caixa de seleção da licença do Skype for Business Online Plano 1 e selecione um novo plano de serviço para a assinatura para a qual o cliente está mudando.

6. Selecione **Enviar**. Uma página de confirmação lista as novas atribuições de licença. Continue esse mesmo processo para outros usuários que precisam de atribuições de licença.

Depois de migrar a licença do usuário para o novo serviço, você pode cancelar com segurança a assinatura desativada no nível do cliente.

7. No menu **Partner Center,** selecione **Clientes**. Selecione o cliente cuja assinatura você está cancelando.

8. Na página de detalhe da assinatura, defina o status da assinatura como **Suspensa**.

9. Selecione **Enviar.**

A assinatura antiga será suspensa e a nova assinatura será ativada. A assinatura suspensa será desprovisionada automaticamente após 120 dias. O cliente não pagará custos adicionais pela assinatura antiga.

## <a name="next-steps"></a>Próximas etapas

- [Consultores: criar e enviar um convite de avaliação para os clientes experimentarem o Office 365](advisors-create-a-trial-invitation.md)
- [Consultores: crie sua base de clientes com convites de avaliação do Office 365 e ofertas de compra](advisors-build-your-business.md)
- [Consultores: Criar uma oferta de compra](advisor-create-a-purchase-offer.md)
