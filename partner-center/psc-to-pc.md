---
title: Migrar do Partner Sales Connect (PSC)
ms.topic: article
ms.date: 08/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como os parceiros da Microsoft podem migrar do PSC (Partner Sales Connect) para o Partner Center e criar ou gerenciar as negociações enviadas pelos vendedores da Microsoft.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 8fa06bb0aaecb5f2564c2baab9d7a2c6ac6f0f1d
ms.sourcegitcommit: 3502f32da07a3db8b865d7f32416eeb8cfd5502c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "90082514"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>Guia para a venda em conjunto no Partner Center (PC) para parceiros migrando do PSC (Partner Sales Connect)

**Aplica-se a**

- Partner Center

**Funções apropriadas**

- Administrador de conta
- Administrador de indicações
- Vendedor do PSC (Partner Sales Connect)
- Administrador do PSC (Partner Sales Connect)
- Gerente de negociações do Partner Sales Connect (PSC)

Como você sabe, sua empresa perderá o acesso ao PSC após 31 de dezembro de 2020. No entanto, você encontrará tudo o que deseja fazer para criar negociações de venda, gerenciar seus negócios e agir sobre as negociações enviadas pelos vendedores da Microsoft para você no Partner Center. No entanto, haverá diferenças, e as diretrizes a seguir ajudarão a fazer sua transição para o Partner Center mais suave e direto.

>[!Important]
> Se você estiver aqui porque viu uma faixa no PSC sobre a migração, você está no lugar certo. Este guia não é aplicável à SA (avaliação de solução) e a parceiros de IOT OEM que gerenciam suas negociações no PSC.

## <a name="before-you-move-things-you-need-to-know"></a>Antes de mover, as coisas que você precisa saber

### <a name="if-you-are-psc-admin"></a>Se você for administrador do PSC

- Você precisa de um email de trabalho para fazer logon no [Partner Center](https://partner.microsoft.com/).
- Configure sua conta com a ajuda do [administrador da conta](https://docs.microsoft.com/partner-center/permissions-overview)do Partner Center.
- Saiba como fazer uma venda conjunta no Partner Center lendo este documento.
- Configure contas de usuário no Partner Center para todos os usuários do PSC (funções de administrador, gerente de negociações e vendedor) e atribua a eles [funções de administrador de referência](https://docs.microsoft.com/partner-center/permissions-overview).

>[!Important]
> Verifique se a ID de MPN mostrada na faixa PSC está disponível na lista de locais MPN no Partner Center. Você pode verificar isso no Partner Center acessando configurações de conta e [locais](https://docs.microsoft.com/partner-center/manage-locations) sob isso para localizar a lista de todos os MPNs associados à conta do Partner Center.

### <a name="if-you-are-psc-deal-manager-or-seller"></a>Se você for o PSC, gerente de negócios ou vendedor

- Você precisa de um email de trabalho para entrar no [Partner Center](https://partner.microsoft.com/).
- Se você estiver usando uma conta que não seja de trabalho no PSC ou seu email de trabalho for para uma empresa diferente da empresa parceira, entre em contato com o administrador do PSC para obter ajuda de configuração de conta.
- Verifique com o administrador do PSC se a configuração da sua conta do Partner Center está concluída, independentemente da conta que você usa para fazer logon no PSC.
- Verifique se você tem acesso ao Partner Center e à seção referências.
- Leia este documento para entender os fluxos de trabalho e as alterações no Partner Center.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>Como administrador no PSC, estas são as próximas etapas

Se você não vir a guia Referências:

- O [administrador global](https://docs.microsoft.com/partner-center/permissions-overview) da sua empresa pode conceder acesso à guia referências. Para localizar seu administrador global, vá para configurações de parceiro no ícone de engrenagem na parte superior direita da central de parceiros. Selecione a página Gerenciamento de usuários no segundo nível da barra de navegação à esquerda. Clique na lista suspensa que mostra "todos os usuários" no canto superior direito da página e altere para "administradores globais". A página exibirá todos os administradores globais com suas respectivas IDs de email. Entre em contato com eles para obter acesso "administrador de referência" para sua conta corporativa.

>[!Important]
> Se sua função estiver gerenciando apenas usuários no PSC, você poderá obter a função de [administrador da conta](https://docs.microsoft.com/partner-center/permissions-overview#manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant) no Partner Center. Se sua função também incluir o gerenciamento de oportunidades de venda conjunta, você deverá obter a função de [administrador de referências](https://docs.microsoft.com/partner-center/permissions-overview#manage-referrals) . Além disso, indique um líder de gerenciamento de alterações entre os administradores do PSC para trabalhar com o administrador da conta do Partner Center, em vez de todos os administradores do PSC que estão chegando aos administradores da conta no PC individualmente.

 :::image type="content" source="images/pscmigration/accountadmin.png" alt-text="Imagem que mostra os administradores de conta na página de gerenciamento de usuário configurações de parceiro.":::

- Vá para a guia referências no painel de navegação à esquerda e verifique se você pode acessar as páginas.

>[!Note]
> Talvez você precise sair do Partner Center e entrar novamente para atualizar suas credenciais para acessar as páginas de referências.

Depois de configurar sua conta no Partner Center,

- Convide todos os usuários que têm uma função "gerente de negociações" ou "vendedor" no PSC para o Partner Center como uma próxima etapa.
- O [administrador da conta](https://docs.microsoft.com/partner-center/permissions-overview#manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant) que ajudou você com acesso às referências pode convidar todos os usuários.
- Ao convidar os usuários, peça ao administrador da conta para atribuir a função de [administrador de referência](https://docs.microsoft.com/partner-center/permissions-overview#manage-referrals) a eles.
- Alguns dos seus usuários do PSC podem estar usando uma conta que não seja de trabalho ou uma conta de um domínio diferente daquele que você está usando no Partner Center. Todos esses usuários precisam entrar no Partner Center usando sua conta de trabalho anexada ao seu locatário do Azure AD. Seu [administrador global](https://docs.microsoft.com/partner-center/permissions-overview#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) pode ajudar com isso. Para localizar seu administrador global, vá para configurações de parceiro no ícone de engrenagem na parte superior direita da central de parceiros. Clique na página Gerenciamento de usuários no segundo nível da barra de navegação à esquerda. Clique na lista suspensa que mostra "todos os usuários" no canto superior direito da página e altere para "administradores globais".
- O administrador global pode criar uma nova conta de usuário no seu locatário do Azure AD ou atribuir acesso de usuário convidado aos outros usuários da conta de domínio.
- Depois que as contas são configuradas para todos os gerentes de negócios e usuários do PSC, elas precisam entrar no Partner Center, ir para a guia referência no painel de navegação esquerdo e verificar se elas podem ver a página referências.

Se sua empresa tiver um PDM – quando sua conta do Partner Center estiver configurada e os usuários tiverem migrado e tiverem funções e permissões, você poderá mover suas atividades de vendas para o Partner Center. Informe ao PDM para fazer o comutador em vez de esperar até o prazo de conclusão da migração, o que permitirá que todas as suas novas negociações fluam para o Partner Center.
>[!Note]
>Depois de fazer essa opção, você só poderá agir sobre as negociações ativas existentes no PSC. Você não pode criar novas negociações nem receber nenhuma medida de vendedores da Microsoft no PSC.

Se sua empresa não tiver um PDM, verifique se todas as contas de usuário estão configuradas e verificadas por todos os usuários. Você será notificado por meio de um email e uma faixa no PSC em relação à data exata quando puder começar a trabalhar com a venda no Partner Center. Lembre-se de que você ainda precisará gerenciar as negociações ativas existentes no PSC.

>[!Important]
>As negociações ativas não serão migradas para o PC. Você tem até 31 de dezembro de 2020 para fechar e registrar as negociações.

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>Próximas etapas para administradores do PSC, gerentes de negócios do PSC e vendedores do PSC

Saiba como fazer uma venda conjunta no Partner Center.
Esta é uma etapa importante, que ajudará você a se preparar para a venda em conjunto no Partner Center. Entenda os fluxos de trabalho e as alterações no Partner Center para que você possa realmente vender do dia um. Comece lendo este documento completamente. Um bom conjunto de recursos também está disponível na [Galeria de experiência de venda conjunta](https://aka.ms/cosellexperience).

## <a name="major-differences-between-psc-and-pc-workflows"></a>Principais diferenças entre os fluxos de trabalho do PSC e do PC

|**Cenário**|**Conexão de vendas do parceiro**|**Partner Center**|
|-----|:-----|:-----|
|Funções de usuário|O PSC tem funções de administrador, gerente de negociações e vendedor.|O PC tem apenas a função [administrador de referências](https://docs.microsoft.com/partner-center/permissions-overview#manage-referrals) que fornece permissão de leitura e gravação para todas as negociações.|
|Convidando a Microsoft em um negócio de venda conjunta|Iniciado pelo vendedor da Microsoft, não há nenhuma pergunta explícita pelo parceiro.|O parceiro terá que fazer uma [solicitação explícita](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#add-solutions) se uma ajuda do Microsoft seller for necessária para um negócio. O vendedor da Microsoft tem uma opção para recusar a solicitação.|
|Expiry|Não há nenhum conceito de expiração de uma negociação.|Os acordos de entrada do parceiro expiram em 14 dias se não forem aceitos pelo parceiro. O mesmo é o caso de negócios de saída de parceiros onde eles podem entrar no estado expirado se o vendedor da Microsoft não agir em 14 dias.|
|Detalhes do vendedor da Microsoft|Visível assim que um acordo é criado.|Os detalhes do vendedor da Microsoft serão compartilhados com o parceiro somente se o vendedor aceitar explicitamente o convite para a venda de vendas do parceiro.|
|[Pipeline privado](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#types-of-co-sell-opportunities)|Não disponível.|Os parceiros podem compartilhar seus pipelines sem dar visibilidade aos vendedores da Microsoft.|
|Soluções|As soluções que pertencem a apenas uma lista de preços podem ser adicionadas a um negócio.|O parceiro pode adicionar [soluções](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#add-solutions) que pertencem às listas a seguir. a) as soluções de suas próprias soluções b) do catálogo de primeira parte da Microsoft (semelhante à função de negócio de transação no PSC) e c) comercializar soluções de outros parceiros de terceiros (semelhante à função de negócio de ISV no PSC).|
|Atribuição de negociações|Somente o vendedor atribuído pode exibir e agir sobre as negociações.|Os membros da equipe podem ser adicionados a um negócio para especificar as pessoas que trabalham em um negócio, não há nenhum bloqueio de outros administradores de referência de exibir ou agir nessas negociações.|
|Organização do cliente|Entrada de texto de formato livre.|Você pode pesquisar a [organização do cliente](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#select-your-customer) no [banco de dados D&B](https://www.dnb.com/) digitando apenas alguns caracteres. O nome e o endereço legais são preenchidos automaticamente com base na escolha.|
|Contato do cliente|Não obrigatório.|Não obrigatório para compartilhamento de pipeline privado. Necessário se o vendedor da Microsoft for convidado a participar de uma solicitação de venda de uma parceria.|
|API pública|Não disponível.|[API pública](https://docs.microsoft.com/partner/develop/referrals) para gerenciar programaticamente as referências do Partner Center.|

## <a name="psc-and-partner-center-field-mapping"></a>Mapeamento de campos do PSC e do Partner Center

Esta seção apresenta o mapeamento exato de atributos entre o PSC e o Partner Center. Cada tela no PSC é comparada com a exibição relevante na seção oportunidades de venda do Partner Center. 

>[!Note]
>Siga os números nas bolhas amarelas em capturas de tela do PSC para localizar o atributo equivalente no Partner Center. As bolhas vermelhas indicam que o Arquivado não está disponível no Partner Center.

**Home Page do PSC e exibição padrão das oportunidades de venda conjunta no Partner Center**

 :::image type="content" source="images/pscmigration/homepage.png" alt-text="Imagem mostrando os mapeamentos de campo entre o home page de vendas do parceiro Connect e a exibição padrão de oportunidades de venda conjunta no Partner Center.":::

**Exibição de grade do PSC e visão do negócio do Partner Center**

- Não há nenhuma exibição de lista no Partner Center como a do PSC.  Todas as negociações são listadas com base na data mais recente recebida ou criada com as informações do cliente e o tipo de negócio. A primeira negociação na exibição é selecionada por padrão. A maioria dos valores exibidos no formato de tabela do PSC está disponível na exibição de detalhes do negócio no PC.
- A função de negócio não é um campo obrigatório no PC. Ele não é exibido nem capturado em nenhum dos fluxos de trabalho. Ele é derivado automaticamente no lado do vendedor da Microsoft com base nas soluções adicionadas ao negócio.
- A data da última modificação não é exibida na página de detalhes de referência no PC. Os parceiros podem usar a funcionalidade de classificação para classificar as negociações com base na data da última atualização.

 :::image type="content" source="images/pscmigration/gridview.png" alt-text="Imagem mostrando os mapeamentos de campo entre a exibição de grade do PSC (Partner Sales Connect) e a exibição de negociações do Partner Center.":::

**Exibição dos detalhes do acordo no PSC e no Partner Center**

- Os parceiros podem editar um negócio clicando no botão Editar na exibição de detalhes do acordo do parceiro (6). Depois que o botão de edição for clicado, todos os campos ativarão editável com a opção de salvar ou cancelar as edições feitas no negócio.
- Não há nenhuma opção para fechar o negócio como duplicado no Partner Center.
- O resultado do cliente não está disponível no Partner Center. Todos os detalhes relacionados às interações do cliente podem ser atualizados na seção observações do PC.
- A data de fechamento da solução estimada só está disponível para as negociações de IOT OEM no Partner Center. Ele não é exibido para nenhum outro tipo de negócio.
- O programa de licenciamento não é necessário no PC. Ele é inferido automaticamente com base nas soluções selecionadas no negócio.

>[!Note]
>Qualquer negociação marcada como ganha ou perdida não pode ser editada post. Tenha cuidado ao mover um negócio para um desses Estados de terminal.

 :::image type="content" source="images/pscmigration/dealdetails.png" alt-text="Imagem mostrando os mapeamentos de campo entre a exibição de detalhes de negociações do PSC (Partner Sales Connect) e a exibição de detalhes de acordo do Partner Center.":::

**Exibição do PSC ' Adicionar produtos ' e a exibição ' Adicionar soluções ' do centro de parceiros**

 :::image type="content" source="images/pscmigration/products.png" alt-text="Imagem mostrando os mapeamentos de campo entre a exibição Adicionar produtos do PSC (Partner Sales Connect) e o modo de exibição Adicionar soluções do Partner Center.":::

**Gerenciamento de usuários no PSC e no Partner Center**

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="Imagem mostrando os mapeamentos de campo entre o gerenciamento de usuário do Partner Sales Connect (PSC) e o gerenciamento de usuários do Partner Center na exibição configurações da conta.":::

**Atribuição de função de usuário no PSC e no centro de parceiros**

- A função equivalente para o administrador do PSC é a função de administrador da conta no Partner Center.
- Há apenas uma função no Partner Center para o gerenciamento de negociações de venda, que é a função de administrador de referência.

 :::image type="content" source="images/pscmigration/roles.png" alt-text="Imagem que mostra os mapeamentos de campo entre o modo de exibição de atribuição de função do PSC (Partner Sales Connect) e a exibição de atribuição de função do Partner Center.":::

**Notificações no PSC e no Partner Center**

 :::image type="content" source="images/pscmigration/notifications.png" alt-text="Imagem mostrando o mapeamento entre as notificações do PSC (Partner Sales Connect) e a exibição de notificações do Partner Center.":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>Mudando do PSC para o Partner Center-perguntas frequentes

**Trimestre. O que devo fazer se não tiver acesso ao Partner Center?**

Você pode entrar em contato com seus administradores listados na página "sem acesso" para obter as funções atribuídas. Você precisará da função "[administrador de referência](https://docs.microsoft.com/partner-center/permissions-overview#manage-referrals)" para permissão de leitura e gravação na seção referências. Se você estiver gerenciando apenas perfis comerciais, precisará da função "administrador de perfil de negócios" no centro de parceiros.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="Imagem mostrando a experiência sem acesso no Partner Center.":::

**Lançado. Quem pode me conceder acesso à seção referências no Partner Center?**

O [administrador da conta](https://docs.microsoft.com/partner-center/permissions-overview#manage-mpn-membership-and-your-company-non-aad-roles-these-roles-manage-the-company-business-rather-than-the-tenant) pode conceder acesso à guia referências. Para localizar o administrador da conta, vá para configurações de parceiro no ícone de engrenagem no canto superior direito do Partner Center. Clique na página Gerenciamento de usuários no segundo nível da barra de navegação à esquerda. Clique na lista suspensa que mostra "todos os usuários" no canto superior direito da página e altere para "administradores de conta". A página exibirá todos os administradores de conta com suas respectivas IDs de email. Entre em contato com eles para obter acesso "administrador de referência" para sua conta corporativa.

**3o. O botão de negociação + novo está esmaecido para nossa conta. O que devo fazer para começar a criar acordos?**

Isso só ocorrerá se não houver soluções prontas para venda coexistentes conectadas à organização MPN que você está usando no Partner Center. Entre em contato com o PDM para obter a ID do MPN de suas soluções corrigidas ou crie um tíquete de suporte mencionando o problema "novo botão de negociação esmaecido após a migração do PSC".

**P4. Posso atribuir negociações a uma pessoa específica de nossa organização, como o PSC?**

Você pode atribuir membros da equipe a um negócio específico. Ele não impede que outros administradores de referência exibam ou atuem nessas negociações. 

**P5. Há uma exibição de todas as negociações atribuídas a mim?**

Você pode usar o recurso favoritos, que é uma guia nível de usuário. Você pode marcar todas as negociações atribuídas a você como favoritos para obter acesso rápido às negociações.

**P6. Há uma exibição somente leitura para as negociações?**

Não, não há nenhuma exibição somente leitura das negociações na seção referências. Todos os administradores de referência terão acesso completo de leitura e gravação a todas as negociações.

**P7. Como posso registrar um negócio depois de torná-lo como ganha?**

Se o negócio atender aos critérios abaixo, vamos exibir um pop-up para iniciar o [registro de negociações](https://docs.microsoft.com/partner-center/register-deals).

- Há uma solução qualificada de incentivo anexada ao negócio.
- O vendedor da Microsoft é convidado para participar do negócio ou convidou você para o negócio.
- O cartão da Microsoft está no estado aceito ou ganho no Partner Center.

**P8. Recebo uma mensagem de erro quando clico no botão "+ novo registro de negociações" na seção registro de negociações. Como posso registrar minhas negociações?**

O "+ novo registro de negociações" deve ser usado somente pelos parceiros registrados no programa ISV Connect para registrar um negócio sem nenhuma oportunidade de venda correspondente no Partner Center. Para o registro de negócios com uma oportunidade de venda conjunta, um pop-up será exibido quando o negócio for marcado como ganho e se atender aos critérios para o registro de negociações.

**P9. Está adicionando uma organização de cliente obrigatória?**

Sim, adicionar uma [organização do cliente](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#select-your-customer) é obrigatório no Partner Center. Primeiro, comece pesquisando o local onde o cliente é o local. Com base nos detalhes que você tem; Você pode ser específico, incluindo o nome exato da construção ou apenas fornecer detalhes da cidade. A pesquisa da organização buscará todas as entidades legais que correspondem ao nome inserido para que você não precise inserir os detalhes do endereço. Todos os detalhes são preenchidos automaticamente com base na organização selecionada.

**P10. Os detalhes de contato do cliente são obrigatórios?**

Depende do [tipo de negócio](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#types-of-co-sell-opportunities) que você está criando. Se você estiver apenas compartilhando seu pipeline e não precisar de ajuda da organização de vendas da Microsoft, você pode optar por não fornecer detalhes de contato do cliente. Se você estiver vendendo uma venda em que está buscando ativamente ajuda do vendedor da Microsoft, será necessário fornecer os detalhes de contato do cliente. Você deve obter o consentimento explícito do cliente antes de criar uma solicitação de venda conjunta no Partner Center.

**P11. Quantas soluções posso adicionar a um negócio?**

Você pode adicionar até 50 soluções (análogas a ' produtos ' no PSC) a um negócio. Ao contrário do PSC, você pode misturar soluções de suas próprias soluções qualificadas para venda, SKUs de terceiros da Microsoft e outros produtos qualificados de terceiros. Não há nenhuma função de negócio que seja selecionada ou disponível no Partner Center. Para SKUs da Microsoft, você pode opcionalmente adicionar a quantidade e o preço para cada SKU que é adicionado ao negócio.

**P12. Quando receberei os detalhes do vendedor da Microsoft depois de criar um negócio?**

Os vendedores da Microsoft são atribuídos somente depois de corresponder ao requisito exato de ajuda declarado ao criar o negócio com o persona vendedor relevante no lado da Microsoft. Mesmo após a atribuição, os vendedores da Microsoft terão a opção de aceitar ou rejeitar o convite de venda conjunta. Somente se um convite de venda conjunta for aceito por um vendedor, o negócio será atualizado com os detalhes de contato do vendedor da Microsoft. O SLA para que os vendedores da Microsoft atuem no negócio é de 14 dias. É o mesmo SLA que os parceiros têm de agir sobre o negócio antes de entrar no estado expirado.

**Q13. Onde posso encontrar a ID da oportunidade?**

A ID da oportunidade no PSC é igual à ID do negócio no PC. Você pode encontrar a ID do negócio ao lado do nome da negociação ao abrir qualquer negócio.

**Q14. Como meu PDM pode obter acesso ao PC?**

O Partner Center não pode ser acessado pelo PDMs diretamente ao contrário do PSC. Há várias opções para habilitar esse recurso, que são mencionados abaixo.

- OCP insights – se PDMs estiver apenas exibindo as negociações & progresso relacionado a elas, eles poderão usar o portal do insights OCP para obter a exibição da sua organização. Essa é uma ferramenta interna e só está disponível para PDMs. Observe que o OCP insights não está disponível para os usuários da sua empresa.
- Usuário convidado no Partner Center-você pode adicionar sua conta do PDM @microsoft.com como um usuário convidado no Partner Center e atribuir a função de administrador de referência a eles para que eles possam exibir e agir em referências.
- Criando um [novo usuário](https://docs.microsoft.com/partner-center/create-user-accounts-and-set-permissions#add-a-new-user) em seu locatário-você pode criar um novo usuário em seu próprio locatário e compartilhar esses detalhes com o PDM para que eles possam exibir e agir em referências semelhantes a outros usuários de referência em sua conta.

## <a name="resources-to-help-you-create-and-manage-your-deals-in-partner-center"></a>Recursos para ajudá-lo a criar e gerenciar seus negócios no Partner Center

Se você ainda não leu os tópicos de ajuda de venda conjunta, os recursos a seguir ajudarão você a gerenciar as negociações no Partner Center.

|**Para fazer isso**   |**Leia isto**   |
|-----------------------|:-----------------------|
|Entendendo as guias e a navegação na página de oportunidades de venda|[Navegando na seção de venda conjunta](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#navigating-the-co-sell-section)|
|Selecionando uma organização de cliente na lista D&B |[Selecione seu cliente](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#select-your-customer)|
|Modificando os campos na seção detalhes do acordo|[Detalhes do acordo](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#deal-details)|
|Adicionando os funcionários da empresa a uma equipe de negociação|[Adicionar seus funcionários](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#add-your-employees)|
|Respondendo a um negócio de venda conjunta|[Gerenciar acordos de venda](https://docs.microsoft.com/partner-center/manage-co-sell-opportunities#responding-to-a-co-sell-opportunity)
|Registre as negociações que você ganhou no Partner Center |[Registrar uma nova negociação](https://docs.microsoft.com/partner-center/register-deals)
|Obtenha informações de referência e descubra como suas referências estão fazendo |[Insights de indicação](https://docs.microsoft.com/partner-center/referral-insights)
|Criando e gerenciando perfil de negócios|[Gerenciar perfil de negócios](https://docs.microsoft.com/partner-center/create-a-marketing-profile)
|Gerenciar clientes potenciais para seu perfil de negócios |[Gerenciar clientes potenciais](https://docs.microsoft.com/partner-center/manage-leads)|

## <a name="additional-resources"></a>Recursos adicionais

- [Vendas de parceiros Conecte-se à pasta de trabalho do Partner Center](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) -pasta de trabalho para alinhar os processos de vendas e as funções dos parceiros com novos processos de vendas por meio do Partner Center versus parceiros de vendas.
- [Guia de operações de covenda do Partner Center](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) -orientação para identificar um modelo operacional por meio do Partner Center para gerenciar clientes potenciais ou vender oportunidades de venda e registro de negócios.
- [Gerenciamento de referências deck](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) -instruções passo a passo para gerenciar clientes potenciais e comercializar oportunidades por meio do Partner Center.
- [Publicação e gerenciamento no Marketplace comercial](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) – instruções passo a passo visualizadas para criar, gerenciar e publicar ofertas por meio do Partner Center no mercado comercial.
