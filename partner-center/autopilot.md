---
title: Personalizar a experiência de out-of-box do dispositivo com perfis do Windows Autopilot | Partner Center
description: Pré-configure experiência de out-of-box do dispositivo com perfis Autopilot.
author: maggiepuccievans
keywords: piloto automático, o windows autopilot, piloto automático da microsoft, implantação zero touch, oobe, telas de logon, out-of-box
ms.localizationpriority: medium
ms.openlocfilehash: 7df979042799954c5b43a2adef1915941db02e57
ms.sourcegitcommit: 90d656ed3a4d056a0506f7b5e2b1b8c728f58c46
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/19/2018
ms.locfileid: "8976803"
---
# <a name="customize-a-devices-out-of-box-experience-with-windows-autopilot-profiles"></a>Personalizar a experiência de out-of-box do dispositivo com perfis do Windows Autopilot

**Aplica-se ao**

- Parceiros de cobrança direta CSP, provedores indiretos e revendedores indiretos

Se você gerencia dispositivos cliente, talvez seja necessário personalizar a experiência de out-of-box (OOBE) para usuários do cliente. Você pode pré-configurar novos dispositivos com perfis do Windows Autopilot antes de entregar os dispositivos para os clientes e aplicar perfis de novos dispositivos clientes já tem comprado. Este artigo explica como criar e aplicar perfis Autopilot para dispositivos no Partner Center.

Se você já não estiver familiarizado com o Autopilot, examine as informações neste artigo:

- [Visão geral do Windows Autopilot.](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [Guia de referência de implantação do AutoPilot](http://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>Visão geral

Com o recurso Windows Autopilot no Partner Center, você pode criar perfis personalizados para aplicar aos dispositivos de cliente. As seguintes configurações de perfil estavam disponíveis no momento em que este artigo foi publicado:

- Ignorar configurações de privacidade. Essa configuração de perfil do Autopilot opcional permite que as organizações não pergunte sobre configurações de privacidade durante o processo de configuração inicial pelo usuário.

- Desabilite a criação de conta de administrador local no dispositivo. As organizações podem decidir se o usuário de configuração do dispositivo deve ter acesso de administrador quando o processo for concluído.

- Configure automaticamente o dispositivo para trabalho ou escola. Todos os dispositivos registrados com o Autopilot automaticamente serão considerados trabalho ou escola dispositivos, portanto, essa pergunta não será solicitada durante o processo de configuração inicial pelo usuário.

- Ignorar a Cortana, OneDrive e OEM páginas de configuração do registro. Todos os dispositivos registrados com o Autopilot ignorará automaticamente essas páginas durante o processo de experiência de out-of-box (OOBE).

- Ignorar o contrato de licença de usuário final (EULA). A partir do Windows 10 versão 1709, as organizações podem optar por ignorar a página de EULA apresentada durante o processo de configuração inicial pelo usuário. Consulte o [descarte de EULA do Windows Autopilot](#windows-autopilot-eula-dismissal) abaixo para obter informações importantes a serem consideradas sobre ignorar a página do EULA durante a instalação do Windows.

Os seguintes permissões de gerenciamento de dispositivo e de perfil e limitações se aplicam:

- Os parceiros CSP podem continuar a gerenciar perfis Autopilot para clientes existentes com quem eles têm relações de revendedor, mesmo que os clientes tenham removido privilégios de administração delegada do parceiro.

- Você pode gerenciar dispositivos existentes para seus clientes que foram adicionados por você ou por outro parceiro CSP.

- Você não pode gerenciar dispositivos que seu cliente carregou a Microsoft Store para empresas ou Portal do Microsoft Intune.

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>Criar e gerenciar perfis Autopilot no Partner Center

No Partner Center, você pode criar perfis de implantação do Windows Autopilot e aplicá-los aos dispositivos.

>[!NOTE]
>Somente agentes de administrador podem criar e aplicar perfis.

### <a name="create-a-new-autopilot-profile"></a>Criar um novo perfil do Autopilot

1. Selecione **os clientes** no menu Partner Center e, em seguida, selecione o cliente que você estiver criando o perfil Autopilot.

2. Na página de detalhes do cliente, selecione **dispositivos**.

3. Em **perfis do Windows Autopilot** selecione **Adicionar novo perfil**.

4. Insira o nome e a descrição do perfil e, em seguida, defina as configurações de OOBE. Escolha:  

   - Ignorar configurações de privacidade na instalação
   
   - Desabilitar a conta de administrador local na instalação
   
   - Ignorar automaticamente as páginas na instalação<br>
        (Inclui *Selecionar automaticamente a configuração para trabalho ou escola* e *Ignorar Cortana, OneDrive e OEM páginas de configuração de registro*)
   
   - Ignorar contrato de licença de usuário final (EULA)<br> 
       >[!IMPORTANT] Consulte o [descarte de EULA do Windows Autopilot](#windows-autopilot-eula-dismissal) abaixo para obter informações importantes a serem consideradas sobre ignorar a página do EULA durante a instalação do Windows.

5. Selecione **Enviar** quando terminado.

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>Aplicar um perfil Autopilot para dispositivos cliente

>[!NOTE]
>As instruções a seguir pressupõem que você já tiver adicionado os dispositivos do cliente para o Partner Center e que você possa acessar sua lista de dispositivos. Se você ainda não tiver adicionado dispositivos do cliente, siga as instruções em [Adicionar dispositivos para uma conta do cliente](#add-devices-to-a-customers-account) e, em seguida, siga as etapas abaixo.

Depois de criar um perfil Autopilot para um cliente, você pode aplicá-lo a dispositivos do cliente.

1. Selecione **os clientes** no menu Partner Center e, em seguida, selecione o cliente que você criou o perfil Autopilot para.

2. Na página de detalhes do cliente, selecione **dispositivos**.

3. Em **aplicar perfis aos dispositivos** , selecione os dispositivos ou grupos de dispositivos que você deseja adicionar perfis a e, em seguida, selecione o **perfil de aplicar**. O perfil que você acabou de aplicar aparece na coluna **perfil** .

4. Siga as etapas abaixo para verificar que o perfil será aplicado com êxito no dispositivo.

    a.  Conecte um dispositivo à rede e ativá-lo.

    b.  Verifique se aparecem as telas OOBE apropriadas (se existirem).

    c.  Quando o processo de OOBE parar, redefina o dispositivo para as configurações padrão de fábrica para prepará-lo para um novo usuário.

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>Remover um perfil Autopilot do dispositivo do cliente

1. Selecione **os clientes** no menu Partner Center e, em seguida, selecione o cliente que você criou o perfil Autopilot para.

2. Na página de detalhes do cliente, selecione **dispositivos**.

3. Em **aplicar perfis aos dispositivos** selecione os dispositivos que você deseja remover o perfil e, em seguida, selecione **Remover perfil**.

  >[!NOTE]
  >Remover um perfil de um dispositivo não exclui o perfil de sua lista. Se você deseja excluir um perfil, siga as instruções na [atualização ou excluir um perfil Autopilot](#update-or-delete-an-autopilot-profile).

### <a name="update-or-delete-an-autopilot-profile"></a>Atualizar ou excluir um perfil Autopilot

Se um cliente quiser alterar a experiência de out-of-box depois que você tiver recebido os dispositivos para eles, você pode alterar o perfil no Partner Center.

Quando o dispositivo do cliente se conecta à internet, ele vai baixar a versão mais recente do perfil durante o processo de configuração inicial pelo usuário. Além disso, sempre que um cliente restaura um dispositivo para as configurações padrão de fábrica, o dispositivo baixará novamente a versão mais recente do perfil durante o processo de configuração inicial pelo usuário.

1. Selecione **os clientes** no menu Partner Center e, em seguida, selecione o cliente que deseja alterar um perfil Autopilot.

2. Na página de detalhes do cliente, selecione **dispositivos**.

3. Em **perfis do Windows Autopilot** , selecione o perfil que você precisa atualizar. Faça as alterações necessárias e, em seguida, selecione **Enviar**.

Para excluir esse perfil, selecione **Excluir perfil** no canto superior direito da página.

### <a name="add-devices-to-a-customers-account"></a>Adicionar dispositivos a uma conta do cliente

>[!NOTE]
>Agentes de vendas e agentes de administrador podem adicionar dispositivos para uma conta do cliente.

Antes de aplicar perfis Autopilot personalizados em dispositivos cliente, você deve ser capaz de acessar a lista de dispositivos do cliente.

Se você pretende usar o nome do OEM, o número de série e combinação de modelo, lembre-se dessas limitações:

- Isso funciona tupla apenas para dispositivos mais recentes (4 hashes de k, por exemplo) e não há suporte para 128b hashes (RS2 e dispositivos anteriores).

- O registro de tupla diferencia maiusculas de minúsculas, portanto, os dados no arquivo devem coincidir com o modelo e fabricante nomes ***exatamente*** conforme fornecido pelo provedor de OEM (fornecedor de hardware).

Siga as instruções para adicionar dispositivos a uma conta do cliente no Partner Center.

1. Selecione **os clientes** no menu Partner Center e, em seguida, selecione o cliente cujos dispositivos que você deseja gerenciar.

2. Na página de detalhes do cliente, selecione **dispositivos**.

3. Em **aplicar perfis aos dispositivos** selecione **Adicionar dispositivos**.

4. Insira um nome para a lista de dispositivos e, em seguida, selecione **Procurar** para carregar a lista do cliente (no formato de arquivo. csv) para o Partner Center.

    >[!NOTE]
    >Você deve ter recebido esse arquivo. csv com sua compra de dispositivo. Se você não receber um arquivo. csv, você pode criar uma por conta própria, seguindo as etapas em [adicionando dispositivos Windows Autopilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).  

5. Carregue o arquivo. csv e, em seguida, selecione **Salvar**.

Se você receber uma mensagem de erro ao tentar carregar o arquivo. csv, verifique o formato do arquivo. Você pode usar somente o hash de hardware ou o nome do OEM, o número de série e modelo (nessa ordem coluna) ou a ID do produto do Windows. Você também pode usar o arquivo. csv de exemplo fornecido no link ao lado de **Adicionar dispositivos** para criar uma lista de dispositivos.

## <a name="windows-autopilot-eula-dismissal"></a>Descarte de EULA do Windows Autopilot

### <a name="important-information"></a>INFORMAÇÕES IMPORTANTES

O Windows Autopilot permite que você configure instalações personalizadas do Windows em dispositivos que você gerencia para seus clientes. Se tiver autorização para fazê-lo pelo cliente, você pode suprimir ou ocultar determinadas telas de instalação que normalmente são apresentadas aos usuários ao configurar o Windows, incluindo a tela de aceitação do EULA (contrato de licença de usuário final).

Ao usar essa função, você concorda que suprimir ou ocultar quaisquer telas projetadas para fornecer aos usuários aviso ou aceitação dos termos significa que você obteve o consentimento suficiente e autorização de seu cliente para ocultar termos e que você, em nome de seu cliente (se uma organização ou um usuário individual como o caso pode ser), concorda com quaisquer avisos e aceitar qualquer termos que são aplicáveis ao cliente. Isso inclui o acordo com os termos e condições da licença ou o aviso que seria apresentado ao usuário caso você não o tenha suprimido ou ocultado usando essa ferramenta. Seu cliente não pode usar o software do Windows nesses dispositivos se o cliente não tiver adquirido de forma válida uma licença para o software da Microsoft ou de seus distribuidores licenciados.