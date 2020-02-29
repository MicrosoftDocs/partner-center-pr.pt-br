---
title: Preços e ofertas | Partner Center
ms.topic: article
ms.date: 02/27/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: A lista de ofertas inclui as diferentes famílias de produtos que podem ser adquiridas por meio do Partner Center e suas informações de preços.
author: brentserbus
ms.author: brserbus
ms.localizationpriority: medium
ms.custom: seodec18
ms.openlocfilehash: e33b89e76a57e1e6f5457e208a61bc04ad841271
ms.sourcegitcommit: 2634057663a0ea27393212f898018538dada796e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/28/2020
ms.locfileid: "78161510"
---
# <a name="pricing-and-offers"></a>Preços e ofertas

**Aplica-se a**

-  Centro de Parceiros

**Funções apropriadas**
-   Administração global
-   Administrador de usuários
-   Agente administrador
-   Administrador de parceiros do MPN
-   Agente de vendas
-   Administrador de cobrança

Para ver os mais recentes programas de provedor de soluções na nuvem e ofertas, acesse **vender > preços e ofertas**. Você encontrará listas de preços separadas para serviços baseados em licença, como o Office 365, o Microsoft Dynamics CRM e o Enterprise Mobility Suite, e para serviços com base no uso que incluem o Azure. 

A lista de ofertas inclui as diferentes famílias de produtos que podem ser adquiridas por meio do Partner Center. Atualmente, eles incluem o Office 365, Enterprise Mobility Suite, o Microsoft Dynamics CRM e o Microsoft Azure. Esta lista continuará a expandir à medida que novos produtos forem disponibilizados.

Em cada uma dessas famílias de produtos, há diferentes SKUs e pacotes de produtos disponíveis para venda, dependendo do seu negócio. Você sempre pode acessar os detalhes mais recentes sobre esses produtos usando a matriz de oferta de revendedor de nuvem, que está disponível na página preços e ofertas.

## <a name="price-list-preview-and-change-frequency"></a>Visualização da lista de preços e alteração de frequência 

Os serviços baseados em licença incluem uma visualização da lista de preços, desde 30 dias antes de qualquer alteração. Para ver a visualização da lista de preços, acesse **vender > preços e ofertas**. Não há prévia de preços para serviços baseados em uso, pois eles são dinâmicos. A tabela a seguir explica como ler a tabela de lista de preços.

|**Item**        |**Definição**      |
|:-----------   |:-----------   |
|ADICIONAR   |Um novo item à lista de preços|
|CHG   |Alterações no preço de lista de mês a mês. Outras alterações não relacionadas ao preço da lista podem ocorrer, os parceiros devem comparar as listas de preços entre meses para determinar alterações em outras propriedades.|
|DEL   |Um item removido da lista de preços|
|UNC   |Preço de lista inalterado na lista de preços do mês anterior  |
|Válido a partir de   |A primeira data em que uma oferta pode ser adquirida    |
|Válido até   |A última data em que uma oferta pode ser adquirida   |
|Nome de exibição da oferta   |O nome voltado para o cliente da oferta   |
|ID da oferta   |O identificador interno da oferta   |
|Tipo de contrato de licença   |Os tipos de contrato de licença podem ser corporativos, governamentais ou acadêmicos e determina para quais tipos de clientes a oferta pode ser vendida.|
|Unidade de compra   |A duração da oferta adquirida. As unidades de compra são normalmente um mês.   |
|Tipo de licença secundária   |Os tipos de licença secundárias serão não específicos, complementares ou de avaliação. O complemento indica que há produtos exigidos como pré-requisito que o cliente deve comprar antes de adquirir o complemento.|
|Tipo de cliente final   |Relacionado ao tipo de contrato de licença: licença corporativa – revendedor de nuvem corporativo, licença governamental – governo do revendedor na nuvem ou licença acadêmica-estudante do revendedor de nuvem ou aluno do revendedor de nuvem   |
|Preço de tabela   |O preço que o parceiro pagará   |
|Preço ERP   |O preço de varejo estimado ou recomendado para o cliente   |

## <a name="price-changes"></a>Alterações de preço

As alterações de preço são uma ocorrência comum. Os parceiros podem prever as alterações de preço para ofertas baseadas em licença examinando a visualização da lista de preços na página preços e ofertas no painel do Partner Center. O preço com base no uso do Azure não tem nenhuma versão prévia. Os parceiros podem acompanhar as alterações de preço de consumo do Azure usando a API RateCard, que retorna o preço do medidor desse dia.

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

O CSP oferece alguns serviços para segmentos de mercado especiais, por exemplo, educação, não lucrativo e nuvem da Comunidade governamental. Nem todos os serviços estão disponíveis em todos os canais. Nenhum segmento assume como padrão o que chamamos de segmento ' comercial '. Todos os preços com base em licença estão disponíveis na lista de preços baseada em licença na página preços e ofertas. Os preços do Azure governamental estão disponíveis na lista de preços baseada no uso quando conectados ao locatário do CSP habilitado para o Azure governamental.

|**Explica**   |**Quem precisa se qualificar**   |**O parceiro qualifica o cliente**|**Tipos de produtos habilitados**|
|-------------------|-----------------------|----------------------------|-----------------------------|
|Formação educacional|Cliente|Não, a qualificação do cliente será executada pela Microsoft |Somente baseado em licença|
|Sem fins lucrativos|Cliente|Não, o cliente se qualifica fora do Partner Center|Somente baseado em licença|
|GCC (nuvem da Comunidade governamental)|Parceiro e cliente|Após o GCC habilitado, o parceiro pode criar clientes GCC| Somente baseado em licença|
|Gov do Azure|Parceiro|Uma vez qualificado, o parceiro opera em um locatário do CSP específico para o Azure gov|Recursos do Azure|

As margens do parceiro, a diferença entre o preço da lista e os preços de varejo estimados, pode variar de segmento para segmento. Normalmente, a educação e o não-lucro tendem a ter menos ou nenhuma margem para parceiros CSP. Consulte a lista de preços baseada em licenças para obter valores exatos.  
## <a name="pricing-between-azure-and-non-azure"></a>Preços entre o Azure e não o Azure

Os preços diferem entre diferentes tipos de ofertas. O preço com base em licença normalmente é o valor por estação (licença) para um determinado mês. O preço com base no uso é determinado pelo uso de um determinado recurso, com uma ID de medição associada. Os parceiros não são cobrados pela aquisição da assinatura do Azure, mas são cobrados pelos recursos consumidos por implantações diferentes na assinatura. Os preços na lista de preços com base no uso são organizados em relação a diferentes IDs de medidor de recursos no Azure.

As reservas do Azure são compras baseadas em termos para o tipo de recurso específico – máquinas virtuais. A compra de uma reserva do Azure permite que um parceiro pague antecipadamente (termos de um ou três anos) e reserve uma determinada máquina virtual, economizando o dinheiro do parceiro e garantindo que sua máquina virtual esteja sempre disponível durante o período. Um parceiro pode alinhar a reserva que desejam em relação às IDs de medidor de recursos com base no uso. As IDs de medidor são consistentes em todo o recurso, quer o parceiro esteja comprando uma máquina virtual ou simplesmente implantando a máquina virtual como um recurso baseado em uso. 


## <a name="offers-matrix"></a>Matriz de ofertas

Leia sobre os diferentes pacotes de produtos e SKUs disponíveis para você vender na Matriz de ofertas para revendedores de serviços na nuvem, localizada na página Preços e ofertas. A matriz de ofertas inclui quais ofertas estão disponíveis por localidade. Se um item estiver na lista de preços, mas ainda não estiver listado na matriz de oferta, significa que os produtos ainda não podem ser ordenados. Assim que ele estiver disponível para compra, a matriz de ofertas será atualizada.

Para parceiros CSP que usam os Software Development Kits (SDKs) do Partner Center. A Microsoft também publica uma lista dos Serviços do Azure no CSP na página Preços e ofertas.

### <a name="offers-matrix-and-price-list-questions"></a>Oferece perguntas sobre matriz e lista de preços

Se você tiver dúvidas sobre a lista de preços ou a matriz de ofertas, envie uma solicitação de serviço por meio do Partner Center.

### <a name="taxes-and-pricing"></a>Impostos e preços

Todos os preços em listas de preços do CSP do Partner Center são incluídos no imposto. Para obter mais informações sobre os impostos do documento do Partner Center [e as isenções fiscais](https://docs.microsoft.com/partner-center/tax-and-tax-exemptions).
