---
title: Localizar contagem de área de trabalho e nível de taxa
ms.topic: how-to
ms.date: 02/18/2021
description: Saiba como usar a plataforma de incentivos de canal (CHIP) para localizar a contagem de desktops e as informações de nível de taxa de um contrato.
ms.service: partner-dashboard
ms.subservice: partnercenter-incentives
author: Karthic83
ms.author: kashanum
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: e433b44f158c3e4cefe22027e7f7d3b845991308
ms.sourcegitcommit: bff907bdbddc769716c7418a2b4a94ca37c2d590
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/03/2021
ms.locfileid: "101756115"
---
# <a name="locate-the-desktop-count-and-fee-level-for-an-agreement"></a>Localizar a contagem de desktops e o nível de taxas para um contrato

**Funções apropriadas**

- Administrador primário de contato ou programa

Você pode fazer logon no [Explore.ms](https://www.explore.ms/) para revisar o contrato ou baixar um arquivo fornecendo detalhes do contrato para contagem de desktops e nível de taxa.

## <a name="to-locate-the-information"></a>Para localizar as informações

### <a name="method-1--explorems"></a>Método 1 – Explore.ms

1. Abra o [Explore.ms](https://www.explore.ms/) no Internet Explorer. 

>[!Note]
>Não é possível executar essa função no Google Chrome ou no Microsoft Edge.

2. Faça logon com sua conta corporativa/de estudante ou Live ID.  

3. No campo **relatórios** , selecione **contratos**.

4. Na página resultante, insira o número do contrato no campo de **pesquisa** e selecione colunas de **selecionar/ordenar**.

5. Na janela pop-up, selecione **contagem de áreas de trabalho de contrato** na lista colunas disponíveis e, em seguida, selecione a seta para a direita para adicionar a coluna. Selecione **OK**.

6. Selecione **Pesquisar.**

7. Na tela resultante, percorra os resultados para localizar a coluna **contagem de área de trabalho do contrato** . 

8. Use a contagem de desktops para determinar o nível de taxa com base na tabela de taxas abaixo.  

| Nível de taxa | Contagem de desktops |
| ------ | :-----------: |
|  A | 0 a 2.399    |
|  B | 2.400 – 5.999    |
|  C | 6.000 – 14.999    |
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
