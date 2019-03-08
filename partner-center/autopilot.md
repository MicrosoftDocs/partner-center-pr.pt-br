---
title: Personalizar a experiência de out-of-box do dispositivo com perfis do Windows Autopilot | Partner Center
description: Pré-configure a experiência de out-of-box do dispositivo com perfis do Autopilot.
ms.topic: article
ms.date: 02/06/19
author: maggiepuccievans
ms.author: evansma
keywords: piloto automático, do windows autopilot, piloto automático da microsoft, implantação zero-touch, oobe, telas de logon, out-of-box
ms.localizationpriority: medium
ms.openlocfilehash: 00c4bc3717b5f40984f60dd2c04ee7fec10b80da
ms.sourcegitcommit: 4c34d6fcaf020bcc53eaa5f0379011a56149a14f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2019
ms.locfileid: "57586909"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a>Personalizar a experiência de out-of-box do dispositivo com perfis do Windows Autopilot

**Aplica-se a**

- Os parceiros CSP direto fatura, provedores indiretos e revendedores indiretos

Se você gerenciar dispositivos de cliente, você talvez precise personalizar a experiência de out-of-box (OOBE) para usuários do cliente. Você pode pré-configurar novos dispositivos com perfis do Windows Autopilot antes de entregar os dispositivos para os clientes e aplicar novos perfis em dispositivos clientes já tem comprado. Este artigo explica como criar e aplicar os perfis do Autopilot para dispositivos no Partner Center.

Se você não ainda estiver familiarizado com o piloto automático, examine as informações nesses artigos:

- [Visão geral do Windows Autopilot.](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [Guia de referência de implantação do AutoPilot](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>Visão geral

Com o recurso do Windows Autopilot no Partner Center, você pode criar perfis personalizados para se aplicam a dispositivos de cliente. As seguintes configurações de perfil estavam disponíveis no momento em que este artigo foi publicado em:

- Ignorar configurações de privacidade. Essa configuração de perfil do Autopilot opcional permite que as organizações não pergunte sobre as configurações de privacidade durante o processo OOBE.

- Desabilite a criação da conta de administrador local no dispositivo. As organizações podem decidir se a configuração do dispositivo de usuário deve ter acesso de administrador quando o processo for concluído.

- Configure automaticamente o dispositivo para o trabalho ou escola. Todos os dispositivos registrados com o Autopilot serão automaticamente considerados trabalho ou escola de dispositivos, portanto, essa questão não será solicitado durante o processo OOBE.

- Ignorar as páginas de configuração de registro de OEM, OneDrive e Cortana. Todos os dispositivos registrados com o Autopilot ignorará automaticamente essas páginas durante o processo de out-of-box experience (OOBE).

- Ignore o contrato de licença de usuário final (EULA). Começando no Windows 10 versão 1709, as organizações podem optar por ignorar a página de EULA apresentada durante o processo OOBE. Ver [exoneração do EULA do Windows Autopilot](#windows-autopilot-eula-dismissal) abaixo para obter informações importantes a considerar sobre como ignorar a página de EULA Windows durante a instalação.

As seguintes permissões de gerenciamento de dispositivo e de perfil e limitações se aplicam:

- Os parceiros CSP podem continuar a gerenciar os perfis do Autopilot para os clientes existentes com os quais eles têm relações de revendedor, mesmo se os clientes removeu os privilégios de administração delegada do parceiro.

- Você pode gerenciar os dispositivos existentes para os clientes que foram adicionados por você ou por outro parceiro CSP.

- Você não pode gerenciar dispositivos de que seu cliente tiver carregado para a Microsoft Store for Business ou o Portal do Microsoft Intune.

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>Criar e gerenciar perfis do Autopilot no Partner Center

No Partner Center, você pode criar perfis de implantação do Windows Autopilot e aplicá-las a dispositivos.

>[!NOTE]
>Somente os agentes administradores podem criar e aplicar perfis.

### <a name="create-a-new-autopilot-profile"></a>Criar um novo perfil do Autopilot

1. Selecione **clientes** no menu do Partner Center e em seguida, selecione o cliente você está criando o perfil do Autopilot.

2. Na página de detalhes do cliente, selecione **dispositivos**.

3. Sob **perfis do Windows Autopilot** selecionar **adicionar novo perfil**.

4. Insira o nome e uma descrição do perfil e, em seguida, defina as configurações de OOBE. Escolha entre:  

   - Ignorar configurações de privacidade na instalação

   - Desabilitar a conta de administrador local na instalação
  
   - Ignorar automaticamente as páginas na instalação<br>
        (Inclui *automaticamente Selecionar configuração de trabalho ou escola* e *páginas de configuração de registro de Skip Cortana, o OneDrive e o OEM*)
  
   - Ignorar o contrato de licença de usuário final (EULA)<br> 
       >[!IMPORTANT] 
       >Ver [exoneração do EULA do Windows Autopilot](#windows-autopilot-eula-dismissal) abaixo para obter informações importantes a considerar sobre como ignorar a página de EULA Windows durante a instalação.

5. Selecione **Enviar** quando terminado.

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>Aplicar um perfil do Autopilot para dispositivos cliente

>[!NOTE]
>As instruções abaixo pressupõem que você já adicionou os dispositivos do cliente ao Partner Center e que você pode acessar sua lista de dispositivos. Se você já não tiver adicionado os dispositivos do cliente, siga as instruções em [adicionar dispositivos para uma conta de cliente](#add-devices-to-a-customers-account) e, em seguida, siga as etapas abaixo.

Depois de criar um perfil do Autopilot para um cliente, você pode aplicá-lo a dispositivos do cliente.

1. Selecione **clientes** no menu do Partner Center e em seguida, selecione o cliente é criado para o perfil do Autopilot.

2. Na página de detalhes do cliente, selecione **dispositivos**.

3. Sob **aplicar perfis de dispositivos** selecione os dispositivos ou grupos de dispositivos que você deseja adicionar os perfis para e, em seguida, selecione **aplicar perfil**. O perfil que você acabou de ser aplicado aparecerá na **perfil** coluna.

4. Siga as etapas abaixo para verificar que o perfil será aplicado com êxito para o dispositivo.

    a.  Conectar um dispositivo à rede e ativá-lo.

    b.  Verifique se aparecem as telas OOBE apropriadas (se existirem).

    c.  Quando o processo OOBE é interrompida, redefina o dispositivo para as configurações padrão de fábrica para prepará-lo para um novo usuário.

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>Remover um perfil do Autopilot de dispositivo do cliente

1. Selecione **clientes** no menu do Partner Center e em seguida, selecione o cliente é criado para o perfil do Autopilot.

2. Na página de detalhes do cliente, selecione **dispositivos**.

3. Sob **aplicar perfis de dispositivos** selecione os dispositivos que você deseja remover o perfil do e, em seguida, selecione **remover perfil**.

   >[!NOTE]
   >A remoção de um perfil de um dispositivo não exclui o perfil da sua lista. Se você quiser excluir um perfil, siga as instruções em [Update ou delete de um perfil do Autopilot](#update-or-delete-an-autopilot-profile).

### <a name="update-or-delete-an-autopilot-profile"></a>Atualizar ou excluir um perfil do Autopilot

Se um cliente deseja alterar a experiência de out-of-box depois que você enviou os dispositivos a eles, você pode alterar o perfil no Partner Center.

Quando o dispositivo do cliente se conecta à internet, ele baixará a última versão de perfil durante o processo OOBE. Além disso, sempre que um cliente restaura um dispositivo para suas configurações padrão de fábrica, o dispositivo novamente baixará a última versão de perfil durante o processo OOBE.

1. Selecione **clientes** no menu do Partner Center e, em seguida, selecione o cliente que deseja alterar um perfil do Autopilot.

2. Na página de detalhes do cliente, selecione **dispositivos**.

3. Sob **perfis do Windows Autopilot** selecione o perfil que você precisa atualizar. Faça as alterações necessárias e, em seguida, selecione **enviar**.

Para excluir este perfil, selecione **excluir perfil** do canto superior direito da página.

### <a name="add-devices-to-a-customers-account"></a>Adicionar dispositivos para uma conta de cliente

>[!NOTE]
>Agentes de vendas e agentes de administrador podem adicionar dispositivos para uma conta de cliente.

Antes de aplicar os perfis personalizados do Autopilot para dispositivos de cliente, você deve ser capaz de acessar a lista de dispositivos do cliente.

Se você planeja usar o nome, número de série e combinação de modelo do OEM, esteja ciente dessas limitações:

- Isso funciona de tupla somente para dispositivos mais recentes (4 hashes de k, por exemplo) e não há suporte para hashes 128b (dispositivos anteriores e RS2).

- O registro de tupla é diferencia maiusculas de minúsculas, portanto, os dados no arquivo devem corresponder aos nomes de modelo e fabricante ***exatamente*** conforme fornecido pelo provedor de OEM (provedor de hardware).

Siga as instruções abaixo para adicionar dispositivos de uma conta de cliente no Partner Center.

1. Selecione **clientes** no menu do Partner Center e, em seguida, selecione o cliente cujos dispositivos você deseja gerenciar.

2. Na página de detalhes do cliente, selecione **dispositivos**.

3. Sob **aplicar perfis de dispositivos** selecionar **adicionar dispositivos**.

4. Insira um nome para a lista de dispositivos e, em seguida, selecione **procurar** para carregar a lista do cliente (no formato de arquivo. csv) no Partner Center.

    >[!NOTE]
    >Você deve ter recebido esse arquivo. csv com a compra de dispositivo. Se você não recebeu um arquivo. csv, você pode criar um por conta própria, seguindo as etapas em [adição de dispositivos Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).  

5. Carregue o arquivo. csv e, em seguida, selecione **salvar**.

Se você receber uma mensagem de erro ao tentar carregar o arquivo. csv, verifique o formato do arquivo. Você pode usar somente, o hash de hardware ou o nome do OEM, número de série e modelo (nessa ordem coluna) ou a ID do produto do Windows. Você também pode usar o arquivo. csv de exemplo fornecido, próximo a partir do link **adicionar dispositivos** para criar uma lista de dispositivos.

## <a name="windows-autopilot-eula-dismissal"></a>Exoneração do EULA do Windows Autopilot

### <a name="important-information"></a>INFORMAÇÕES IMPORTANTES

Windows Autopilot permite que você configure instalações personalizadas do Windows nos dispositivos gerenciados para seus clientes. Se autorizado a fazê-lo pelo cliente, você pode suprimir ou ocultar determinadas telas de configuração que normalmente são apresentadas aos usuários durante a configuração do Windows, incluindo a tela de aceitação do EULA (contrato de licença de usuário final).

Usando essa função, você concorda que, suprimindo ou ocultando as telas que são projetadas para fornecer aos usuários Observe ou a aceitação dos meios de termos que você obteve suficiente consentimento e autorização do cliente para ocultar os termos e que você, em nome de seu cliente (se uma organização ou um usuário individual, como o caso pode estar), concordar com quaisquer avisos e aceitar qualquer termos que são aplicáveis ao seu cliente. Isso inclui o acordo com os termos e condições da licença ou o aviso que seria apresentado ao usuário caso você não o tenha suprimido ou ocultado usando essa ferramenta. Seu cliente não pode usar o software do Windows nesses dispositivos se o cliente não tiver adquirido de forma válida uma licença para o software da Microsoft ou de seus distribuidores licenciados.