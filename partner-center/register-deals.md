---
title: Registre suas negociações
ms.topic: article
ms.date: 06/29/2021
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Quando você registra um negócio que ganhou no Partner Center, isso ajuda a Microsoft a fornecer mais oportunidades no futuro.
author: rajap-ms
ms.author: rajap
ms.localizationpriority: medium
ms.openlocfilehash: eaa9bb6f8e57033669ef584e7c52c0d050a532e0
ms.sourcegitcommit: 8235c89e789cdb5115fc1c19151fa8e97c743fe5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "113080649"
---
# <a name="register-deals-youve-won-in-partner-center"></a>Registre as negociações que você ganhou Partner Center

**Funções apropriadas**: Administrador de indicações

Você pode registrar negociações que ganhou no Partner Center fornecendo mais informações sobre o contrato. Essas informações nos ajudam a oferecer mais oportunidades para você no futuro.

Há dois caminhos que levam ao registro de negociação:

- Você criou uma nova oferta na seção Oportunidades de venda em **cooperação** e sua oferta atende aos critérios de registro de oferta.
- Você deseja relatar um negócio fechado do ISV Connect, que não foi vendido em cooperação com a Microsoft.

## <a name="register-a-deal-originating-from-a-co-sell-opportunity"></a>Registrar uma oferta originada de uma oportunidade de venda em cooperação

Se você estiver procurando registrar uma negociação originada de uma oportunidade de venda reversível, sua oferta deverá atender aos seguintes requisitos de qualificação:

- O tipo de negociação é co-venda ou por parceiro (você optou por permitir que os vendedores da Microsoft exigam essa oferta).
- Há pelo menos uma solução qualificada para incentivos na oferta. Uma solução será qualificada para incentivos se contiver pelo menos uma das seguintes marcas:
  - Venda co-venda de IP do Azure
  - Business Applications Premium
  - Business Applications Standard
- O status do negócio é "Won".
- Se o tipo de oferta for venda em cooperação, a Microsoft deverá ter aceito o convite ou marcado como ganho. Você pode ver o status da Microsoft observando o cartão da Microsoft abaixo dos detalhes do acordo.

Se você tiver atendido aos requisitos de qualificação, será solicitado **automaticamente** que registre seu negócio com um botão Registrar agora mostrado na barra de progresso do negócio:

:::image type="content" source="images/register-deals.png" alt-text="Captura de tela mostrando a barra de progresso do negócio.":::

> [!NOTE]
> Se o item **de registro deal** não aparecer na barra de progresso do acordo para seu negócio, a oferta não atenderá a todos os requisitos para o registro de negociação.

Depois de **clicar** em Registrar agora , você será redirecionado para a página Registro de Oferta e solicitado a preencher um formulário com o qual inclua informações preenchidas previamente para seu cliente e solução. Preencha o formulário usando as instruções abaixo e clique em **Registrar**.

Após o registro, haverá um ou dois registros de registro de negociação criados dependendo da solução.

- Se sua solução estiver qualificada para o ISV Connect, um registro de registro de negociação do ISV Connect será criado. Esse registro de negociação será usado para faturamento.
- Se sua solução estiver qualificada para incentivos de venda de IP, um registro de registro de oferta de venda de venda de IP será criado. Esse registro de negociação será revisado e aprovado ou rejeitado pela equipe de revisão de negociação de venda em cooperação.

## <a name="report-a-closed-isv-connect-deal"></a>Relatar um negócio fechado do ISV Connect

Para relatar um negócio fechado do ISV Connect, vá para a guia Registro **de** negociação e clique **em + Relatório fechado oferta do ISV Connect**. Preencha os campos necessários e clique em **Registrar**. Esse registro de negociação será usado para faturamento.

## <a name="fill-out-the-deal-registration-form"></a>Preencha o formulário de registro de negociação

> [!NOTE]
> Você pode filtrar as negociações por nome do cliente, status e tipo de acordo. Para fazer isso, clique no **botão Filtrar** na parte superior da página Registro de Oferta.

Se você tiver vindo para lidar com o registro de uma oportunidade de venda em cooperação ou se está relatando uma negociação fechada do ISV Connect, que não foi vendida em cooperação com a Microsoft, você será solicitado a preencher os campos a seguir no formulário de registro de negociação.

- **Detalhes do** cliente: insira o **Nome da empresa** para seu cliente e selecione seu **País/Região.** Em seguida, insira a **Cidade** e o **Estado/província** dele(a).
- **Solução:** selecione a solução que será usada para a negociação. Se você não vir a solução correta listada, entre em contato com o suporte.
- **Tipo de** contrato: especifique se essa oferta é um **Novo** contrato ou uma **Renovação** de um contrato anterior.
- **Valor total do contrato:** o valor total esperado para a participação. Esse valor deve incluir todos os valores de software e serviço, mas não os custos de hardware. Selecione a moeda adequada.
- **Valor da** solução: o valor total da solução de nuvem que será usada para o negócio. Inclua todos os valores associados às tarifas de software e de manutenção, mas não inclua itens reembolsáveis, valores de personalização não recorrentes ou valores de licença do CSP associados diretamente pagos pela Microsoft.
- **A solução será implantada no Azure? Caso contrário, escolha Outro:** selecione **Azure** ou **Outro.**
- **O consumo da solução será executado no** locatário do parceiro ou no locatário do cliente? : selecione o locatário cliente **ou** o **locatário do parceiro**.
- **Data de início do** contrato: a data em que o contrato será iniciada. Para ofertas pay-as-you-go (PAYG), use a data da primeira fatura. Por design, Partner Center permitirá que você insira uma data de início anterior à data de assinatura do contrato. Isso pode afetar alguns acordos, como implantações de IP que começam antes da data de assinatura. Para inserir essas negociações com êxito, use  a data de assinatura do contrato para os campos de data de assinatura e data de início quando você estiver enviando. (O contrato deve explicitamente sinalizar a duração da negociação para que o ACV possa ser calculado corretamente.)
- **Data de término do** contrato: se o contrato terminar em uma data específica, selecione Tem **uma data de término** e forneça essa data. Se o contrato não tiver uma data de término específica, selecione **Perpétuo.** Para ofertas pay-as-you-go (PAYG), use a data da última ou mais recente fatura.
- **Data de assinatura do** contrato: a data em que o contrato final foi assinado pela sua organização e pelo cliente. Para ofertas pay-as-you-go (PAYG), use a data da primeira fatura.
- **Contato de** registro: **o** nome **,** **sobrenome,** número de telefone e **Email** para uma pessoa em sua organização que possamos contatar se precisarmos de mais detalhes sobre qualquer uma das informações fornecidas aqui.

Quando tiver concluído todas as seções da página, clique em **Registrar**.

- Se a oferta for uma oferta do ISV Connect, você observará que o status da oferta é "Enviado, Concluído". Não há mais nenhuma ação necessária nesse registro de registro de negociação. Esse registro será usado para faturamento.
- Se a oferta for uma venda de venda de IP, você observará que o status da oferta é "Enviado". A equipe de revisão de negociações de venda co-venda da Microsoft revisará as informações fornecidas neste registro de negociação. A equipe de revisão solicitará mais ação de você, se necessário, ou aprovará/rejeitará o acordo diretamente.
- Se você estiver registrando uma oferta originada de uma oportunidade de venda em cooperação e vir que dois registros de registro de negociação foram criados, isso significa que a solução em seu negócio está qualificada para o ISV Connect e para a venda de IP. O registro do ISV Connect será usado para faturamento. O registro de venda co-venda de IP será revisado pela equipe de validação de negociação de venda em conjunto.

