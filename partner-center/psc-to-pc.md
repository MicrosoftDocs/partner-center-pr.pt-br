---
title: Migrar do Partner Sales Connect (PSC)
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como os parceiros da Microsoft podem migrar do PSC (Partner Sales Connect) para o Partner Center e criar ou gerenciar as negociações enviadas pelos vendedores da Microsoft.
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 12/07/2020
ms.openlocfilehash: 3475d606b3a59cf88bb9fb864ee765e4e9a20063
ms.sourcegitcommit: 1a0c83e2089cb58221bdb24525127378f5197ea8
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/14/2021
ms.locfileid: "98215944"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>Guia para a venda em conjunto no Partner Center (PC) para parceiros migrando do PSC (Partner Sales Connect)

**Funções apropriadas**

- Administrador de conta
- Administrador de indicações
- Vendedor do PSC (Partner Sales Connect)
- Administrador do PSC (Partner Sales Connect)
- Gerente de negociações do Partner Sales Connect (PSC)

Este artigo fornece diretrizes para parceiros que migram de vendas de parceiros conectam-se ao Partner Center para que eles possam continuar criando e gerenciando acordos de venda de produtos no Partner Center.

Como você sabe, sua empresa perderá o acesso ao PSC após 31 de março de 2021. No entanto, você ainda encontrará tudo o que deseja fazer no Partner Center, como criar negociações de venda, gerenciar suas negociações e agir sobre as negociações enviadas para você pelos vendedores da Microsoft.

No entanto, haverá diferenças. As diretrizes a seguir podem ajudar a fazer sua transição para o Partner Center mais fácil e mais simples.

>[!Important]
> Se você estiver aqui porque viu uma faixa no PSC sobre a migração, você está no lugar certo. Este guia não é aplicável à SA (avaliação de solução) e a parceiros de IOT OEM que gerenciam suas negociações no PSC.

## <a name="before-you-move-things-you-need-to-know"></a>Antes de mover, as coisas que você precisa saber

### <a name="if-you-are-a-psc-admin"></a>Se você for um administrador do PSC

- Você precisa de um email de trabalho para entrar no [Partner Center](https://partner.microsoft.com/).
- Configure sua conta com a ajuda do [administrador da conta](permissions-overview.md)do Partner Center.
- Saiba como fazer uma venda conjunta no Partner Center lendo este documento.
- Configure contas de usuário no Partner Center para todos os usuários do PSC (funções de administrador, gerente de negociações e vendedor) e atribua a eles [funções de administrador de referência](permissions-overview.md).

>[!IMPORTANT]
> Verifique se a ID de MPN mostrada na faixa PSC está disponível na lista de locais MPN no Partner Center.

:::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="Imagem mostrando a faixa do PSC em que os parceiros podem encontrar a ID do MPN.":::

 Para verificar se a ID do MPN aparece como um local do MPN do Partner Center, entre no [painel](https://partner.microsoft.com/dashboard)do Partner Center e selecione **configurações** (o ícone de engrenagem) na parte superior direita da tela, seguida pelas **configurações da conta**. No segundo nível, menu de navegação à esquerda, selecione **locais** para ver a lista de todas as IDs e locais MPN associados à conta do Partner Center.

### <a name="if-you-are-a-psc-deal-manager-or-seller"></a>Se você for um gerente de negociações do PSC ou vendedor

- Você precisa de um email de trabalho para entrar no [painel](https://partner.microsoft.com/dashboard)do Partner Center.
- Se você estiver usando uma conta que não seja de trabalho no PSC ou seu email de trabalho for para uma empresa diferente da empresa parceira, entre em contato com o administrador do PSC para obter ajuda de configuração de conta.
- Verifique com o administrador do PSC se a configuração da sua conta do Partner Center está concluída, independentemente da conta que você usa para entrar no PSC.
- Verifique se você tem acesso ao Partner Center e à seção referências.
- Leia este documento para entender os fluxos de trabalho e as alterações no Partner Center.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>Como administrador no PSC, estas são as próximas etapas

No menu de navegação esquerdo do Partner Center, selecione a opção **referências** . Confirme que você pode acessar as páginas de referências.

  >[!Note]
  > Talvez você precise sair do Partner Center e entrar novamente para atualizar suas credenciais para acessar as páginas de referências.

Se você não vir a opção **referências** no menu do Partner Center ou em páginas relacionadas a referências, entre em contato com o [administrador da conta](permissions-overview.md) da sua empresa e peça para conceder acesso à opção **referências** e à área relacionada.

Para localizar o administrador da conta da sua empresa:

1. Selecione **configurações de conta** no ícone de engrenagem na parte superior direita do painel do Partner Center.

1. Selecione **Gerenciamento de usuários** no menu de navegação esquerdo de segundo nível.

1. Na parte superior da lista de usuários, selecione o menu suspenso **filtro** . Altere a opção para **administrador da conta**.

   A página exibirá todos os administradores de conta com seus respectivos endereços de email. Envie um email para ele e peça para atribuir a função de administrador de referências para sua conta corporativa.

  :::image type="content" source="images/pscmigration/account-admin.png" alt-text="Imagem que mostra os administradores de conta na página de gerenciamento de usuário configurações de parceiro.":::

>[!Important]
>- Se sua função envolver apenas o gerenciamento de usuários no PSC, peça ao administrador da conta da sua empresa para atribuir a você a função de [administrador da conta](permissions-overview.md#manage-mpn-membership-and-your-company) no Partner Center. 
>- Se sua função também incluir o gerenciamento de oportunidades de venda conjunta, peça para receber a função de [administrador de referências](permissions-overview.md#manage-referrals) .
> - É uma boa ideia também indicar um líder de gerenciamento de alterações entre os administradores do PSC. Isso impedirá que todos os administradores do PSC precisem acessar individualmente os administradores de conta do Partner Center. Em vez disso, o líder de gerenciamento de alterações pode ser a pessoa principal trabalhando com o administrador da conta do Partner Center.

## <a name="user-migration"></a>migração de usuário

Depois de configurar sua conta no Partner Center, use o assistente de migração de usuário na página de oportunidades de venda para atribuir automaticamente funções do Partner Center aos funcionários de sua empresa.

>[!Note]
> A migração de usuário só pode ser executada por [Administradores de conta](permissions-overview.md#manage-mpn-membership-and-your-company) da sua empresa. Se você não tiver a função Administrador de conta, localize um administrador de conta que possa ajudar a configurar as contas de usuário com a ajuda do assistente de migração de usuário. A funcionalidade de migração do usuário estará disponível a partir de 18 de novembro de 2020.

:::image type="content" source="images/pscmigration/psc-user-migration.png" alt-text="Imagem mostrando o assistente de migração de usuário.":::

Os administradores de conta verão um link do assistente de migração de usuário do PSC na página de oportunidades de venda ao lado do guia de referências. Eles podem iniciar a migração do usuário selecionando o link. Para iniciar a migração de usuário, os administradores podem selecionar o link. Eles podem executar essa etapa de migração de usuário várias vezes até que todos os usuários recebam funções adequadas no Partner Center.

A tabela de migração de usuário tem os seguintes detalhes:

- Conta de usuário-ID de email do funcionário
- Conta de parceiro do PSC-a conta à qual o funcionário está associado no PSC
- Função de usuário do PSC – uma das três funções atribuídas ao no PSC.
- Local MPN do PC – o local para o qual o usuário receberá as funções relevantes do computador. A conta de parceiro do PSC MPN é usada para localizar o local equivalente do MPN no Partner Center para atribuir permissões. Toda a organização denota a ID de MPN vOrg.
- Função de usuário do computador-os funcionários recebem funções com base em suas funções de usuário do PSC. O administrador no PSC será atribuído às funções de administrador de referências no PC. O vendedor será atribuído à função de usuário de indicações no PC. Saiba mais sobre as funções do PC e o que os usuários com essas funções podem fazer no Partner Center [aqui](permissions-overview.md#manage-referrals)
- Locatário do AAD do PC-o locatário ao qual os usuários são atribuídos no Partner Center
- Status-há três estados possíveis para o status da migração
    - **Não migrado** -o usuário não tem nenhuma função de referências do PC atribuída
    - **Migrado** -o usuário foi migrado com êxito com a função relevante atribuída conforme mostrado na tabela
    - **Erro** -não é possível concluir a migração devido a algum erro

Às vezes, a migração pode falhar e resultar em erros. Aqui estão alguns motivos pelos quais uma migração pode causar um erro e algumas das maneiras de resolver o problema:

1. Os usuários do PSC podem estar usando uma conta que não seja de trabalho.

2. O usuário do PSC pode estar usando uma conta de um domínio diferente daquele que você usa no Partner Center.

   Para resolver erros relacionados aos cenários 1 e 2, peça ao usuário para entrar no Partner Center usando sua conta de trabalho anexada ao seu locatário do Azure AD. O [administrador global](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) pode ajudar.
   
   Para localizar seu administrador global: 
   - Entre no [painel](https://partner.microsoft.com/dashboard) do Partner Center e selecione **configurações de conta** no ícone de engrenagem na parte superior direita.
   - Selecione **Gerenciamento de usuários** na barra de navegação à esquerda de segundo nível.
   - Na parte superior da lista de usuários, selecione o menu suspenso **filtro** e altere a opção para **administrador global**. A página exibe todos os administradores globais com seus respectivos endereços de email. Peça a um deles para atribuir a função de administrador de referência para sua conta corporativa.
   
      O administrador global pode criar uma nova conta de usuário no seu locatário do Azure AD ou atribuir acesso de usuário convidado aos outros usuários da conta de domínio. Depois que as contas são configuradas para todos os gerentes de negócios e usuários do PSC, elas precisam entrar no Partner Center, selecionar **referências** no menu de navegação à esquerda e confirmar que podem ver a página referências.

3. O usuário já tem uma função de referência atribuída no Partner Center.
    - Você pode verificar a função existente do usuário. No canto superior direito do Partner Center, selecione **configurações** (o ícone de engrenagem) e, em seguida, **configurações de conta**. Quando você vir um segundo menu de navegação à esquerda, selecione **Gerenciamento de usuários** e procure o usuário.

Depois de concluir a migração do usuário, use as seguintes diretrizes para decidir a estratégia de migração:

Se sua empresa tiver um gerente de desenvolvimento de parceiros (PDM) – quando sua conta do Partner Center estiver configurada e os usuários tiverem se movido e tiverem funções e permissões, você poderá mover suas atividades de venda para o Partner Center. Informe ao PDM para fazer o comutador em vez de esperar até o prazo de conclusão da migração, o que permitirá que todas as suas novas negociações fluam para o Partner Center.

>[!Note]
>Depois de fazer essa opção, você só poderá agir sobre as negociações ativas existentes no PSC. Você não pode criar novas negociações nem receber nenhuma medida de vendedores da Microsoft no PSC.

Se sua empresa não tiver um PDM, verifique se todas as contas de usuário estão configuradas e verificadas por todos os usuários. Você será notificado por meio de um email e uma faixa no PSC em relação à data exata quando puder começar a trabalhar com a venda no Partner Center. Lembre-se de que você ainda precisará gerenciar as negociações ativas existentes no PSC.

>[!Important]
>As negociações ativas não serão migradas para o PC. Você tem até 31 de março de 2021 para fechar e registrar as negociações.

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>Próximas etapas para administradores do PSC, gerentes de negócios do PSC e vendedores do PSC

Saiba como fazer uma venda conjunta no Partner Center.
Esta é uma etapa importante, que ajudará você a se preparar para a venda em conjunto no Partner Center. Entenda os fluxos de trabalho e as alterações no Partner Center para que você possa realmente vender imediatamente. Comece lendo este documento completamente. Um bom conjunto de recursos também está disponível na [Galeria de experiência de cooperação](https://aka.ms/cosellexperience).

## <a name="major-differences-between-psc-and-pc-workflows"></a>Principais diferenças entre os fluxos de trabalho do PSC e do PC

|**Cenário**|**Conexão de vendas do parceiro**|**Partner Center**|
|-----|:-----|:-----|
|Funções de usuário|O PSC tem funções de administrador, gerente de negociações e vendedor.|O PC tem apenas a função [administrador de referências](permissions-overview.md#manage-referrals) que fornece permissão de leitura e gravação para todas as negociações.|
|Convidando a Microsoft em um negócio de venda conjunta|Iniciado pelo vendedor da Microsoft, não há nenhuma pergunta explícita pelo parceiro.|O parceiro terá que fazer uma [solicitação explícita](manage-co-sell-opportunities.md#add-solutions) se uma ajuda do Microsoft seller for necessária para um negócio. O vendedor da Microsoft tem uma opção para recusar a solicitação.|
|Expiry|Não há nenhum conceito de expiração de uma negociação.|Os acordos de entrada do parceiro expiram em 14 dias se não forem aceitos pelo parceiro. O mesmo é o caso de negócios de saída de parceiros onde eles podem entrar no estado expirado se o vendedor da Microsoft não agir em 14 dias.|
|Detalhes do vendedor da Microsoft|Visível assim que um acordo é criado.|Os detalhes do vendedor da Microsoft serão compartilhados com o parceiro somente se o vendedor aceitar explicitamente o convite para a venda de vendas do parceiro.|
|[Pipeline privado](manage-co-sell-opportunities.md#types-of-co-sell-opportunities)|Não disponível.|Os parceiros podem compartilhar seus pipelines sem dar visibilidade aos vendedores da Microsoft.|
|Soluções|As soluções que pertencem a apenas uma lista de preços podem ser adicionadas a um negócio.|O parceiro pode adicionar [soluções](manage-co-sell-opportunities.md#add-solutions) que pertencem às listas a seguir. a) as soluções de suas próprias soluções b) do catálogo de primeira parte da Microsoft (semelhante à função de negócio de transação no PSC) e c) comercializar soluções de outros parceiros de terceiros (semelhante à função de negócio de ISV no PSC).|
|Atribuição de negociações|Somente o vendedor atribuído pode exibir e agir sobre as negociações.|Os membros da equipe podem ser adicionados a um negócio para especificar as pessoas que trabalham em um negócio, não há nenhum bloqueio de outros administradores de referência de exibir ou agir nessas negociações.|
|Organização do cliente|Entrada de texto de formato livre.|Você pode pesquisar a [organização do cliente](manage-co-sell-opportunities.md#select-your-customer) no [banco de dados D&B](https://www.dnb.com/) digitando apenas alguns caracteres. O nome e o endereço legais são preenchidos automaticamente com base na escolha.|
|Contato do cliente|Não obrigatório.|Não obrigatório para compartilhamento de pipeline privado. Necessário se o vendedor da Microsoft for convidado a participar de uma solicitação de venda de uma parceria.|
|API pública|Não disponível.|[API pública](/partner/develop/referrals) para gerenciar programaticamente as referências do Partner Center.|

## <a name="map-the-fields-in-psc-to-the-corresponding-fields-in-partner-center"></a>Mapear os campos no PSC para os campos correspondentes no Partner Center

Esta seção compara (ou "mapeia") capturas de tela selecionadas para o PSC no modo de exibição correspondente na seção de oportunidades de venda do Partner Center.

Você verá círculos numerados, amarelos ou vermelhos em cada par de capturas de tela:

- **O que significam círculos amarelos?** Os círculos numerados e amarelos aparecem primeiro em cada captura de tela do PSC. Em seguida, você encontrará uma captura de tela do Partner Center com muitos dos mesmos números.

   Para ver como cada campo ou atributo no PSC é mapeado para sua contraparte no Partner Center, combine os círculos numerados juntos nas duas capturas de tela relacionadas. Por exemplo, coincida com o número, amarelo "1" na primeira, a captura de tela do PSC para o numerado, amarelo "1" no segundo, a captura de tela do Partner Center abaixo dele.

- **O que significa um círculo vermelho?** Se você vir um círculo vermelho em uma captura de tela, isso indicará que o campo PSC não está disponível no Partner Center.

Os mapeamentos de campo do centro do PSC para o parceiro são mostrados para as seguintes áreas:

1. O PSC home page mapeado para a exibição padrão de oportunidades de venda de parceiros do Partner Center
1. Exibição de grade do PSC mapeada para a exibição de negócio do Partner Center
1. Exibição de detalhes de acordo do PSC mapeada para a exibição de detalhes de negociações do Partner Center
1. Modo de exibição Adicionar produtos do PSC mapeado para o Partner Center adicionar exibição de soluções
1. Exibição de gerenciamento de usuário do PSC mapeada para a exibição de gerenciamento de usuário do Partner Center
1. Exibição de atribuição de função de usuário do PSC mapeada para a exibição de atribuição de função do Partner Center
1. Exibição de notificações do PSC mapeada para a exibição de notificações do Partner Center

### <a name="1---psc-home-page-mapped-to-the-partner-center-co-sell-opportunities-default-view"></a>1-PSC home page mapeado para a exibição padrão de oportunidades de venda do Partner Center

Compare os círculos correspondentes numerados entre a captura de tela principal do PSC e a captura de tela do Partner Center abaixo dele. Os números correspondentes mostram onde você pode encontrar o recurso ou atributo relacionado ao PSC no Partner Center. Círculos vermelhos indicam que não há nenhum campo do Partner Center correspondente.  

:::image type="content" source="images/pscmigration/homepage.png" alt-text="Imagem mostrando os mapeamentos de campo entre o home page de vendas do parceiro Connect e a exibição padrão de oportunidades de venda conjunta no Partner Center." lightbox="images/pscmigration/home-page-expanded.png":::

### <a name="2---psc-grid-view-mapped-to-the-partner-center-deal-view"></a>2-exibição de grade do PSC mapeada para a exibição de negócio do Partner Center

Compare os círculos correspondentes numerados entre a captura de tela principal do PSC e a captura de tela do Partner Center abaixo dele. Os números correspondentes mostram onde você pode encontrar o recurso ou atributo relacionado ao PSC no Partner Center. Círculos vermelhos indicam que não há nenhum campo do Partner Center correspondente.  

> [!NOTE]
> Outras considerações aparecem abaixo das capturas de tela.

:::image type="content" source="images/pscmigration/gridview.png" alt-text="Imagem mostrando os mapeamentos de campo entre a exibição de grade do PSC (Partner Sales Connect) e a exibição de negociações do Partner Center." lightbox="images/pscmigration/grid-view-expanded.png":::

**Considerações especiais:**

- Não há nenhuma exibição de lista no Partner Center como a do PSC.  Todas as negociações são listadas com base na data mais recente recebida ou criada com as informações do cliente e o tipo de negócio. A primeira negociação na exibição é selecionada por padrão. A maioria dos valores exibidos no formato de tabela do PSC está disponível na exibição de detalhes do negócio no PC.
- A função de negócio não é um campo obrigatório no PC. Ele não é exibido nem capturado em nenhum dos fluxos de trabalho. Ele é derivado automaticamente no lado do vendedor da Microsoft com base nas soluções adicionadas ao negócio.
- A data da última modificação não é exibida na página de detalhes de referência no PC. Os parceiros podem usar a funcionalidade de classificação para classificar as negociações com base na data da última atualização.

### <a name="3---psc-deal-details-view-mapped-to-partner-center"></a>3-modo de exibição de detalhes de acordo com o PSC mapeado para o Partner Center

Compare os círculos correspondentes numerados na captura de tela superior (PSC) com a captura de tela do Partner Center abaixo dele. Os números correspondentes mostram onde você pode encontrar o recurso ou atributo relacionado ao PSC no Partner Center. Círculos vermelhos indicam que não há nenhum campo ou área correspondente no Partner Center.

> [!NOTE]
> Outras considerações aparecem abaixo das capturas de tela.

:::image type="content" source="images/pscmigration/dealdetails.png" alt-text="Imagem mostrando os mapeamentos de campo entre a exibição de detalhes de negociações do PSC (Partner Sales Connect) e a exibição de detalhes de acordo do Partner Center." lightbox="images/pscmigration/deal-details-expanded.png":::

**Considerações especiais:**

- Os parceiros podem editar um negócio selecionando o botão Editar na exibição de detalhes do acordo do parceiro (6). Depois que o botão Editar for selecionado, todos os campos ficarão editáveis. Em seguida, você tem a opção de salvar ou cancelar as edições feitas no negócio.
- Não há nenhuma opção para fechar o negócio como duplicado no Partner Center.
- O resultado do cliente não está disponível no Partner Center. Todos os detalhes relacionados às interações do cliente podem ser atualizados na seção observações do PC.
- A data de fechamento da solução estimada só está disponível para as negociações de IOT do OEM no Partner Center. Essas informações não são exibidas para nenhum outro tipo de negócio.
- O programa de licenciamento não é necessário no PC. Essas informações são inferidas automaticamente com base nas soluções selecionadas no negócio.

>[!Note]
>Qualquer negociação marcada como ganha ou perdida não pode ser editada posteriormente. Tenha cuidado ao mover um negócio para um desses Estados de terminal.

### <a name="4---psc-add-products-view-mapped-to-the-partner-center-add-solutions-view"></a>4-a exibição ' Adicionar produtos ' do PSC está mapeada para a exibição ' Adicionar soluções ' do Partner Center

Compare os círculos correspondentes numerados na captura de tela superior (PSC) com a captura de tela do Partner Center abaixo dele. Os números correspondentes mostram onde você pode encontrar o recurso ou atributo relacionado ao PSC no Partner Center. Círculos vermelhos indicam que não há nenhum campo ou área correspondente no Partner Center.
  
:::image type="content" source="images/pscmigration/products.png" alt-text="Imagem mostrando os mapeamentos de campo entre a exibição Adicionar produtos do PSC (Partner Sales Connect) e o modo de exibição Adicionar soluções do Partner Center." lightbox="images/pscmigration/products-expanded.png":::

### <a name="5---user-management-in-psc-versus-partner-center"></a>5-gerenciamento de usuário no PSC versus Partner Center

Compare os círculos correspondentes numerados na captura de tela superior (PSC) com a captura de tela do Partner Center abaixo dele. Os números correspondentes mostram onde você pode encontrar o recurso ou atributo relacionado ao PSC no Partner Center. Círculos vermelhos indicam que não há nenhum campo ou área correspondente no Partner Center.  

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="Imagem mostrando os mapeamentos de campo entre a página de gerenciamento de usuário do PSC (Partner Sales Connect) e o modo de exibição de usuário do Partner Center na área de configurações da conta."  lightbox="images/pscmigration/user-management-expanded.png":::

### <a name="6---user-role-assignment-in-psc-versus-partner-center"></a>6-atribuição de função de usuário no PSC versus Partner Center

Compare os círculos correspondentes numerados na captura de tela superior (PSC) com a captura de tela do Partner Center abaixo dele. Os números correspondentes mostram onde você pode encontrar o recurso ou atributo relacionado ao PSC no Partner Center. Círculos vermelhos indicam que não há nenhum campo ou área correspondente no Partner Center.  

:::image type="content" source="images/pscmigration/roles.png" alt-text="Imagem que mostra os mapeamentos de campo entre o modo de exibição de atribuição de função do PSC (Partner Sales Connect) e a exibição de atribuição de função do Partner Center." lightbox="images/pscmigration/roles-expanded.png":::

**Considerações especiais:**

- A função equivalente para o administrador do PSC é a função de administrador da conta no Partner Center.
- Há apenas uma função no Partner Center para gerenciamento de negociações de venda. Essa função é a função de administrador de referência.

### <a name="7---notifications-in-psc-versus-partner-center"></a>7-notificações no PSC versus Partner Center

Compare os círculos correspondentes numerados na captura de tela superior (PSC) com a captura de tela do Partner Center abaixo dele. Os números correspondentes mostram onde você pode encontrar o recurso ou atributo relacionado ao PSC no Partner Center. Círculos vermelhos indicam que não há nenhum campo ou área correspondente no Partner Center.  

:::image type="content" source="images/pscmigration/notifications.png" alt-text="Imagem mostrando o mapeamento entre as notificações do PSC (Partner Sales Connect) e a exibição de notificações do Partner Center."  lightbox="images/pscmigration/notifications-expanded.png":::

## <a name="moving-from-psc-to-partner-center---frequently-asked-questions"></a>Mudando do PSC para o Partner Center-perguntas frequentes

As seções a seguir respondem a perguntas frequentes sobre a migração.

### <a name="1---what-should-i-do-if-i-dont-have-access-to-partner-center"></a>1-o que devo fazer se não tiver acesso ao Partner Center?

Você pode entrar em contato com seus administradores listados na página "sem acesso" para obter as funções atribuídas. Você precisará da função [administrador de referência](permissions-overview.md#manage-referrals) para permissão de leitura e gravação na seção referências. Se você estiver gerenciando apenas perfis comerciais, precisará da função de administrador do perfil de negócios no Partner Center.

:::image type="content" source="images/pscmigration/noaccess.png" alt-text="Imagem mostrando a experiência sem acesso no Partner Center.":::

### <a name="2---who-can-grant-me-access-to-the-referrals-section-in-partner-center"></a>2-quem pode me conceder acesso à seção referências no Partner Center?

O [administrador da conta](permissions-overview.md#manage-mpn-membership-and-your-company) pode conceder acesso à guia referências. Para localizar o administrador da conta, selecione **configurações de conta** no ícone de engrenagem na parte superior direita do [painel](https://partner.microsoft.com/dashboard)do Partner Center. Em seguida, selecione **Gerenciamento de usuários** na barra de navegação à esquerda de segundo nível. Na parte superior da lista de usuários, selecione o menu suspenso **filtro** e altere a opção para administrador da **conta**. A página exibirá todos os administradores de conta com seus respectivos endereços de email. Peça a um deles para atribuir a função de administrador de referência para sua conta corporativa.

### <a name="3---the-new-deal-button-is-greyed-out-for-our-account-what-should-i-do-to-start-creating-deals"></a>3-o botão de negociação + novo está esmaecido para nossa conta. O que devo fazer para começar a criar acordos?

Isso só ocorrerá se não houver soluções prontas para venda coexistentes conectadas à organização MPN que você está usando no Partner Center. Entre em contato com o PDM para obter a ID do MPN de suas soluções corrigidas ou criar um tíquete de suporte mencionando o problema, "novo botão de negociação esmaecido após a migração do PSC".

### <a name="4---can-i-assign-deals-to-a-specific-person-from-our-organization-like-psc"></a>4-posso atribuir negociações a uma pessoa específica de nossa organização, como o PSC?

Você pode atribuir membros da equipe a um negócio específico. Ele não impede que outros administradores de referência exibam ou atuem nessas negociações.

### <a name="5---is-there-a-view-of-all-the-deals-assigned-to-me"></a>5-há uma exibição de todas as negociações atribuídas a mim?

Você pode usar o recurso favoritos, que é uma guia no nível do usuário. Você pode marcar todas as negociações atribuídas a você como favoritos para obter acesso rápido às negociações.

### <a name="6---is-there-a-read-only-view-for-the-deals"></a>6-há uma exibição somente leitura para as negociações?

Não, não há nenhuma exibição somente leitura das negociações na seção referências. Todos os administradores de referência terão acesso completo de leitura e gravação a todas as negociações.

### <a name="7---how-can-i-register-a-deal-after-marking-it-as-won"></a>7-como posso registrar um negócio depois de marcá-lo como ganho?

Se o negócio atender aos critérios abaixo, vamos exibir um pop-up para iniciar o [registro de negociações](./register-deals.md).

- Há uma solução qualificada de incentivo anexada ao negócio.
- O vendedor da Microsoft é convidado para participar do negócio ou convidou você para o negócio.
- O cartão da Microsoft está no estado aceito ou ganho no Partner Center.

### <a name="8---i-get-an-error-message-when-i-select-the-new-deal-registration-button-in-the-deal-registration-section-how-can-i-register-my-deals"></a>8-recebo uma mensagem de erro quando seleciono o botão "+ novo registro de negociações" na seção registro de negociações. Como posso registrar minhas negociações?

O botão **+ novo registro de negociação** é usado somente pelos parceiros registrados no programa ISV Connect para registrar um negócio sem nenhuma oportunidade de venda correspondente no Partner Center. Para o registro de negócios com uma oportunidade de venda conjunta, um pop-up será exibido quando o negócio for marcado como ganho e se atender aos critérios para o registro de negociações.

### <a name="9---is-adding-a-customer-organization-mandatory"></a>9-está adicionando uma organização de cliente obrigatória?

Sim, adicionar uma [organização do cliente](./manage-co-sell-opportunities.md#select-your-customer) é obrigatório no Partner Center. Primeiro, comece pesquisando o local onde o cliente é o local. Com base nos detalhes que você tem; Você pode ser específico, incluindo o nome exato da construção ou apenas fornecer detalhes da cidade. A pesquisa da organização buscará todas as entidades legais que correspondem ao nome inserido para que você não precise inserir os detalhes do endereço. Todos os detalhes são preenchidos automaticamente com base na organização selecionada.

### <a name="10---are-customer-contact-details-mandatory"></a>10-os detalhes de contato do cliente são obrigatórios?

Depende do [tipo de negócio](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) que você está criando. Se você estiver apenas compartilhando seu pipeline e não precisar de ajuda da organização de vendas da Microsoft, você pode optar por não fornecer detalhes de contato do cliente. Se você estiver vendendo uma venda em que está buscando ativamente ajuda do vendedor da Microsoft, será necessário fornecer os detalhes de contato do cliente. Você deve obter o consentimento explícito do cliente antes de criar uma solicitação de venda conjunta no Partner Center.

### <a name="11---how-many-solutions-can-i-add-to-a-deal"></a>11-quantas soluções posso adicionar a um negócio?

Você pode adicionar até 50 soluções (análogas a ' produtos ' no PSC) a um negócio. Ao contrário do PSC, você pode misturar soluções de suas próprias soluções qualificadas para venda, SKUs de terceiros da Microsoft e outros produtos qualificados de terceiros. Não há nenhuma função de negócio que seja selecionada ou disponível no Partner Center. Para SKUs da Microsoft, você pode opcionalmente adicionar a quantidade e o preço para cada SKU que é adicionado ao negócio.

### <a name="12---when-will-i-get-to-know-the-microsoft-seller-details-after-creating-a-deal"></a>12-quando saberei os detalhes do vendedor da Microsoft depois de criar um negócio?

Os vendedores da Microsoft são atribuídos somente depois de corresponder ao requisito exato de ajuda declarado ao criar o negócio com o persona vendedor relevante no lado da Microsoft. Mesmo após a atribuição, os vendedores da Microsoft terão a opção de aceitar ou rejeitar o convite de venda conjunta. Somente se um convite de venda conjunta for aceito por um vendedor, o negócio será atualizado com os detalhes de contato do vendedor da Microsoft. O SLA para que os vendedores da Microsoft atuem no negócio é de 14 dias. É o mesmo SLA que os parceiros têm de agir sobre o negócio antes de entrar no estado expirado.

### <a name="13---where-can-i-find-the-opportunity-id"></a>13-onde posso encontrar a ID da oportunidade?

A ID da oportunidade no PSC é igual à ID do negócio no PC. Você pode encontrar a ID do negócio ao lado do nome da negociação ao abrir qualquer negócio.

### <a name="14---how-can-my-pdm-get-access-to-pc"></a>14-como meu PDM pode obter acesso ao PC?

O Partner Center não pode ser acessado pelo PDMs diretamente ao contrário do PSC. Há várias opções para habilitar esse recurso, que são mencionados abaixo.

- Provisões do OCP – se PDMs estiver apenas exibindo as negociações e o progresso relacionados a elas, eles poderão usar o portal do insights OCP para obter a exibição da sua organização. Essa é uma ferramenta interna e só está disponível para PDMs. Observe que o OCP insights não está disponível para os usuários da sua empresa.
- Usuário convidado no Partner Center-você pode adicionar sua conta do PDM @microsoft.com como um usuário convidado no Partner Center e atribuir a função de administrador de referência a eles para que eles possam exibir e agir em referências.
- Criando um [novo usuário](./create-user-accounts-and-set-permissions.md#add-a-new-user) em seu locatário-você pode criar um novo usuário em seu próprio locatário e compartilhar esses detalhes com o PDM para que eles possam exibir e agir em referências semelhantes a outros usuários de referência em sua conta.

## <a name="finding-the-correct-mpn-id-if-your-account-in-psc-is-not-associated-with-a-valid-mpn"></a>Encontrando a ID de MPN correta se sua conta no PSC não estiver associada a um MPN válido

Se você estiver aqui porque viu uma faixa no PSC mencionando "problema de associação de ID de MPN inválido do PSC", você está no lugar certo.

Primeiro, localize a ID de MPN correta seguindo as etapas abaixo

- Faça logon em sua conta do Partner Center
- Use as diretrizes fornecidas na [documentação de configurações de conta](./partner-center-account-setup.md#locate-your-mpn-id) para localizar a ID de MPN.

Em seguida,

- Se você tiver um PDM, peça-lhe para que sua ID do MPN seja corrigida com a ID MPN correta da sua conta do Partner Center.
- Se você não tiver um PDM, envie um email para o endereço fornecido na faixa PSC com as informações de conta do PSC mostradas na faixa PSC e a ID de MPN correta da sua conta do Partner Center.

## <a name="resources-to-help-you-create-and-manage-your-deals-in-partner-center"></a>Recursos para ajudá-lo a criar e gerenciar seus negócios no Partner Center

Se você ainda não leu os tópicos de ajuda de venda conjunta, os recursos a seguir ajudarão você a gerenciar as negociações no Partner Center.

|**Para fazer isso**   |**Leia isto**   |
|-----------------------|:-----------------------|
|Entendendo as guias e a navegação na página de oportunidades de venda|[Navegando na seção de venda conjunta](./manage-co-sell-opportunities.md#navigating-the-co-sell-section)|
|Selecionando uma organização de cliente na lista D&B |[Selecione seu cliente](./manage-co-sell-opportunities.md#select-your-customer)|
|Modificando os campos na seção detalhes do acordo|[Detalhes do acordo](./manage-co-sell-opportunities.md#deal-details)|
|Adicionando os membros da equipe a uma equipe de negociação|[Adicionar seus funcionários](./manage-co-sell-opportunities.md#add-team-members)|
|Respondendo a um negócio de venda conjunta|[Gerenciar acordos de venda](./manage-co-sell-opportunities.md#responding-to-a-co-sell-opportunity)
|Registre as negociações que você ganhou no Partner Center |[Registrar uma nova negociação](./register-deals.md)
|Obtenha informações de referência e descubra como suas referências estão fazendo |[Insights de indicação](./referral-insights.md)
|Criando e gerenciando perfil de negócios|[Gerenciar perfil de negócios](./create-a-marketing-profile.md)
|Gerenciar clientes potenciais para seu perfil de negócios |[Gerenciar clientes potenciais](./manage-leads.md)|

## <a name="next-steps"></a>Próximas etapas


- [Vendas de parceiros Conecte-se à pasta de trabalho do Partner Center](https://partner.microsoft.com/resources/detail/partner-sales-connect-to-partner-center-transition-workbook-pptx) -pasta de trabalho para alinhar os processos de vendas e as funções dos parceiros com novos processos de vendas por meio do Partner Center versus parceiros de vendas.
- [Guia de operações de covenda do Partner Center](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) -orientação para identificar um modelo operacional por meio do Partner Center para gerenciar clientes potenciais ou vender oportunidades de venda e registro de negócios.
- [Gerenciamento de referências deck](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) -instruções passo a passo para gerenciar clientes potenciais e comercializar oportunidades por meio do Partner Center.
- [Publicação e gerenciamento no Marketplace comercial](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) – instruções passo a passo visualizadas para criar, gerenciar e publicar ofertas por meio do Partner Center no mercado comercial.