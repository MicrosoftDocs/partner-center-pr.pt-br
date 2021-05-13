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
ms.openlocfilehash: 584f8a7f2794cb64be49fe7f790904eff50c4c26
ms.sourcegitcommit: 7a6836bd962d5b426a8cb34a9132a87cbbbf39f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "109855090"
---
# <a name="guide-to-co-selling-in-partner-center-pc-for-partners-migrating-from-partner-sales-connect-psc"></a>Guia para a venda em conjunto no Partner Center (PC) para parceiros migrando do PSC (Partner Sales Connect)

**Funções apropriadas**: administrador da conta | Administrador de referências | Vendedor do PSC (Partner Sales Connect) | Administrador de Partner Sales Connect (PSC) | Gerente de negociações do Partner Sales Connect (PSC)

Este artigo fornece diretrizes para parceiros que migram de vendas de parceiros conectam-se ao Partner Center para que eles possam continuar criando e gerenciando acordos de venda de produtos no Partner Center.

>[!Note]
> Se você estiver aqui porque viu uma faixa no PSC sobre a migração, você está no lugar certo. Este guia não se aplica aos parceiros comerciais de avaliação de solução (SA) e de licenciamento OEM que gerenciam suas negociações no PSC.

>[!Important]
> A partir de 1º de abril de 2021, sua empresa não será capaz de criar ou editar acordos no PSC. **Você ainda poderá baixar os dados de negócios existentes usando o recurso de exportação em massa no PSC. Você também pode [migrar acordos abertos](psc-to-pc.md#psc-deals-migration) do PSC para o Partner Center após essa data.** <br><br> Se houver acordos em que você está trabalhando ativamente e que contenham soluções elegíveis de incentivo de venda de IP, você tem duas opções: <br><br> 1. Marque o negócio como ganho e conclua o registro do negócio no PSC antes de 31 de março de 2021. <br> 2. [migre as negociações para o](psc-to-pc.md#psc-deals-migration) Partner Center para que você obtenha mais tempo para trabalhar no negócio e inicie o registro de negócios.

Como você sabe, **a empresa perderá o acesso ao PSC após 30 de abril de 2021**. No entanto, você ainda encontrará tudo o que deseja fazer no Partner Center, como criar negociações de venda, gerenciar suas negociações e agir sobre as negociações enviadas para você pelos vendedores da Microsoft.

No entanto, haverá diferenças. As diretrizes a seguir podem ajudar a fazer sua transição para o Partner Center mais fácil e mais simples.

## <a name="before-you-move-things-you-need-to-know"></a>Antes de mover, as coisas que você precisa saber

### <a name="if-you-are-a-psc-admin"></a>Se você for um administrador do PSC

- Você precisa de um email de trabalho para entrar no [Partner Center](https://partner.microsoft.com/).
- Configurar sua conta com a ajuda do administrador Partner Center [conta.](permissions-overview.md)
- Saiba como fazer a venda em Partner Center lendo este documento.
- Configurar contas de usuário no Partner Center para todos os usuários PSC (funções de Administrador, Gerente de Oferta e Vendedor) e atribua a eles funções de administrador [de indicação](permissions-overview.md).

>[!IMPORTANT]
> Certifique-se de que a ID do MPN mostrada na faixa PSC está disponível na lista de locais do MPN Partner Center.

:::image type="content" source="images/pscmigration/mpnidcheck.png" alt-text="Imagem mostrando a faixa PSC em que os parceiros podem encontrar a ID do MPN.":::

 Para verificar se a ID do MPN aparece como um local do MPN do Partner Center, entre no [painel](https://partner.microsoft.com/dashboard)do Partner Center e selecione Configurações **(o** ícone de Engrenagem) no canto superior direito da tela, seguido por Configurações da **Conta**. No menu de navegação à esquerda  de segundo nível, selecione Locais para ver a lista de todas as IDs e locais do MPN associados à Partner Center segurança.

### <a name="if-you-are-a-psc-deal-manager-or-seller"></a>Se você for um gerente ou vendedor de negociações PSC

- Você precisa de um email de trabalho para entrar no painel Partner Center [.](https://partner.microsoft.com/dashboard)
- Se você estiver usando uma conta não comercial no PSC ou seu email de trabalho for para uma empresa diferente da empresa parceira, entre em contato com o administrador do PSC para ter ajuda com a configuração da conta.
- Verifique com o administrador do PSC se Partner Center configuração da conta de Partner Center estiver concluída, independentemente da conta que você usa para entrar no PSC.
- Verifique se você tem acesso ao Partner Center e à seção Indicações.
- Leia este documento para entender os fluxos de trabalho e as alterações no Partner Center.

## <a name="as-an-admin-in-psc-these-are-your-next-steps"></a>Como administrador no PSC, essas são as próximas etapas

No menu Partner Center à esquerda, selecione a **opção Indicações.** Confirme se você pode acessar as páginas Indicações.

  >[!Note]
  > Talvez seja necessário sair do Partner Center e entrar novamente para atualizar suas credenciais para acesso às páginas de Indicações.

Se você não vir a opção Indicações no menu Partner Center ou páginas relacionadas a [](permissions-overview.md) indicações, entre em contato  com o administrador da conta da sua empresa e peça que ele lhe dê acesso à opção Indicações e à área relacionada. 

Para encontrar o administrador da conta da sua empresa:

1. Selecione **configurações de conta** no ícone de engrenagem na parte superior direita do painel do Partner Center.

1. Selecione **Gerenciamento de usuários** no menu de navegação esquerdo de segundo nível.

1. Na parte superior da lista de usuários, selecione o menu suspenso **filtro** . Altere a opção para **administrador da conta**.

   A página exibirá todos os administradores de conta com seus respectivos endereços de email. Envie um email para ele e peça para atribuir a função de administrador de referências para sua conta corporativa.

  :::image type="content" source="images/pscmigration/account-admin.gif" alt-text="Imagem que mostra os administradores de conta na página de gerenciamento de usuário configurações de parceiro.":::

>[!Important]
>- Se sua função envolver apenas o gerenciamento de usuários no PSC, peça ao administrador da conta da sua empresa para atribuir a você a função de [administrador da conta](permissions-overview.md#manage-mpn-membership-and-your-company) no Partner Center. 
>- Se sua função também incluir o gerenciamento de oportunidades de venda conjunta, peça para receber a função de [administrador de referências](permissions-overview.md#manage-referrals) .
> - É uma boa ideia também indicar um líder de gerenciamento de alterações entre os administradores do PSC. Isso impedirá que todos os administradores do PSC precisem acessar individualmente os administradores de conta do Partner Center. Em vez disso, o líder de gerenciamento de alterações pode ser a pessoa principal trabalhando com o administrador da conta do Partner Center.

## <a name="user-migration"></a>migração de usuário

Depois de configurar sua conta no Partner Center, use o assistente de migração de usuário na página de oportunidades de venda para atribuir automaticamente funções do Partner Center aos funcionários de sua empresa.

>[!Note]
> A migração de usuário só pode ser executada por [Administradores de conta](permissions-overview.md#manage-mpn-membership-and-your-company) da sua empresa. Se você não tiver a função Administrador de conta, localize um administrador de conta que possa ajudar a configurar as contas de usuário com a ajuda do assistente de migração de usuário.

:::image type="content" source="images/pscmigration/user-migration.gif" alt-text="Imagem mostrando o assistente de migração de usuário.":::

Os administradores de conta verão um link do assistente de migração de usuário do PSC na página de oportunidades de venda ao lado do guia de referências. Eles podem iniciar a migração do usuário selecionando o link. Para iniciar a migração de usuário, os administradores podem selecionar o link. Eles podem executar essa etapa de migração de usuário várias vezes até que todos os usuários recebam funções adequadas no Partner Center.

A tabela de migração de usuário tem os seguintes detalhes:

- Conta de usuário – ID de email do funcionário
- Conta de parceiro PSC – a conta à qual o funcionário está associado no PSC
- Função de usuário PSC – uma das três funções atribuídas ao no PSC.
- Local do MPN do pc – o local para o qual o usuário receberá funções de computador relevantes. O MPN da conta de parceiro PSC é usado para localizar o local do MPN equivalente Partner Center atribuir permissões. Toda a organização indica a ID do MPN do vOrg.
- Função de usuário do pc – os funcionários são atribuídos a funções com base em suas funções de usuário PSC. O administrador no PSC receberá funções de administrador de indicações no PC. O vendedor receberá a função de usuário de indicações no PC. Saiba mais sobre as funções de PC e o que os usuários com essas funções podem fazer no Partner Center [aqui](permissions-overview.md#manage-referrals)
- Locatário do PC AAD – o locatário ao qual os usuários são atribuídos Partner Center
- Status – Há três estados possíveis para o status da migração
    - **Não migrado** – o usuário não tem nenhuma função de indicações de COMPUTADOR atribuída
    - **Migrado** – o usuário foi migrado com êxito com a função relevante atribuída, conforme mostrado na tabela
    - **Erro** – Não é possível concluir a migração devido a algum erro

Às vezes, a migração pode falhar e resultar em erros. Aqui estão alguns motivos pelos quais uma migração pode causar um erro e algumas das maneiras de resolver o problema:

1. Os usuários do PSC podem estar usando uma conta que não é de trabalho.

2. O usuário PSC pode estar usando uma conta de um domínio diferente do que você usa no Partner Center.

   Para resolver erros relacionados aos cenários 1 e 2, peça ao usuário para entrar no Partner Center usando sua conta de trabalho anexada ao seu locatário do Azure AD. O [administrador global](permissions-overview.md#manage-commercial-transactions-in-partner-center-azure-ad-and-csp-roles) pode ajudar.
   
   Para localizar seu administrador global: 
   - Entre no [painel](https://partner.microsoft.com/dashboard) do Partner Center e selecione **configurações de conta** no ícone de engrenagem na parte superior direita.
   - Selecione **Gerenciamento de usuários** na barra de navegação à esquerda de segundo nível.
   - Na parte superior da lista de usuários, selecione o menu suspenso **filtro** e altere a opção para **administrador global**. A página exibe todos os administradores globais com seus respectivos endereços de email. Peça a um deles para atribuir a função de administrador de referência para sua conta corporativa.
   
      O administrador global pode criar uma nova conta de usuário no seu locatário do Azure AD ou atribuir acesso de usuário convidado aos outros usuários da conta de domínio. Depois que as contas são configuradas para todos os gerentes de negócios e usuários do PSC, elas precisam entrar no Partner Center, selecionar **referências** no menu de navegação à esquerda e confirmar que podem ver a página referências.

3. O usuário já tem uma função de referência atribuída no Partner Center.
    - Você pode verificar a função existente do usuário. No canto superior direito do Partner Center, selecione **configurações** (o ícone de engrenagem) e, em seguida, **configurações de conta**. Quando você vir um segundo menu de navegação à esquerda, selecione **Gerenciamento de usuários** e procure o usuário.

## <a name="psc-deals-migration"></a>Migração de acordos do PSC

Depois de concluir a migração do usuário, use o assistente de migração para negociações na página de oportunidades de venda para trazer todos os acordos abertos qualificados do PSC para o PC. **O link de migração de negociações será visível somente para administradores de referência com escopo de toda a organização no Partner Center.** Haverá um link chamado **"migração de acordo com o PSC"** no canto superior direito da página de oportunidades de venda conjunta, que abrirá o assistente de migração de negociações.

Leia esta seção antes de iniciar a migração de negociações.

**Qualificado para migração**

Somente algumas ofertas estão qualificadas para a migração do PSC para o PC. Esse assistente de migração foi criado para ajudar os parceiros a Partner Center em que eles ainda estão trabalhando ativamente com seus clientes para fechar a transação. **Somente as negociações que estão em estado aberto criadas a partir de 1º de janeiro de 2020 com detalhes válidos da conta de parceiro (ID do MPN válida) e que não estão passando pelo registro de negociação são qualificadas para migração.**

**Não qualificado para migração**

- Os acordos de avaliação de solução não estão qualificados para a migração de negociações
- Os negócios de licenciamento do OEM não estão qualificados para a migração de ofertas
- Qualquer negociação que tenha sido marcada como ganha no PSC não está qualificada para migração. O registro de negociação, se elegíveis para as negociações marcadas como ganhas, deve ser concluído no PSC.

## <a name="pre-requisites-for-deal-migration"></a>Pré-requisitos para migração de negociação

Antes de iniciar a migração de oferta do PC, siga as instruções abaixo para configurar as negociações no PSC para uma migração bem-sucedida.

1. Todos os membros da equipe de vendas em sua empresa que trabalham em ofertas abertas são informados sobre essa migração.
2. Os membros da equipe de vendas são treinados para usar Partner Center gerenciamento de ofertas.
3. As negociações têm todas as informações necessárias, conforme descrito abaixo.
    - Detalhes da empresa do cliente, incluindo nome e endereço
    - Detalhes de contato do cliente se for uma negociação de venda em cooperação
    - Pelo menos uma solução
    - Pelo menos um membro da equipe com todos os detalhes – nome, sobrenome, ID de email e número de telefone
    - Valor da negociação
    - Data de fechamento estimada do negócio
    - Observações do parceiro

Você pode usar os recursos de download e upload em massa no PSC para adicionar todos os detalhes ausentes na oferta para todas as negociações qualificadas.

>[!Note]
> A migração de negociações terá sucesso mesmo se os pré-requisitos acima não forem atendidos. Mas, você não poderá alterar o estado do negócio se qualquer um dos campos obrigatórios acima mencionados no Partner Center não estiver disponível. Em seguida, você precisará inserir todas as informações necessárias que estão faltando nas negociações no Partner Center para começar a trabalhar nelas. **É altamente recomendável limpar as negociações qualificadas no PSC antes de migrá-las para o Partner Center.**

A migração de negociações no Partner Center é criada como uma experiência de clique. Tudo o que você precisa fazer é clicar no botão **"migrar negociações"** quando sua empresa estiver pronta para migrar os acordos qualificados. **Você não pode escolher as negociações que deseja migrar do PSC. Se você não quiser migrar qualquer um dos acordos para o Partner Center, mova-os para o estado fechado no PSC antes de iniciar a migração.**

>[!Note]
> Depois de iniciar a migração, **pode levar até 24 horas para que as negociações sejam migradas**.

Quando a migração for concluída, a mensagem de faixa terá o status alterado para concluída com um link para o relatório de migração. Baixe o relatório para exibir os detalhes das negociações que foram migradas do PSC para o PC.

O relatório inclui os detalhes abaixo.

1. **ID do engajamento do Partner Center** -o identificador exclusivo no Partner Center para todas as negociações em um envolvimento. Há duas negociações – uma para o parceiro e uma para a Microsoft em um compromisso de venda covendedor no Partner Center.
2. **ID de referência do Partner Center** -o identificador exclusivo no Partner Center para o negócio que pertence ao parceiro.
3. **Nome do acordo** -identificador dado à negociação no PSC.
4. **ID do acordo do PSC** -o identificador exclusivo no PSC para o negócio.
5. **Erros** -para indicar se há algum erro ao migrar um negócio específico.

Todas as negociações que foram migradas com êxito não estarão visíveis no PSC. Você pode continuar trabalhando nas negociações migradas no PC, incluindo a conclusão do registro de negociações no PC. Não haverá nenhuma alteração nas interações com os vendedores da Microsoft para as negociações de venda conjuntas.

As negociações migradas do PSC estarão disponíveis nas guias Entrada e Saída com base na origem da oferta. Todas as negociações compartilhadas por sua empresa estarão disponíveis na guia Saída e as negociações iniciadas pela Microsoft estarão disponíveis na guia Entrada do Partner Center. Haverá dois tipos de acordos que serão criados após a migração.

1. **Acordos de venda em cooperação** – as negociações marcadas como venda em PSC serão criadas como negociações de venda em Partner Center.
2. **Ofertas conduzidas por** parceiros – as negociações que não estão marcadas como venda co-venda serão criadas como ofertas de parceiros no Partner Center. As negociações conduzidas por parceiros são visíveis para vendedores da Microsoft e podem ser atualizadas para acordos de venda de co-venda antes de atingir o estado do terminal (ganho, perdido). Além disso, as negociações conduzidas por parceiros serão qualificadas para o registro de negociação se houver uma solução qualificada para incentivos na negociação.

>[!Important]
> Se houver erros devido aos quais algumas negociações não puderam ser migradas, você poderá reatar a migração de oferta clicando no botão **"Migrar ofertas".** Ela só será habilitada se houver algumas negociações qualificadas ainda a serem migradas. Isso também será útil se você estiver na fase de transição em que algumas novas negociações serão criadas no PSC depois de iniciar a migração de negociações.

Depois que todas as negociações são migradas com êxito, haverá uma faixa mostrando "Nenhuma oferta **para migrar"** com o botão **"Migrar ofertas"** sendo **desabilitado.**

Depois de concluir a migração de usuário e/ou a migração de negociação, use as seguintes diretrizes para decidir a estratégia de migração:

Se sua empresa tiver um PDM (Partner Development Manager) – quando sua conta do Partner Center estiver configurada e os usuários mudarem e têm funções e permissões, você poderá mover suas atividades de venda de parceiros para Partner Center. Informe o PDM para fazer a opção em vez de aguardar até que a migração seja concluída, o que permitirá que todas as novas negociações fluam para Partner Center.

>[!Note]
>Depois de fazer essa opção, você só poderá agir nos acordos ativos existentes no PSC. Você não pode criar novas negociações nem receber nenhuma medida de vendedores da Microsoft no PSC.

Se sua empresa não tiver um PDM, verifique se todas as contas de usuário estão configuradas e verificadas por todos os usuários. Você será notificado por meio de um email e uma faixa no PSC em relação à data exata quando puder começar a trabalhar com a venda no Partner Center. Lembre-se de que você ainda precisará gerenciar as negociações ativas existentes no PSC.

>[!Important]
> Você tem até 30 de abril de 2021 para registrar as negociações marcadas como ganhas.

## <a name="next-steps-for-psc-admins-psc-deal-managers-and-psc-sellers"></a>Próximas etapas para administradores do PSC, gerentes de negócios do PSC e vendedores do PSC

Saiba como fazer uma venda conjunta no Partner Center.
Esta é uma etapa importante, que ajudará você a se preparar para a venda em conjunto no Partner Center. Entenda os fluxos de trabalho e as alterações no Partner Center para que você possa realmente vender imediatamente. Comece lendo este documento completamente. Um bom conjunto de recursos também está disponível na [Galeria de experiência de cooperação](https://aka.ms/cosellexperience).

## <a name="major-differences-between-psc-and-pc-workflows"></a>Principais diferenças entre os fluxos de trabalho do PSC e do PC

|**Cenário**|**Conexão de vendas do parceiro**|**Partner Center**|
|-----|:-----|:-----|
|Funções de usuário|O PSC tem funções de administrador, gerente de negociações e vendedor.|O PC tem apenas a função [administrador de referências](permissions-overview.md#manage-referrals) que fornece permissão de leitura e gravação para todas as negociações.|
|Convidando a Microsoft em um negócio de venda conjunta|Iniciado pelo vendedor da Microsoft, não há nenhuma pergunta explícita pelo parceiro.|O parceiro terá que fazer uma [solicitação explícita](manage-co-sell-opportunities.md#add-solutions) se uma ajuda do Microsoft seller for necessária para um negócio. O vendedor da Microsoft tem uma opção para recusar a solicitação.|
|Expiry|Não há nenhum conceito de expiração de uma negociação.|Os acordos de entrada de parceiro expiram em 14 dias se não são aceitos pelo parceiro. O mesmo ocorre com os acordos de saída do parceiro em que eles podem entrar no estado expirado se o vendedor da Microsoft não agir sobre eles em 14 dias.|
|Detalhes do vendedor da Microsoft|Visível assim que um acordo é criado.|Os detalhes do Vendedor da Microsoft serão compartilhados com o Parceiro somente se o vendedor aceitar explicitamente o convite para venda em parceria.|
|[Pipeline privado](manage-co-sell-opportunities.md#types-of-co-sell-opportunities)|Não disponível.|Os parceiros podem compartilhar seu pipeline sem dar visibilidade aos vendedores da Microsoft.|
|Soluções|Soluções que pertencem a apenas uma lista de preços podem ser adicionadas a uma oferta.|O parceiro pode adicionar [soluções](manage-co-sell-opportunities.md#add-solutions) que pertencem às listas a seguir. a) Suas próprias soluções b) Soluções do catálogo de primeira parte da Microsoft (semelhantes à função transação deal no PSC) e c) soluções de venda co-venda de outros parceiros de terceiros (semelhante à função isv deal no PSC).|
|Atribuição de negociação|Somente o vendedor atribuído pode exibir e agir sobre as negociações.|Os membros da equipe podem ser adicionados a um acordo para especificar as pessoas que trabalham em um acordo, não há nenhum bloqueio de outros administradores de indicações de exibir ou agir sobre esses acordos.|
|Organização do cliente|Entrada de texto de formulário livre.|Você pode pesquisar a [organização do cliente](manage-co-sell-opportunities.md#select-your-customer) no banco de dados&[B](https://www.dnb.com/) apenas digitando alguns caracteres. O nome legal e o endereço são preenchidos automaticamente com base na escolha.|
|Contato do cliente|Não obrigatório.|Não é obrigatório para o compartilhamento de pipeline privado. Necessário se o vendedor da Microsoft for convidado a participar de uma solicitação de venda de uma parceria.|
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

### <a name="1---psc-home-page-mapped-to-the-partner-center-co-sell-opportunities-default-view"></a>1 - PSC home page mapeado para a exibição padrão de oportunidades de venda Partner Center venda de dados

Compare os círculos numerados correspondentes entre a captura de tela superior do PSC e a Partner Center de tela abaixo dele. Os números correspondentes mostram onde você pode encontrar o recurso ou atributo relacionado ao PSC Partner Center. Círculos vermelhos indicam que não há nenhuma correspondência Partner Center campo.  

:::image type="content" source="images/pscmigration/homepage.png" alt-text="Imagem mostrando os mapeamentos de campo entre a home page do Partner Sales Connect e a exibição padrão das oportunidades de venda em Partner Center." lightbox="images/pscmigration/home-page-expanded.png":::

### <a name="2---psc-grid-view-mapped-to-the-partner-center-deal-view"></a>2 - Exibição de grade PSC mapeada para a exibição Partner Center de negócios

Compare os círculos numerados correspondentes entre a captura de tela superior do PSC e a Partner Center de tela abaixo dele. Os números correspondentes mostram onde você pode encontrar o recurso ou atributo relacionado ao PSC Partner Center. Círculos vermelhos indicam que não há nenhuma correspondência Partner Center campo.  

> [!NOTE]
> Outras considerações aparecem abaixo das capturas de tela.

:::image type="content" source="images/pscmigration/gridview.png" alt-text="Imagem mostrando os mapeamentos de campo entre a exibição de grade do PSC (Partner Sales Connect) e a exibição Partner Center de negócios." lightbox="images/pscmigration/grid-view-expanded.png":::

**Considerações especiais:**

- Não há nenhuma exibição de lista Partner Center como a do PSC.  Todas as negociações são listadas com base na data mais recente recebida ou criada com as informações do cliente e o tipo da oferta. A primeira oferta na exibição é selecionada por padrão. A maioria dos valores exibidos no formato de tabela PSC está disponível na exibição detalhada da oferta no PC.
- A função deal não é um campo obrigatório no PC. Ele não é exibido ou capturado em nenhum dos fluxos de trabalho. Ele é derivado automaticamente no lado do vendedor da Microsoft com base nas soluções adicionadas à oferta.
- A data da última modificação não é exibida na página de detalhes da indicação no PC. Os parceiros podem usar a funcionalidade de classificação para classificar as negociações com base na data da última atualização.

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

### <a name="4---psc-add-products-view-mapped-to-the-partner-center-add-solutions-view"></a>4 - Exibição "Adicionar Produtos" do PSC mapeada para a exibição Partner Center "Adicionar soluções"

Compare os círculos numerados correspondentes na captura de tela superior (PSC) com a Partner Center de tela abaixo dela. Os números correspondentes mostram onde você pode encontrar o recurso ou atributo relacionado ao PSC Partner Center. Círculos vermelhos indicam que não há campo ou área correspondente Partner Center.
  
:::image type="content" source="images/pscmigration/products.png" alt-text="Imagem mostrando os mapeamentos de campo entre o PSC (Partner Sales Connect) adicionar exibição de produtos e a exibição Partner Center adicionar soluções." lightbox="images/pscmigration/products-expanded.png":::

### <a name="5---user-management-in-psc-versus-partner-center"></a>5 - Gerenciamento de usuários no PSC versus Partner Center

Compare os círculos numerados correspondentes na captura de tela superior (PSC) com a Partner Center de tela abaixo dela. Os números correspondentes mostram onde você pode encontrar o recurso ou atributo relacionado ao PSC Partner Center. Círculos vermelhos indicam que não há campo ou área correspondente Partner Center.  

 :::image type="content" source="images/pscmigration/usermanagement.png" alt-text="Imagem mostrando os mapeamentos de campo entre a página inicial de gerenciamento de usuários do PSC (Partner Sales Connect) e a exibição Partner Center Página de gerenciamento de usuários na área Configurações da conta."  lightbox="images/pscmigration/user-management-expanded.png":::

### <a name="6---user-role-assignment-in-psc-versus-partner-center"></a>6 - Atribuição de função de usuário no PSC versus Partner Center

Compare os círculos numerados correspondentes na captura de tela superior (PSC) com a Partner Center de tela abaixo dela. Os números correspondentes mostram onde você pode encontrar o recurso ou atributo relacionado ao PSC Partner Center. Círculos vermelhos indicam que não há campo ou área correspondente Partner Center.  

:::image type="content" source="images/pscmigration/roles.png" alt-text="Imagem mostrando os mapeamentos de campo entre a exibição de atribuição de função do PSC (Partner Sales Connect) e a exibição Partner Center de atribuição de função." lightbox="images/pscmigration/roles-expanded.png":::

**Considerações especiais:**

- A função equivalente para o administrador do PSC é a função de administrador da conta Partner Center.
- Há apenas uma função no Partner Center para o gerenciamento de negociações de venda em cooperação. Essa função é a função de administrador de indicação.

### <a name="7---notifications-in-psc-versus-partner-center"></a>7 - Notificações no PSC versus Partner Center

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

### <a name="4---can-i-assign-deals-to-a-specific-person-from-our-organization-like-psc"></a>4 - Posso atribuir acordos a uma pessoa específica de nossa organização, como PSC?

Você pode atribuir membros da equipe a um negócio específico. Ele não bloqueia a exibição ou a ação de outros administradores de indicações nessas negociações.

### <a name="5---is-there-a-view-of-all-the-deals-assigned-to-me"></a>5 - Há uma exibição de todos os acordos atribuídos a mim?

Você pode usar o recurso favoritos, que é uma guia no nível do usuário. Você pode marcar todas as negociações atribuídas a você como favoritos para obter um acesso rápido às negociações.

### <a name="6---is-there-a-read-only-view-for-the-deals"></a>6 - Há uma exibição somente leitura para as negociações?

Não, não há nenhuma exibição somente leitura dos acordos na seção de indicações. Todos os administradores de indicação terão acesso completo de leitura e gravação a todas as ofertas.

### <a name="7---how-can-i-register-a-deal-after-marking-it-as-won"></a>7 - Como posso registrar um negócio depois de marcar como ganho?

Se o acordo atender aos critérios abaixo, exibiremos um pop-up para iniciar o [registro de negociação.](./register-deals.md)

- Há uma solução qualificada para incentivos anexada à oferta.
- O vendedor da Microsoft é convidado a participar da negociação ou ele o convida para a oferta.
- O cartão da Microsoft está no estado Aceito ou Ganho Partner Center.

### <a name="8---i-get-an-error-message-when-i-select-the-new-deal-registration-button-in-the-deal-registration-section-how-can-i-register-my-deals"></a>8 - Eu receber uma mensagem de erro ao selecionar o botão "+Novo registro de oferta" na seção Registro de Oferta. Como posso registrar minhas ofertas?

O **botão +Novo** registro de oferta deve ser usado somente pelos parceiros registrados no programa ISV Connect para registrar um negócio sem oportunidade de venda de venda correspondente no Partner Center. Para registrar acordos com uma oportunidade de venda em cooperação, um pop-up será exibido quando o negócio for marcado como ganho e se ele atender aos critérios de registro de negociação.

### <a name="9---is-adding-a-customer-organization-mandatory"></a>9 - A adição de uma organização do cliente é obrigatória?

Sim, a adição [de uma organização do](./manage-co-sell-opportunities.md#select-your-customer) cliente é obrigatória Partner Center. Primeiro, comece pesquisando o local em que o cliente está localizado. Com base nos detalhes que você tem; Você pode ser específico, incluindo o nome exato da construção ou apenas fornecer detalhes da cidade. A pesquisa da organização buscará todas as entidades legais que correspondem ao nome inserido para que você não precise inserir os detalhes do endereço. Todos os detalhes são preenchidos automaticamente com base na organização selecionada.

### <a name="10---are-customer-contact-details-mandatory"></a>10-os detalhes de contato do cliente são obrigatórios?

Depende do [tipo de negócio](./manage-co-sell-opportunities.md#types-of-co-sell-opportunities) que você está criando. Se você estiver apenas compartilhando seu pipeline e não precisar de ajuda da organização de vendas da Microsoft, você pode optar por não fornecer detalhes de contato do cliente. Se você estiver vendendo uma venda em que está buscando ativamente ajuda do vendedor da Microsoft, será necessário fornecer os detalhes de contato do cliente. Você deve obter o consentimento explícito do cliente antes de criar uma solicitação de venda conjunta no Partner Center.

### <a name="11---how-many-solutions-can-i-add-to-a-deal"></a>11-quantas soluções posso adicionar a um negócio?

Você pode adicionar até 50 soluções (análogas a ' produtos ' no PSC) a um negócio. Ao contrário do PSC, você pode misturar soluções de suas próprias soluções qualificadas para venda, SKUs de terceiros da Microsoft e outros produtos qualificados de terceiros. Não há nenhuma função de negócio que seja selecionada ou disponível no Partner Center. Para SKUs da Microsoft, você pode opcionalmente adicionar a quantidade e o preço para cada SKU que é adicionado ao negócio.

### <a name="12---when-will-i-get-to-know-the-microsoft-seller-details-after-creating-a-deal"></a>12-quando saberei os detalhes do vendedor da Microsoft depois de criar um negócio?

Os vendedores da Microsoft são atribuídos somente depois de corresponder ao requisito exato de ajuda declarado ao criar o negócio com o persona vendedor relevante no lado da Microsoft. Mesmo após a atribuição, os vendedores da Microsoft terão a opção de aceitar ou rejeitar o convite de venda conjunta. Somente se um convite de venda conjunta for aceito por um vendedor, o negócio será atualizado com os detalhes de contato do vendedor da Microsoft. O SLA para que os vendedores da Microsoft atuem no negócio é de 14 dias. É o mesmo SLA que os parceiros têm de agir sobre o negócio antes de entrar no estado expirado.

### <a name="13---where-can-i-find-the-opportunity-id"></a>13-onde posso encontrar a ID da oportunidade?

A ID da oportunidade no PSC é a mesma que a ID de negociação no PC. Você pode encontrar a ID da negociação ao lado do nome da negociação ao abrir qualquer acordo.

### <a name="14---how-can-my-pdm-get-access-to-pc"></a>14 - Como meu PDM pode obter acesso ao PC?

Partner Center pode ser acessado por seus PDMs diretamente ao contrário do PSC. Há várias opções para habilitar essa funcionalidade, que são mencionadas abaixo.

- Insights do OCP – se os PDMs estão apenas exibindo os acordos e o progresso relacionados a eles, eles podem usar o portal do OCP Insights para obter a exibição da sua organização. Essa é uma ferramenta interna e está disponível apenas para PDMs. Observe que os insights do OCP não estão disponíveis para os usuários da sua empresa.
- Usuário convidado no Partner Center – você pode adicionar sua conta pdm como um usuário convidado no partner center e atribuir a ele a função de administrador de indicação para que ele possa exibir e agir em @microsoft.com indicações.
- Criando [um](./create-user-accounts-and-set-permissions.md#add-a-new-user) novo usuário em seu locatário – você pode criar um novo usuário em seu próprio locatário e compartilhar esses detalhes com o PDM para que ele possa exibir e agir em indicações semelhantes a outros usuários de indicação em sua conta.

## <a name="finding-the-correct-mpn-id-if-your-account-in-psc-is-not-associated-with-a-valid-mpn"></a>Localizar a ID do MPN correta se sua conta no PSC não estiver associada a um MPN válido

Se você estiver aqui porque viu uma faixa no PSC mencionando 'Problema de associação de ID de MPN inválida do PSC', você está no lugar certo. Sua conta pode ter sido vinculada a uma ID de MPN inválida devido aos seguintes motivos

- Sua empresa não tem uma conta Partner Center conta.
- Seu PDM errou ao inserir a ID do MPN de sua conta nos sistemas internos que vinculam sua conta PSC à sua conta Partner Center (MPNID).
- Sua empresa não concluiu a migração Partner Membership Center (PMC) para PC.

Primeiro, encontre a ID do MPN correta seguindo as etapas abaixo

- Faça logoff em sua Partner Center conta
- Use as diretrizes fornecidas na [documentação de configurações da conta](./partner-center-account-setup.md#locate-your-mpn-id) para localizar a ID do MPN.

Abaixo está uma captura de tela mostrando o local exato em que você pode encontrar sua ID Partner Center MPN

:::image type="content" source="images/pscmigration/findingMPNID.png" alt-text="Imagem mostrando as configurações de conta em que o parceiro pode encontrar sua ID de MPN."  lightbox="images/pscmigration/findingMPNID.png":::

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
- [Partner Center](https://partner.microsoft.com/resources/detail/co-sell-operating-model-guide-pptx) guia operacional de venda em cooperação – diretrizes para identificar um modelo operacional por meio do Partner Center para gerenciar oportunidades de venda ou venda em cooperação e registrar ofertas.
- [Baralho de gerenciamento de](https://partner.microsoft.com/resources/detail/referral-management-in-partner-center-pptx) indicações – instrução passo a passo visualizada para gerenciar leads e oportunidades de venda co-venda por meio Partner Center.
- [Publicação e gerenciamento](https://partner.microsoft.com/resources/detail/publishing-and-managing-co-sell-offers-in-commercial-marketplace-pptx) no marketplace comercial – instrução passo a passo visualizada para criar, gerenciar e publicar ofertas por meio de Partner Center no marketplace comercial.