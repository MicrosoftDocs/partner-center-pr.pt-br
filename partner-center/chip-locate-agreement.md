---
title: Encontrar contagem de área de trabalho e nível de taxa
ms.topic: how-to
ms.date: 02/18/2021
description: Saiba como usar a chip (plataforma de incentivos de canal) para encontrar as informações de nível de taxa e contagem de área de trabalho para um contrato.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 288e4ebb224d3ff1b0d4050691b733e678ec29a3
ms.sourcegitcommit: 376a49bcd245d3358a78871128761175a96ec200
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/17/2021
ms.locfileid: "112276922"
---
# <a name="locate-the-desktop-count-and-fee-level-for-an-agreement"></a>Localizar a contagem de desktops e o nível de taxas para um contrato

**Funções apropriadas:** contato principal ou administrador do programa

Você pode fazer logo [explore.ms](https://www.explore.ms/) para revisar o contrato ou baixar um arquivo que fornece detalhes do contrato para contagem de área de trabalho e nível de tarifa.

## <a name="to-locate-the-information"></a>Para localizar as informações

### <a name="method-1--explorems"></a>Método 1 – Explore.ms

1. Abra [explore.ms](https://www.explore.ms/) em Internet Explorer. 

>[!Note]
>Você não pode executar essa função no Google Chrome ou Microsoft Edge.

2. Faça logoff com sua conta de Trabalho/Escola ou ID ao vivo.  

3. No campo **Relatórios,** selecione **Contratos**.

4. Na página resultante, insira o número do contrato no **campo** Pesquisa e selecione **Selecionar/Ordenar Colunas**.

5. Na janela pop-up, selecione Contagem de **Área** de Trabalho do Contrato na lista de colunas disponíveis e, em seguida, selecione a seta para a direita para adicionar a coluna. Selecione **OK**.

6. Selecione **Pesquisar.**

7. Na tela resultante, role pelos resultados para encontrar a coluna Contagem de Área de **Trabalho do** Contrato. 

8. Use a contagem da área de trabalho para determinar o nível de taxa com base na tabela de taxa abaixo.  

| Nível de taxa | Contagem de área de trabalho |
| ------ | :-----------: |
|  Um | 0 – 2,399    |
|  B | 2,400 – 5,999    |
|  C | 6,000 – 14,999    |
|  D | 15,000+   |

>[!NOTE]
>Os níveis de Incentivo Empresarial são baseados na contagem de usuários ou área de trabalho (o que for maior) em registro de PS (Setor Comercial e Público). Para os registro sem nenhuma contagem de usuários ou área de trabalho associada natural, a Microsoft aplica uma contagem de área de trabalho com base na contagem de área de trabalho ou na contagem de usuários do EA que o acompanha. <br><br>Se não houver nenhum EA que o acompanhe, o Nível de Taxa será baseado no nível de preço do registro. O nível de preço da oferta também pode ser exibido [www.explore.ms](https://www.explore.ms/). <br><br>Se houver vários níveis de pool e/ou preços no EA/EAS existente, a Microsoft pagará incentivos no nível de preço/pool atribuído mais alto, com o nível A sendo o mais baixo e o nível D o mais alto.

#### <a name="pool-and-pricing-levels"></a>Pool e níveis de preços

Depois de pesquisar o número do contrato explore.ms as etapas descritas acima, selecione o número do contrato. Isso levará você para a página de detalhes do contrato, que mostrará o Resumo **do Contrato** e **as Ofertas**. A seção de ofertas contém os níveis de preço.

## <a name="method-2---chip"></a>Método 2 – CHIP

1. Entre no CHIP e selecione Incentivos LSP.

2. Na página **Resumo do Pagamento do** Parceiro, selecione o  mês de relatório que você deseja exibir e, em seguida, selecione Detalhes de Cálculo na lista suspenso em Exportar para **o Excel:**

:::image type="content" source="images/chip/chiplocate.png" alt-text="Localize os detalhes do programa.":::

3. A exportação será iniciar e você poderá abrir o arquivo ou salvar/salvar como em um destino.

4. Quando o relatório estiver aberto, navegue até a **guia DetailReport-FlatFile** na parte inferior inferior esquerda:

:::image type="content" source="images/chip/flatfile.png" alt-text="Download de arquivo simples.":::

Agora você pode pesquisar o número do contrato que está procurando na coluna J e encontrará a contagem de área de trabalho atribuída na coluna R, rotulada como Agreement_DesktopCount. Você também pode confirmar o Nível de Taxa para este contrato na coluna 'IA' rotulada Camada.

## <a name="next-steps"></a>Próximas etapas

- [Solucionar problemas de acesso do CHIP](chip-access-trouble.md)
