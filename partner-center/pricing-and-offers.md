---
title: Preços e ofertas | Partner Center
ms.topic: article
ms.date: 09/26/2019
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: A lista de ofertas inclui as diferentes famílias de produtos que podem ser adquiridas por meio do Partner Center e suas informações de preços.
author: LauraBrenner
ms.author: labrenne
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: 0e81ead73308902e75b842c00bbd32ed228ca3a5
ms.sourcegitcommit: 07eb5eb6c1cfed1c84fad3626b8f989247341e70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/11/2019
ms.locfileid: "75004945"
---
# <a name="pricing-and-offers"></a>Preços e ofertas

**Aplica-se a**

-  Partner Center

**Funções apropriadas**
-   Administração global
-   Administrador de usuários
-   Agente administrativo
-   Administrador de parceiros do MPN
-   Agente de vendas
-   Administrador de cobrança

Para ver as últimas listas de preços e ofertas do programa Provedor de Soluções na Nuvem, acesse **Vender > Preços e ofertas**. Você encontrará listas de preços distintas para serviços baseados em licença, como o Office 365, o Microsoft Dynamics CRM e o Enterprise Mobility Suite, e para serviços baseados em uso, como o Azure. 

A lista de ofertas inclui as diferentes famílias de produtos que podem ser adquiridas por meio do Partner Center. Atualmente, elas incluem o Office 365, Enterprise Mobility Suite, Microsoft Dynamics CRM e Microsoft Azure. Essa lista ficará maior.

Dentro de cada uma dessas famílias de produtos há diferentes SKUs e pacotes de produtos disponíveis para venda dependendo dos seus negócios. Você pode acessar os últimos detalhes sobre cada um deles usando a Matriz de Ofertas para Revendedores de Serviços na Nuvem que está disponível na página Preços e ofertas.

## <a name="pricelist-preview-and-change-frequency"></a>Prévia da lista de preços e frequência de alteração 

Serviços baseados em licença incluem uma prévia da lista de preços, fornecida 30 dias antes de quaisquer alterações. Para acessar a prévia da lista de preços, vá para **Vender > Preços e ofertas**. Não há prévia de preços para serviços baseados em uso, pois eles são dinâmicos. A tabela a seguir explica como ler a tabela com a lista de preços.

|**Item**        |**Definição**      |
|:-----------   |:-----------   |
|ADD   |Um novo item na lista de preços|
|CHG   |Alterações no preço de lista de mês a mês. Outras alterações não relacionadas ao preço da lista podem ocorrer, os parceiros devem comparar outras propriedades do mês com o mês para determinar outras alterações.|
|DEL   |Um item removido da lista de preços|
|UNC   |Preço de lista inalterado na relação de preços do mês anterior  |
|Válido a partir de   |A primeira data em que uma oferta pode ser adquirida    |
|Válido até   |A última data em que uma oferta pode ser adquirida   |
|Nome de exibição da oferta   |O nome voltado para o cliente da oferta   |
|ID da oferta   |O identificador interno da oferta   |
|Tipo de contrato de licença   |Pode ser corporativo, governamental ou acadêmico, e determina a que tipos de clientes a oferta poderá ser vendida.|
|Unidade de compra   |A duração da oferta adquirida. Normalmente é de um mês.   |
|Tipo de licença secundária   |Poderá ser do tipo não específica, complementar ou de avaliação. O complemento indica que há produtos exigidos como pré-requisito que o cliente deve comprar antes de adquirir o complemento.|
|Tipo de cliente final   |Está relacionado ao tipo de contrato de licença: licença corporativa - revendedor de nuvem corporativo, licença governamental - revendedor de nuvem governamental ou licença acadêmica - revendedor de nuvem docente ou revendedor de nuvem estudante   |
|Preço de tabela   |O preço que o parceiro pagará   |
|Preço ERP   |O preço de varejo estimado ou recomendado para o cliente   |

## <a name="price-changes"></a>Alterações de preço

As alterações de preço são uma ocorrência comum. Os parceiros podem prever as alterações de preço para ofertas baseadas em licença examinando a visualização da lista de preços na página preços e ofertas no painel do Partner Center. O preço com base no uso do Azure não tem nenhuma versão prévia. Os parceiros podem acompanhar as alterações de preço de consumo do Azure usando a API RateCard que retorna o preço do medidor desse dia.

|**Tipo de produto**   |**Exemplos de produtos**  |**Visualização disponível** |**Alterar detalhes**|
|-----------------------|:-----------------------|:-------------------|------------------|
|Baseado em licença|Office, Dynamics, Intune, Windows Enterprise|30 dias|Listar alterações de preço marcadas como CHNG em listas de preços de visualização|
|Com base no uso|Recursos do Azure|Não disponível|Log de alterações disponível na guia **histórico de alterações** da lista de preços do mês anterior|
|Software||Não disponível|Comparar listas de preços manualmente do mês para o mês|
|Reservas|Máquinas virtuais, pré-paga|Não disponível|Comparar listas de preços manualmente do mês para o mês|

Os preços com base no uso podem ser alterados ao longo de um mês. Para obter o preço diário "atual" para esses recursos do Azure, os parceiros precisam chamar a API RateCard. 

>[!Note] 
>As alterações de preço da assinatura aplicam-se somente durante uma renovação. O custo mensal de um parceiro é determinado pelo preço da compra ou pelo preço no momento da criação de uma assinatura. Se um preço aumentar ou diminuir depois que o termo anual for adquirido, o parceiro não será cobrado pelo preço alterado até a renovação – normalmente no prazo de 12 meses.

## <a name="pricing-and-special-segments"></a>Preços e segmentos especiais

O CSP oferece alguns serviços para segmentos de mercado especiais, por exemplo, educação, não lucrativo e nuvem da Comunidade governamental. Nem todos os serviços estão disponíveis em todos os canais. Nenhum segmento assume como padrão o que chamamos de segmento ' comercial '. Todos os preços com base em licença estão disponíveis na lista de preços baseada em licença na página preços e ofertas. O preço do Azure gov está disponível na lista de preços baseada no uso quando conectado ao locatário do CSP habilitado para o Azure gov.

|**Segment**   |**Quem precisa se qualificar**   |**O parceiro qualifica o cliente**|**Tipos de produtos habilitados**|
|-------------------|-----------------------|----------------------------|-----------------------------|
|Education|Parceiro e cliente|Sim|Somente baseado em licença|
|Sem fins lucrativos|Cliente|Não, o cliente se qualifica fora do Partner Center|Somente baseado em licença|
|GCC (Government Community Cloud)|Parceiro e cliente|Após o GCC habilitado, o parceiro pode criar clientes GCC| Somente baseado em licença|
|Gov do Azure|Parceiro|Uma vez qualificado, o parceiro opera em um locatário do CSP específico para o Azure gov|Recursos do Azure|

As margens do parceiro, a diferença entre o preço da lista e os preços de varejo estimados, pode variar de segmento para segmento. Normalmente, a educação e o não-lucro tendem a ter menos ou nenhuma margem para parceiros CSP. Consulte a lista de preços baseada em licenças para obter valores exatos.  
## <a name="pricing-between-azure-and-non-azure"></a>Preços entre o Azure e não o Azure

Os preços diferem entre diferentes tipos de ofertas. O preço com base em licença normalmente é o valor por estação (licença) para um determinado mês. O preço com base no uso é determinado pelo uso de um determinado recurso, com uma ID de medição associada. Os parceiros não são cobrados pela aquisição da assinatura do Azure, mas são cobrados pelos recursos consumidos por implantações diferentes na assinatura. Os preços na lista de preços com base no uso são organizados em relação a diferentes IDs de medidor de recursos no Azure.

As reservas do Azure são compras baseadas em termos para o tipo de recurso específico – máquinas virtuais. A compra de uma reserva do Azure permite que um parceiro pague antecipadamente (termos de um ou três anos) e reserve uma determinada máquina virtual. Isso economiza o dinheiro do parceiro e garante que sua máquina virtual esteja sempre disponível durante o período. Um parceiro pode alinhar a reserva que desejam em relação às IDs de medidor de recursos com base no uso. As IDs de medidor são consistentes em todo o recurso, quer o parceiro esteja comprando uma máquina virtual ou simplesmente implantando a máquina virtual como um recurso baseado em uso. 


## <a name="offers-matrix"></a>Matriz de ofertas

Leia sobre os diferentes pacotes de produtos e SKUs disponíveis para você vender na Matriz de ofertas para revendedores de serviços na nuvem, localizada na página Preços e ofertas. A matriz de ofertas inclui quais ofertas estão disponíveis por localidade. Se um item estiver na lista de preços, mas ainda não estiver listado na matriz de ofertas, isso significa que ele ainda não pode ser adquirido. Assim que ele estiver disponível para compra, a matriz de ofertas será atualizada.

Para parceiros CSP que usam os SDKs (Software Development Kits) do Partner Center. A Microsoft também publica uma lista dos Serviços do Azure no CSP na página Preços e ofertas.

### <a name="offers-matrix-and-pricelist-questions"></a>Perguntas sobre a matriz de ofertas e a lista de preços

Se você tiver dúvidas sobre a matriz de preços ou oferta, envie uma solicitação de serviço por meio do Partner Center.
