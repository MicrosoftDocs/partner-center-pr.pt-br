---
title: Operações em massa por meio de arquivos do Excel em referências
ms.topic: article
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Saiba como baixar, criar ou atualizar oportunidades de venda conjunta usando arquivos do Excel
author: vikramb
ms.author: vikramb
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.date: 02/03/2021
ms.openlocfilehash: 16975e78c10aeb73bf141c1a1d0a215ac885039c
ms.sourcegitcommit: 64243caed029ffe40e2bbc369f4ee96f4f0ca26f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/18/2021
ms.locfileid: "100645632"
---
# <a name="bulk-operations-for-co-sell-opportunities-using-comma-separated-valuecsv-files"></a>Operações em massa para as oportunidades de venda conjunta usando arquivos CSV (valores separados por vírgula)

**Funções apropriadas**

- Administrador de indicações
- Usuário de indicações

As operações em massa no Partner Center ajudarão sua empresa a exportar e importar dados de oportunidades de venda. Navegue até a página oportunidades de venda conjunta para localizar os links importar e exportar na parte superior direita da faixa título da página. Os usuários com as permissões **administrador de referências** e **referências de usuário** podem usar essa funcionalidade.

> [!IMPORTANT]
> As ações criar/atualizar feitas por meio da importação em massa não são reversível. Tenha cuidado ao modificar ou criar um grande número de registros. Somente um subconjunto de campos pode ser modificado após a criação de um negócio. **Nenhuma ação será permitida quando qualquer negociação atingir um estado de terminal como recusado/expirado/ganha/perdido.**

## <a name="exporting-co-sell-opportunities"></a>Exportando oportunidades de venda de cooperação

Abaixo estão os detalhes da funcionalidade de exportação

- Você pode exportar no **máximo 5000 registros** clicando no botão Exportar.
- As negociações que são baixadas serão baseadas em seus níveis de acesso. Administradores de referência e usuários de referência podem obter resultados diferentes com base em seu escopo e serem incluídos como membros da equipe nas negociações. Saiba mais sobre [as permissões de referências](permissions-overview.md#manage-referrals).
- A função exportar leva em conta a guia atual na página oportunidades de venda e os filtros que foram aplicados.
- Um arquivo CSV com todos os dados com base nos filtros aplicados será gerado.
- Pode levar até um minuto para baixar os registros.
- Você não precisa aguardar a ação de download ser concluída. Mesmo que você navegue para outras páginas no Partner Center, o arquivo será baixado assim que a função de exportação for concluída.
- Você pode reutilizar o arquivo baixado para modificar os detalhes de acordo e carregar para atualizar os registros.

## <a name="importing-co-sell-opportunities"></a>Importando oportunidades de venda de cooperação

- Você pode criar ou atualizar um **máximo de 1000 registros** usando a funcionalidade de importação.
- Você pode criar o modelo do zero baixando o modelo da página Importar no Partner Center.
- Você também pode usar a funcionalidade de exportação para baixar os registros existentes e atualizá-los.
- Se o arquivo tiver mais de 1000 registros, ele não poderá ser processado.
- Depois que o arquivo for processado, um resumo com o número de referências criadas, atualizadas e não processadas será mostrado no último cartão de arquivo do processo.
- Você pode baixar os detalhes dos registros processados, corrigir todos os erros e carregar o mesmo arquivo para criar ou atualizar os registros que falharam na execução anterior. **Remova todos os registros bem-sucedidos do arquivo antes de carregar os registros corrigidos que falharam na execução anterior.**
- Para adicionar mais soluções, adicione colunas extras ao lado da solução 1 e use o nome da coluna como solução X, em que X representa o número da solução no negócio. Por exemplo, solução 2, solução 3.
- Você pode adicionar até 50 soluções a um negócio.
- Para adicionar mais membros da equipe, adicione colunas extras ao lado do membro da equipe 1 e use o nome da coluna como membro da equipe X, em que X representa o número do membro da equipe no negócio. Por exemplo, membro da equipe 2, membro da equipe 3.
- Você pode adicionar até 50 membros da equipe a um negócio.

> [!NOTE]
> Você não precisa aguardar a conclusão do processamento. Os detalhes do último arquivo processado estarão disponíveis para download quando o processamento for concluído. **Pode levar até 10 minutos se você estiver carregando arquivos com 1000 registros.**

> [!IMPORTANT]
> Leia todas as instruções cuidadosamente e verifique o formato de cada coluna da tabela abaixo antes de criar ou atualizar negócios usando arquivos CSV no Partner Center.

|**Nome da coluna**|**É obrigatório?**|**Descrição**|**Valor (es) de exemplo**|
|-----|:-----|:---------|:---|
Errors|Não|Erros se qualquer um relacionado às operações de criação/atualização w. r. t às referências será incluído nesta coluna. Se houver vários erros, todos eles serão listados separados por um ponto-e-vírgula.|Campo obrigatório solução 1 ausente|
ID do Engagement|Não|A ID do Engagement é gerada pelo sistema de referências do Microsoft Partner Center. Não é necessário para a nova criação de referência. Você pode usar a ID do Engagement existente se estiver atualizando um registro.|f7eaae47-0b84-4ac4-b4ea-5b2587d42cee
ID de referência|Não|A ID de referência é gerada pelo sistema de referências do Microsoft Partner Center. Não é necessário para a nova criação de referência. Preencha-o com a ID de referência se estiver atualizando um registro existente.|ebacdkdc-0b84-4ac4-b4ea-5b2587d42cee
Nome da negociação|Sim|O nome amigável do negócio para sua referência.|Mola do Reino Unido
Nome do Cliente|Sim|Nome da empresa do cliente. Use o nome legal da organização para correspondência rápida no lado da Microsoft.|Contoso Corporation
Linha de endereço do cliente 1|Sim|Linha de endereço 1 da empresa do cliente. |Uma maneira da contoso
Linha de endereço do cliente 2|Não|Linha de endereço 2 da empresa do cliente.|NE 148 Street
Cidade do cliente|Sim|Cidade onde a organização do cliente está localizada.|Redmond
Estado do cliente|Não|Estado em que a organização do cliente está localizada.|Washington
Código postal do cliente|Não|Código postal da região onde a organização do cliente está localizada.|98052
País/Região do cliente|Sim|País/região onde a organização do cliente está localizada. Use os códigos de país de duas letras, conforme mencionado [aqui]( https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes).|EUA
ID do cliente D-U-N-S|Não|Tente buscar a ID do DUNS da organização do cliente. Isso ajudará na correspondência mais rápida da organização do cliente no lado da Microsoft, o que ajuda a atribuir uma atribuição mais rápida ao vendedor. Você pode obter a ID do DUNS gratuitamente neste [site](https://www.dnb.com/duns-number/lookup.html).|81466849
Nome do contato do cliente|Depende|O nome só será obrigatório se você precisar da ajuda da Microsoft. O primeiro nome do contato principal da organização do cliente que está trabalhando nessa dose.|John
Sobrenome do contato do cliente|Depende|O sobrenome só será obrigatório se você precisar da ajuda da Microsoft. Sobrenome do contato principal da organização do cliente que está trabalhando nesse negócio.|Cliente
Número de telefone de contato do cliente|Depende|O número de telefone só será obrigatório se você precisar da ajuda da Microsoft. Número de telefone do contato principal da organização do cliente que está trabalhando nesse negócio.|9999999999
Endereço de email de contato do cliente|Depende|O endereço de email só será obrigatório se você precisar da ajuda da Microsoft. Endereço de email do contato principal da organização do cliente que está trabalhando nesse negócio.|john.customer@contoso.com
Status de referência do parceiro|Sim|Indica o status do negócio da perspectiva da sua empresa. Necessário se você estiver tentando criar ou modificar uma referência. Use **novo** se você estiver tentando criar um novo negócio. Os valores aceitos são documentados [aqui](https://docs.microsoft.com/partner/develop/referral-resources#referralstatus).|Ativo
Substatus de referência do parceiro|Sim|Indica o status exato do negócio. Use **aceito** se você estiver tentando criar um novo negócio. Ele também será necessário se você estiver modificando uma referência existente. Os valores aceitos são documentados [aqui](https://docs.microsoft.com/partner/develop/referral-resources#referralsubstatus).|Aceito
Status de referência da Microsoft|Depende|Indica o status da solicitação de televenda que você enviou para a ajuda de busca da Microsoft. Este é um campo somente leitura. Qualquer alteração feita nesse campo durante a importação dos dados será ignorada.| Pendente
Motivo recusado/perdido|Depende| Você precisará fornecer essas informações somente se estiver alterando o substatus do campo para recusado ou perdido. Caso contrário, você poderá ignorar essa coluna. <br/> **Insira um número com base nas opções abaixo** <br/><br/> **1**-o orçamento do projeto não é adequado  <br/> **2**-o cliente não respondeu  <br/> **3**-cliente escolheu outro fornecedor  <br/> **4** -requisito do cliente não atendido  <br/> **5** -não é um cliente <br/> **6**-a linha de tempo proposta era muito curta <br/> **7** -relatar como abuso, spam ou phishing <br/> **8** -outros |6|
Estágio de Vendas|Não|Este é o campo para indicar o estágio de vendas detalhado da referência. Leia mais sobre os estágios de vendas [aqui](https://aka.ms/salesStages)|40
Valor de negócio estimado|Sim|"O valor do acordo com base nas conversas iniciais com o cliente. Isso pode ser alterado até que o negócio atinja um dos Estados de terminal| venceu ou perdido ".|12563
Currency|Sim|A moeda na qual o valor de acordo é inserido. Você pode encontrar os códigos de moeda [aqui](https://en.wikipedia.org/wiki/ISO_4217).|USD
Data de fechamento estimada|Sim|A data de fechamento estimada do negócio com base nas conversas iniciais com o cliente no formato MM/DD/AAAA. <br/> **A data deve estar no fuso horário UTC. Todas as datas exibidas na interface do usuário do Partner Center são baseadas em fusos locais. Pode haver uma diferença de +/-um dia na interface do usuário do Partner Center se você estiver olhando para a referência para a qual forneceu a data no fuso horário UTC.**|1/30/2020
ID DO CRM|Não|Identificador dessa referência específica em seu sistema CRM, se houver. Este é um campo de entrada de texto de formato livre.|34234324-sdfsdf-345345-SFD
ID da campanha de marketing|Não|Este campo indica a campanha de marketing, que resultou nessa referência específica. Normalmente usado para cálculo de ROI|BingSummer2020
Observações|Não|Observações detalhadas indicando as atualizações relacionadas à referência|Esta é uma observação de exemplo
Ajuda da Microsoft necessária?|Sim|Isso é para indicar se você deseja que a Microsoft o ajude a fazer esta solicitação de venda|Sim
Que ajuda específica da Microsoft?|Depende|Uma das seis maneiras diferentes que a Microsoft pode ajudá-lo. Isso será aplicável somente se você escolher não para a pergunta "a ajuda da Microsoft é necessária? " <br/> **Insira um número com base nas opções abaixo** <br/><br/> **1**-proposta de valor específico de carga de trabalho  <br/> **2**-arquitetura técnica do cliente  <br/> **3**-prova de conceito de/demo  <br/> **4**-Cotações e licenciamento  <br/> sucesso do cliente de **5** pós-vendas  <br/> **6**-geral ou outro|1|
Compartilhar com a equipe de vendas da Microsoft|Sim|Isso é para indicar se você deseja compartilhar os detalhes do negócio com a equipe de vendas da Microsoft ou não. Isso será aplicável somente se você escolher não para a pergunta "a ajuda da Microsoft é necessária? "|Sim
Observações para a Microsoft|Não|Qualquer nota específica à Microsoft se você precisar de ajuda da Microsoft|Precisa de ajuda com uma POC para o cliente da contoso
Consentimento para compartilhar contato com o cliente/parceiro|Sim|Consentimento para compartilhar detalhes de contato do cliente e os funcionários de contato da empresa que estão trabalhando no negócio. **As negociações não serão criadas ou atualizadas se você escolher não para esta coluna.** |Sim
Solução 1|Sim|ID da solução (obrigatória), a moeda (opcional) na qual o valor de acordo é inserido. Você pode encontrar os códigos de moeda [aqui](https://en.wikipedia.org/wiki/ISO_4217), o preço da SKU (opcional) e a quantidade da SKU (opcional)  |SOL-1234-PQRS, USD, 10, 100
Membro da equipe 1|Sim|Nome, sobrenome, número de celular e ID de email do respectivo membro da equipe.| Bob, parceiro, 999999, Bob.partner@Contoso.com
