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
ms.openlocfilehash: 64dbbbae0087275fa8d0c5fd4f364079623efe63
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110148985"
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
|  A | 0 – 2,399    |
|  B | 2,400 – 5,999    |
|  C | 6,000 – 14,999    |
|  D | 15000 +   |

>[!NOTE]
>Os níveis de incentivos empresariais são baseados na contagem de área de trabalho ou de usuário (o que for maior) em registros de PS (setor público) e comerciais. Para registros sem contagem de desktops ou usuários associados naturais, a Microsoft aplica uma contagem de área de trabalho com base na contagem de desktops ou na contagem de usuários do EA que o acompanha. <br><br>Se não houver EA acompanhante, o nível de taxa será baseado no nível de preço do registro. O nível de preço do negócio também pode ser exibido em [www.Explore.ms](https://www.explore.ms/). <br><br>Se houver vários níveis de preço e/ou de pool no EA/EAS existente, a Microsoft pagará incentivos no nível de preço/pool mais alto atribuído, com nível um sendo o mais baixo e o nível D sendo o mais alto.

#### <a name="pool-and-pricing-levels"></a>Níveis de preço e de pool

Depois de procurar o número do contrato em explore.ms usando as etapas descritas acima, selecione o número do contrato. Isso levará você à página de detalhes do contrato, que mostrará o **Resumo do contrato** e as **ofertas**. A seção ofertas contém os níveis de preços.

## <a name="method-2---chip"></a>Método 2-CHIP

1. Entre no CHIP e selecione incentivos de LSP.

2. Na página **Resumo de pagamento do parceiro** , selecione o mês de relatório que você deseja exibir e, em seguida, selecione **detalhes de cálculo** na lista suspensa em **exportar para o Excel**:

:::image type="content" source="images/chip/chiplocate.png" alt-text="Localizar detalhes do programa":::

3. A exportação será iniciada e você poderá abrir o arquivo ou salvar/salvar como em um destino.

4. Quando o relatório estiver aberto, navegue até a guia **DetailReport-Flatfile** no canto inferior esquerdo:

:::image type="content" source="images/chip/flatfile.png" alt-text="Download de arquivo simples":::

Agora você pode pesquisar o número do contrato que está procurando na coluna J. você encontrará a contagem de área de trabalho atribuída na coluna R, rotulada Agreement_DesktopCount. Você também pode confirmar o nível de taxa deste contrato na camada rotulada da coluna ' AI '.

## <a name="next-steps"></a>Próximas etapas

- [Solucionar problemas de acesso ao CHIP](chip-access-trouble.md)
