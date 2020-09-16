---
title: Taxas e impostos do serviço de PSTN regional
description: Como um parceiro do Office 365 que transatos Microsoft 365 produtos de voz, você pode estar sujeito a impostos regionais, tarifas ou requisitos regulatórios para serviços de PSTN.
ms.topic: article
ms.date: 09/10/2020
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOMAY.20
ms.openlocfilehash: 5817e5bb010cee0ab280c83408167f28915a6237
ms.sourcegitcommit: 9b36128fdbd24e4bfe4597b1e6104bd560583c5c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/15/2020
ms.locfileid: "90594451"
---
# <a name="regional-taxes-regulations-for-public-switched-telephone-network-ptsn-services"></a>Impostos regionais, regulamentos para serviços PTSN (rede telefônica pública comutada)

**Aplica-se a**

- Partner Center
- Parceiros do Office 365 transagindo Microsoft 365 produtos de voz

**Funções apropriadas**
-    Administrador global
-    Administrador de usuários
-    Agente administrativo

Os serviços de rede telefônica pública comutada (PSTN) em algumas jurisdições podem estar sujeitos a requisitos especiais de impostos e regulamentares que podem afetar a ordem e o faturamento do parceiro. No Estados Unidos, incluindo Porto Rico, os serviços PSTN, que incluem a conferência de áudio, planos de chamada e créditos de comunicação, estão sujeitos a requisitos especiais de impostos e regulamentares. No Estados Unidos e Porto Rico, a Microsoft preços os serviços PSTN como impostos sobre o imposto.  Os impostos e as regulamentações de PSTN exclusivos afetarão os parceiros do Office 365 transformando Microsoft 365 produtos de voz.  Se um parceiro marcar o preço de um serviço PSTN da Microsoft, ele poderá ser responsável pelo cálculo e remissão de impostos e taxas do PSTN.

## <a name="partner-recommendations"></a>Recomendações de parceiros

Envolva seu imposto e seu conselho jurídico para entender a responsabilidade da sua organização em relação às normas, impostos e taxas dos serviços de PSTN e a outros passivos potenciais.

## <a name="invoice-presentation-and-partner-reconciliation-file"></a>Apresentação de nota fiscal e arquivo de reconciliação do parceiro

As notas fiscais do CSP e os arquivos de reconciliação do CSP no Estados Unidos, Porto Rico e Canadá que incluem o Skype for Business PSTN e Microsoft 365 Voice Services fornecerão itens de linha separados para os componentes PSTN e não PSTN.

Além disso, as notas fiscais do CSP exibirão a seguinte nota de rodapé:

* O preço exibido é um encargo para a conferência de áudio e serviços de plano de chamada.  Todos os impostos transacionais aplicáveis são cobrados exclusivamente do valor mostrado, exceto pelas vendas feitas dentro do Estados Unidos.  Nos EUA, o preço exibido é imposto inclusivo, pois inclui um encargo para o plano de chamada e os serviços de conferência de áudio e um encargo para os impostos e as tarifas que precisaremos cobrar.  A conferência de áudio e os serviços de plano de chamada são atendidos pela afiliada da Microsoft autorizada a fornecê-los.  Confira [Licenciamento por Volume da Microsoft](https://go.microsoft.com/fwlink/?LinkId=690247).

## <a name="reconciliation-file-example"></a>Exemplo de arquivo de reconciliação

O Office 365 Enterprise E5 apresenta o arquivo de reconciliação como dois itens de linha com nomes idênticos e IDs idênticas, mas cada item de linha tem um preço unitário exclusivo (exemplo: $28.40 e $2). Isso separa o componente Conferência do Skype for Business da oferta do Office 365, portanto, você pode aplicar impostos corretamente.

**Exemplo de reconciliação de parceiro #1 (selecionar colunas):**

|**ID_oferta_durável**|**Offer_Name**|**Subscription_Start_Date**|**Subscription_End_Date**|**Charge_Start_Date**|**Charge_End_Date**|**Charge_Type**|**Unit_Price**|
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00|9/10/2019 0:00   |Taxa do Ciclo   |28,40   |
|a044b16a-1861-4308-8086-a3a3b506fac2   |Office 365 Enterprise E5   |8/10/2019 0:00   |8/11/2019 0:00   |8/11/2019 0:00   |9/10/2019 0:00   |Taxa do Ciclo   |2,00   |

**Exemplo de reconciliação de parceiro #2**

Microsoft 365 Business voz disponível no Canadá tem componentes adicionais de PSTN que são consolidados na nota fiscal do CSP (semelhante ao Office 365 e5, dois itens de linha são apresentados, um para componentes PSTN e outro para componentes não PSTN).  O arquivo de reconciliação CSP para Microsoft 365 Business voz exibirá todos os componentes tributáveis de PSTN individualmente (componentes PSTN individuais não serão consolidados no. Ferramenta de API ou CSV).  A soma dos detalhes do pedido e dos valores cobrados para os clientes encontrados no arquivo de reconciliação corresponderá à nota fiscal do CSP.

## <a name="additional-resources"></a>Recursos adicionais
Para obter mais detalhes, visite o site [Microsoft 365 para parceiros](https://www.microsoft.com/microsoft-365/partners/) .

