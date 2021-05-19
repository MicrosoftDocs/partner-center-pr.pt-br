---
title: Consolidação de locatários de autorização regional do CSP
ms.topic: how-to
ms.date: 07/15/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Use estas instruções para consolidar locatários para países/regiões diferentes. Isso inclui etapas para migrar contas de clientes e assinaturas de clientes.
author: billLinzbach
ms.author: billLi
ms.localizationpriority: medium
robots: noindex,nofollow
ms.custom: SEOMAY.20
ms.openlocfilehash: d2168dcd60b8675a21960918dab49b778025fa51
ms.sourcegitcommit: 7063fdddee77ad2d8e627ab3c806f76d173ab652
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2021
ms.locfileid: "110147574"
---
# <a name="instructions-for-csp-regional-authorization-tenant-consolidation"></a>Instruções para a consolidação de locatários de autorização regional do CSP

**Aplica-se a**: Partner Center | Partner Center for Microsoft Cloud for US Government

**Funções apropriadas:** administrador global | Agente administrador

\[Algumas informações estão relacionadas ao produto pré-lançado, que pode ser substancialmente modificado antes de ser lançado comercialmente. A Microsoft não oferece garantias, expressas ou implícitas, das informações aqui fornecidas.\]

Você pode consolidar locatários para sua empresa. Use estas instruções para consolidar locatários para países/regiões diferentes.

>[!NOTE]  
>Você deve estar ciente de todas as assinaturas provisionadas e contagens de licença para cada um de seus clientes na conta da sua transição. Você provisionará essas mesmas assinaturas exatas com as mesmas contagens de licença na nova conta central do CSP como parte do processo de migração. Use o recurso de lista de exportação para ajudar a criar uma lista de clientes para mover para o locatário centralizado.  Depois que a consolidação for concluída, você não poderá reverter para o estado do locatário anterior. A ação do cliente também pode ser necessária.

## <a name="prepare-for-migration"></a>Preparar para a migração

- Entre no **Partner Center** usando a  conta transição (aquela que você fará a transição para a nova conta) e revise todos os clientes e todos os serviços provisionados para esses clientes.

- Saia dessa conta.

## <a name="migrate-customer-accounts"></a>Migrar contas de clientes

1. Entre no **Partner Center**  com a **conta** Transição (nova) (aquela para a qual você está fazendo a transição de clientes).

2. Selecione **Clientes**.

3. Selecione **Solicitar uma relação de revendedor.** Você receberá uma mensagem de email padrão para enviar aos seus clientes. Essa mensagem contém uma URL com a ID da organização exclusiva para sua nova conta do Partner Center.

4. **Ação do cliente:** Certifique-se de que cada um dos clientes ativos que você deseja migrar visite essa URL. Ao abrir a URL, o cliente será solicitado a entrar no portal do Office 365. O cliente entra usando a mesma ID da organização que ele usa para acessar os portais de administrador do Azure e do Office 365.

5. Depois de entrar, o  Administrador Global da conta do cliente será solicitado a enviar um contrato que dê privilégios de administrador delegado à nova conta do CSP. Se concordar, o cliente marca a caixa de seleção e concorda em autorizar o relacionamento.

Os clientes aparecerão na lista de clientes do parceiro depois de enviarem o contrato, um por um.

## <a name="migrating-office-365-and-non-azure-usage-based-subscriptions"></a>Migrando assinaturas baseadas em uso do Office 365 e não Azure

1. Depois que o cliente assinar o contrato, você poderá recriar as assinaturas dele em seu locatário parceiro centralizado.

2. No **Partner Center**, selecione **Clientes**.

3. Abra o nome da empresa do cliente que você deseja migrar.

4. Selecione **Adicionar assinatura**.

5. Adicione as assinaturas e contagens de licença corretas do catálogo. Verificar com as informações fornecidas nas contas de parceiro de **origem da transição**.

   :::image type="content" source="images/regionalcustomer2.png" alt-text="lista de clientes":::

6. Selecione **Enviar.**

   Agora os serviços serão fornecidos para o cliente da conta de parceiro de **destino da transição**.

7. Repita essas etapas para migrar assinaturas para todos os outros clientes.

Antes de prosseguir para a próxima seção, certifique-se de que todas as assinaturas de cliente existentes nas contas de parceiros de **origem da transição** sejam reprovisionadas sob a conta de parceiro de **destino da transição**.

> [!NOTE]
> Os parceiros devem suspender as assinaturas na **transição da conta de locatário do** parceiro no centro de parceiros no mesmo dia em que essas assinaturas são transferidas e configuradas na **transição para** a conta de locatário do parceiro no Partner Center para garantir que a cobrança dupla não ocorra. As solicitações de suporte serão negadas para créditos devido a qualquer sobreposição na cobrança que ocorre de não desabilitar corretamente a **transição de** assinaturas.

## <a name="disabling-the-office-365-subscriptions-under-the-transitioning-from-partner-account"></a>Desabilitando as assinaturas do Office 365 na conta de parceiro de origem da transição

Desabilitar a assinatura de CSP sob as contas de parceiros de **destino da transição** impede qualquer cobrança futura. Você não precisa desabilitar manualmente as assinaturas do Azure, pois as assinaturas do Azure são automaticamente desabilitadas durante o processo de migração.

1. Entre no **Partner Center** com a **transição da conta do** CSP e navegue até a lista de clientes.

2. Abra o cliente com assinaturas para desabilitar e, em seguida, selecione a primeira oferta a ser desabilitada.

3. Defina a assinatura como **suspensa** e, em seguida, selecione **Enviar**.

   >[!Note]
   >A suspensão da assinatura garante que a cobrança dupla não ocorra.

   A assinatura mostra **suspensa** na lista de assinaturas.

4. Repita essas etapas para todas as assinaturas sob o cliente. Verifique se todas são exibidas como **suspensas**.

5. Selecione o próximo cliente na lista e repita o processo para desabilitar todas as assinaturas.

## <a name="migrating-azure-usage-based-subscriptions"></a>Migrando assinaturas baseadas em uso do Azure

Ao contrário das assinaturas do CSP do Office 365, as assinaturas do CSP com base no uso do Azure não precisam ser migradas manualmente. Microsoft Azure suporte irá migrar as assinaturas do Azure e todos os serviços ou recursos implantados da **transição de contas de** revendedor do CSP para a **transição para** a conta de revendedor do CSP. Não haverá qualquer interrupção do serviço para o cliente durante a transição.

1. Verifique se as contas de cliente que terão as assinaturas do Azure migradas aceitaram o contrato a ser associado à nova **transição para** a conta do CSP.

2. Você notificará a Microsoft de quais contas de clientes estão prontas para migrar e fornecerá os nomes de empresa do cliente.

3. A Microsoft migra as assinaturas baseadas em uso do Azure e notifica você quando a migração é concluída.

4. Você precisa confirmar se a assinatura do Azure na **transição da conta de** revendedor do CSP agora está marcada como **suspensa** no Partner Center na seção assinaturas do cliente.

5. Confirme se a assinatura do Azure na conta do revendedor  Transição para **CSP** agora mostra um status ativo no Partner Center na seção assinaturas do cliente.

   >[!Note]
   > Desabilitar as assinaturas no cliente não altera a aparência do cliente na lista Clientes. Atualmente, não há uma opção para remover clientes da lista. Os parceiros devem evitar readicionar assinaturas para esses clientes a partir da conta de **destino da transição** no futuro.

6. Repita essas etapas para todas as assinaturas em todos os seus clientes para impedir encargos futuros nas contas de **origem da transição**. O parceiro receberá uma fatura final com um crédito pelo número de dias não utilizados entre o dia de cancelamento e o último dia do período de cobrança. Nenhuma fatura futura será gerada após esse período de cobrança final.

### <a name="additional-information"></a>Informações adicionais

- Desabilitar a assinatura da conta de Transição do **CSP** não afeta o serviço do cliente final, desde que o serviço seja provisionado da conta de Transição para **o** CSP antes de desabilitar a assinatura.

- As assinaturas não podem ser usadas pelo cliente e não geram encargos quando suspensos ou cancelados.

- Atualmente, não há nenhuma maneira de remover completamente um cliente da **lista Clientes.**
- 
    >[!Note]
    > Os parceiros devem suspender  assinaturas na conta de locatário transição do parceiro no Partner Center mesmo dia  em que essas assinaturas são transitivas e configuradas na conta Transição para para garantir que a cobrança dupla não ocorra. A Microsoft não dará suporte a solicitações de créditos devido a qualquer  sobreposição na cobrança que ocorre por não definir corretamente a transição de assinaturas para suspensa.

### <a name="simplify-migration-using-export"></a>Simplificar a migração usando Exportar

Usando a **função Exportar**, você pode capturar as assinaturas que serão usadas em sua nova estrutura consolidada:

1. Selecione **Clientes** no Partner Center para ver a lista de clientes. 

2. Abra o nome do cliente desejado.

3. Na página **Assinaturas,** selecione **Exportar Assinaturas** para exportar detalhes de assinaturas para um arquivo do Excel.

4. Use essa lista para recriar as assinaturas em seu novo locatário consolidado.

### <a name="api-registration"></a>Registro de API

Para obter mais informações sobre o registro de API, consulte [Configurar o acesso à API no Partner Center](/partner-center/develop/set-up-api-access-in-partner-center).

## <a name="next-steps"></a>Próximas etapas

- [Provedor de Soluções na Nuvem mercados regionais e moedas em que você pode vender ofertas do CSP](regional-authorization-overview.md)
