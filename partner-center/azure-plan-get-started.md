---
title: Comece a sua mudança para o plano do Azure
description: Saiba o que você e os seus clientes precisam saber sobre como usar o plano pago conforme o uso do Azure, incluindo as primeiras etapas, as precauções de segurança e como começar.
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
author: amitravat
ms.author: amrava
ms.custom: SEOAPR.20
Keywords: Azure, plano do Azure, comprar assinaturas, assinaturas
ms.localizationpriority: High
ms.date: 12/02/2019
ms.openlocfilehash: 08d5048fdfb2a6032ee2e5ec8f0417a106fbf5c7
ms.sourcegitcommit: 6d45415908711cd0e28aeb19756b036274dcd326
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2020
ms.locfileid: "86390403"
---
# <a name="begin-using-pay-as-you-go-rates-with-the-azure-plan"></a>Comece a usar tarifas pagas conforme o uso com o plano do Azure

A Microsoft introduziu uma nova experiência de comércio no Partner Center.  Com essa nova experiência de comércio, os parceiros terão acesso aos serviços do Azure com tarifas pagas conforme o uso para clientes sob o Contrato de Cliente da Microsoft.

Este plano simplifica a experiência de compra – você pode ter várias assinaturas do Azure em um único plano do Azure. Você não precisa mais enviar um pedido separado por assinatura do Azure. E, nesta nova experiência de comércio para o Azure, nós nos alinhamos a um único princípio de preço global, permitindo aos parceiros CSP oferecer o Azure com os preços publicados.

As necessidades de transformação digital de nossos clientes exigem novas habilidades dos parceiros. Muitos clientes procuram parceiros que forneçam serviços além da transação a fim de tornar o percurso da nuvem mais suave e ajudar a consumir os serviços do Azure com eficiência. Os parceiros da Microsoft desempenham uma função fundamental em todos os estágios do ciclo de vida do cliente. Esses tipos de serviços de parceiros têm natureza contínua e incluem o monitoramento de estado do Azure, o gerenciamento de políticas e governança, o ajuste fino das configurações e instalações, o suporte técnico e uma série de outros serviços. Eles exigem que o parceiro esteja intimamente familiarizado com o ambiente do Azure do cliente e tenha governança e controle adequados e contínuos sobre os recursos subjacentes que gerenciam. Os parceiros de cobrança que fornecerem esse gerenciamento de operações de nuvem 24x7 estarão qualificados para um **Crédito ganho pelo parceiro para serviços gerenciados** por esse trabalho.

## <a name="make-sure-your-customers-have-signed-the-microsoft-customer-agreement"></a>Verifique se os clientes assinaram o Contrato de Cliente da Microsoft

Desde 1º de outubro de 2019, o Contrato de Cliente da Microsoft – um contrato permanente que simplifica e agiliza a experiência de compra do cliente com um processo totalmente digital – está disponível. Todos os clientes que desejam aproveitar a nova experiência de comércio no CSP para o Azure devem assinar o Contrato de Cliente da Microsoft.

Os parceiros que quiserem negociar no novo plano do Azure e fazer uma nova solicitação devem confirmar a aceitação do Contrato de Cliente da Microsoft usando o Painel do Partner Center e a API em produção.

A partir de 1º de fevereiro de 2020, o Contrato de Cliente da Microsoft atual será removido do programa CSP. Em seguida, a confirmação (atestado) do parceiro de que o cliente aceitou o novo Contrato de Cliente da Microsoft será obrigatória para todas as outras ofertas, incluindo o Microsoft 365, o Dynamics 365 e o Azure existente. Os parceiros no CSP não poderão fazer um novo pedido para o cliente sem o atestado do Contrato de Cliente da Microsoft.

Para todos os detalhes, leia [Confirmar a aceitação pelo cliente do Contrato de Cliente da Microsoft](confirm-customer-agreement.md)

## <a name="security-and-access-control-practices"></a>Práticas de segurança e controle de acesso

Para ajudar a proteger parceiros e clientes, estamos introduzindo um conjunto de requisitos de segurança obrigatórios para consultores, fornecedores do painel de controle e parceiros que participam do programa de Provedor de Soluções na Nuvem.

Os parceiros que não implementarem os requisitos de segurança obrigatórios não poderão fazer transações no programa de Provedor de Soluções na Nuvem nem gerenciar locatários de clientes que utilizam direitos de administrador delegado, pois esses requisitos são impostos. Estamos no processo de estabelecer uma data de imposição técnica para os requisitos e notificaremos a data aos parceiros com informações detalhadas.

## <a name="actions-to-take-to-implement-mfa"></a>Ações a serem tomadas para implementar o MFA

Considerando a natureza altamente privilegiada de um parceiro, precisamos garantir que cada usuário tenha um desafio de MFA para cada autenticação única. Para fazer isso, devemos adotar uma das seguintes opções:

- Implementar o Azure AD Premium e garantir a imposição da MFA (autenticação multifator) para cada usuário
- Implementar os [padrões de segurança do Azure AD](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-security-defaults)
- Implementar a solução de terceiros e garantir que a MFA seja imposta para cada usuário

A partir de 1º de agosto de 2019, todos os parceiros são obrigados a impor a autenticação multifator a todos os usuários, incluindo as contas de serviço, em seu locatário de parceiro. Informações detalhadas sobre esses requisitos de segurança podem ser encontradas em [Requisitos de segurança de parceiros](https://docs.microsoft.com/partner-center/partner-security-requirements).

A Microsoft recomenda que os parceiros usem o RBAC de forma adequada, seguindo as melhores práticas habilitadas por meio dos [Recursos do Azure Active Directory Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).

## <a name="read-more-about-the-azure-plan"></a>Leia mais sobre o plano do Azure

- [Comprar o plano do Azure](purchase-azure-plan.md)

- [Comparar as ofertas do Azure](compare-azure-offers.md)

- [Crédito ganho pelo parceiro – visão geral](partner-earned-credit.md)

- Os cálculos do PEC (crédito ganho pelo parceiro) e as funções e permissões qualificadas para obter créditos ganhos pelo parceiro estão disponíveis na lista de preços do Painel do Partner Center (requer credenciais).

## <a name="next-steps"></a>Próximas etapas 

- [Como o crédito ganho pelo parceiro é determinado – detalhes](partner-earned-credit-explanation.md)
- [Lista de preços do plano do Azure explicada](azure-plan-price-list.md)
- [Transferir seu cliente para o plano do Azure](azure-plan-transition.md)
- [Gerenciar assinaturas e recursos no âmbito do plano do Azure](azure-plan-manage.md)
- [A lista completa de países/regiões em que o plano do Azure está disponível](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE3QN0x)
