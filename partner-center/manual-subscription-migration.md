---
title: Migrar assinaturas do Dynamics AX para o Dynamics 365 | Partner Center
description: "A Microsoft apresenta o Dynamics 365, a mais nova geração de aplicativos de negócios inteligentes que permitem que sua organização cresça, evolua e transforme-se para atender às necessidades de seus clientes e aproveitar novas oportunidades."
ms.assetid: 79787bef-a6e9-4c11-8c3b-f0a77485c0a4
author: MaggiePucciEvans
ms.openlocfilehash: f19e46da31a7e479ebd3b1cd368ca7646c3c55b7
ms.sourcegitcommit: 772577c0538a5d5b05d45f0e669697209761ab03
translationtype: HT
---
# <a name="migrate-dynamics-ax-subscriptions-to-dynamics-365"></a>Migrar assinaturas do Dynamics AX para o Dynamics 365

**Aplicável a**

-  Partner Center

A Microsoft apresenta o Dynamics 365, a mais nova geração de aplicativos de negócios inteligentes que permitem que sua organização cresça, evolua e transforme-se para atender às necessidades de seus clientes e aproveitar novas oportunidades. Como parte do novo produto, a Microsoft apresenta novos planos de assinatura do Microsoft Dynamics para clientes em 1º de novembro de 2016, que são semelhantes, mas não idênticos aos seus planos atuais.

As instruções neste documento descrevem como provedores indiretos podem migrar as assinaturas existentes do Microsoft Dynamics AX dos clientes para o novo Microsoft Dynamics 365. As instruções também se aplicam a outros produtos da Microsoft que são atualizados para novas versões, exigindo que os provedores migrem as assinaturas dos clientes para uma nova SKU.

**Alterações de licenciamento do Microsoft Dynamics AX**

A linha de produtos Microsoft Dynamics AX foi desativada, em vigor a partir de 1º de novembro de 2016. Para saber mais sobre as novas opções de licenciamento do Dynamics 365, leia o próximo Guia de Licenciamento que será publicado em breve. Consulte a tabela a seguir para obter detalhes sobre o mapeamento de licenças:

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Licença desativada do Dynamics AX</strong></p></td>
<td><p><strong>Licença do Dynamics 365</strong></p></td>
</tr>
<tr class="even">
<td><p>Dynamics AX Enterprise</p></td>
<td><p>Edição Enterprise do Dynamics 365 Plano 2</p>
<p>OU Dynamics 365 for Operations</p></td>
</tr>
<tr class="odd">
<td><p>Dynamics AX Task</p></td>
<td><p>Dynamics 365 for Team Member</p></td>
</tr>
<tr class="even">
<td><p>Dynamics AX Functional</p></td>
<td><p>Dynamics 365 for Team Member</p></td>
</tr>
<tr class="odd">
<td><p>Dynamics AX Device</p></td>
<td><p>Dynamics 365 for Operations Device</p></td>
</tr>
</tbody>
</table>

 

**Microsoft Dynamics CRM Online**

A partir de 1º de novembro de 2016, o plano Microsoft Dynamics CRM Online atual estará desativado. Consulte [Informações importantes para clientes do CRM Online](https://go.microsoft.com/fwlink/?linkid=831667) para saber mais sobre as novas opções de licenciamento.

## <a name="transition-customers-to-new-product-plans"></a>Transição dos clientes para novos planos do produto


A Microsoft oferece continuamente novos produtos e serviços para revendedores e provedores. Nesses casos, talvez o revendedor precise fazer o upgrade dos clientes para novos serviços ou migrar as assinaturas de SKUs que serão encerradas em breve. A migração dos clientes de SKUs antigas para as mais recentes requer a seguinte sequência:

-   [Comprar a nova assinatura](#manual-subscription-migration-purchasenewsubsc);
-   [Reatribuir as licenças de usuário atuais](#manual-subscription-migration-reassignlicenses);
-   [Cancelar a assinatura antiga](#manual-subscription-migration-cancelsubscriptions).

Nos procedimentos a seguir, você migrará um cliente do Dynamics AX7 Enterprise para o Dynamics 365 for Operations.

<a href="" id="purchasenewsubsc"></a>O revendedor precisa migrar o cliente com uma assinatura existente do Dynamics AX Enterprise para o Dynamics 365 for Operations. A primeira etapa é comprar o Dynamics 365 for Operations.

**Comprar a nova assinatura**

1.  No menu **Painel**, selecione **Clientes**, selecione o cliente para o qual você deseja fazer a migração e escolha **Adicionar Assinaturas**.
2.  Selecione a assinatura que deseja comprar no catálogo (nesse caso, Dynamics 365 for Operations, Enterprise Edition), insira o número de licenças e escolha **Enviar**.

    Agora seu cliente deve ter assinaturas novas e antigas: neste exemplo, o antigo Dynamics AX Enterprise, e a nova assinatura de "destino", Dynamics 365 for Operations, Enterprise Edition.

<a href="" id="reassignlicenses"></a> A próxima etapa é reatribuir todas as licenças de usuário existentes para a nova assinatura.

**Reatribuir licenças de usuário**

1.  No menu **Painel**, selecione **Clientes**, selecione o cliente para o qual deseja fazer a migração e escolha **Usuários e licenças**. A página Usuários e Licenças do cliente será aberta.
2.  Para reatribuir licenças de usuário, selecione o usuário a ser reatribuído e selecione **Gerenciar licenças**.
3.  Na página **Gerenciar licenças**, desmarque a caixa de seleção da licença **Dynamics AX Enterprise** e selecione a licença **Dynamics 365 for Operations**.
4.  Selecione **Enviar**. Uma página de confirmação lista as novas atribuições de licença.
5.  Siga as mesmas etapas com outros usuários do cliente que precisam de reatribuição de licença.

<a href="" id="cancelsubscriptions"></a> Depois de migrar as licenças de usuário para o novo serviço, você pode cancelar com segurança a assinatura antiga no nível superior do cliente.

**Cancelar a assinatura antiga**

1.  No menu **Painel**, selecione **Clientes**, selecione o cliente para o qual você deseja fazer a migração e a assinatura que deseja cancelar.
2.  Na página de detalhes da assinatura, defina o **Status** da assinatura para **Suspensa**.
3.  Selecione **Enviar**.

A assinatura antiga será suspensa e a nova assinatura será ativada. A assinatura suspensa será desprovisionada automaticamente após 120 dias. O cliente não pagará custos adicionais pela assinatura antiga.

## <a name="additional-considerations"></a>Considerações adicionais


Se o cliente for migrar do Programa Open Channel para o Programa de Serviços na Nuvem para mais provisionamento de assinaturas, você também precisará migrar as assinaturas existentes dele:

-   Se o cliente tiver recebido a assinatura antiga pelo Open Channel, a migração do CSP para a nova SKU será simples.
-   Se o cliente ainda não estiver estabelecido como seu cliente, você poderá convidá-lo. Para obter informações, consulte o tópico de ajuda [Solicitar uma relação com um cliente](https://msdn.microsoft.com/en-us/library/partnercenter/mt750320.aspx).

Depois que o cliente aceitar você como seu provedor indireto, as etapas de provisionamento serão basicamente as mesmas que foram descritas acima: você compra a nova assinatura e depois atribui as licenças de usuário. A única diferença envolve o cancelamento de assinaturas antigas. Um novo provedor não pode suspender/cancelar assinaturas adquiridas por meio de outros canais. Se o cliente tiver adquirido assinaturas anteriores em outro canal de vendas, como o Open Channel, ele precisará cancelá-las por meio desse canal.

 

 



