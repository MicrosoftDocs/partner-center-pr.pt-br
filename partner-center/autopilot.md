---
title: Personalizar a experiência de uso inicial do dispositivo
ms.topic: how-to
ms.date: 04/28/2020
ms.service: partner-dashboard
ms.subservice: partnercenter-csp
description: Antes de entregar um novo dispositivo do cliente, você pode usar os perfis do Windows AutoPilot para personalizar ou pré-configurar a OOBE (configuração inicial do usuário) do dispositivo.
author: BillLinzbach
ms.author: BillLi
ms.localizationpriority: medium
ms.custom: SEOAPR.20
ms.openlocfilehash: a59b0c25b8f5203942e73b549d5ffb9d65d90c36
ms.sourcegitcommit: 7e19c211b1d5f2db2a4c56a743b14c8485decd99
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/03/2020
ms.locfileid: "87527652"
---
# <a name="use-windows-autopilot-profiles-on-new-devices-to-customize-a-customers-out-of-box-experience"></a>Usar perfis do Windows AutoPilot em novos dispositivos para personalizar a experiência de uso inicial do cliente

**Aplica-se a**

- CSP direto-parceiros de cobrança, provedores indiretos e revendedores indiretos

**Funções apropriadas**

- Agente administrativo
- Administrador global
- Agente de vendas
- Administrador de gerenciamento de usuário

Se você gerenciar dispositivos de clientes, talvez seja necessário personalizar a OOBE (experiência inicial do usuário) para os usuários do cliente. Você pode pré-configurar novos dispositivos com os perfis do Windows AutoPilot antes de entregar os dispositivos aos clientes e aplicar novos perfis a dispositivos que os clientes já adquiriram. 

Observe que os OEMs começaram a incluir um rótulo de remessa no fora da caixa de dispositivo do piloto automático que mostra a **ID de chave do produto (PKID)** do dispositivo.  Este código de barras legível e unidimensional fornece aos parceiros downstream uma maneira de registrar dispositivos para o AutoPilot sem precisar unboxr os dispositivos e coletar a ID do dispositivo por meios alternativos.

Este artigo explica como criar e aplicar perfis do AutoPilot a dispositivos no Partner Center.

Se você ainda não estiver familiarizado com o piloto automático, revise as informações nestes artigos:

- [Visão geral do Windows AutoPilot](https://docs.microsoft.com/windows/deployment/windows-10-auto-pilot)
- [Guia de referência de implantação do AutoPilot](https://assetsprod.microsoft.com/autopilot-deployment-program-reference-guide-csp.docx)  

## <a name="overview"></a>Visão geral

Com o recurso de piloto automático do Windows no Partner Center, você pode criar perfis personalizados para aplicar aos dispositivos do cliente. As seguintes configurações de perfil estavam disponíveis no momento em que este artigo foi publicado:

- Ignore as configurações de privacidade. Essa configuração opcional do perfil de piloto automático permite que as organizações não perguntem sobre as configurações de privacidade durante o processo OOBE.

- Desabilite a criação da conta de administrador local no dispositivo. As organizações podem decidir se o usuário que está configurando o dispositivo deve ter acesso de administrador quando o processo for concluído.

- Configurar automaticamente o dispositivo para trabalho ou escola. Todos os dispositivos registrados com o piloto automático serão considerados dispositivos corporativos ou de estudante automaticamente, portanto, essa pergunta não será feita durante o processo OOBE.

- Ignore as páginas de configuração de registro do Cortana, do OneDrive e do OEM. Todos os dispositivos registrados com o AutoPilot irão ignorar automaticamente essas páginas durante o processo de OOBE (experiência inicial do uso).

- Ignorar contrato de licença de usuário final (EULA). A partir do Windows 10 versão 1709, as organizações podem decidir ignorar a página de EULA apresentada durante o processo OOBE. Consulte o [contrato de EULA do Windows AutoPilot](#windows-autopilot-eula-dismissal) abaixo para obter informações importantes a serem consideradas para ignorar a página de EULA durante a instalação do Windows.

As seguintes permissões e limitações de gerenciamento de perfil e dispositivo se aplicam:

- Os parceiros CSP podem continuar a gerenciar perfis de AutoPilot para clientes existentes com os quais têm relações de revendedores, mesmo que os clientes tenham removido os privilégios de administração delegada do parceiro.

- Você pode gerenciar dispositivos existentes para seus clientes que você adicionou.

- Você não pode gerenciar dispositivos que seu cliente carregou para Microsoft Store para empresas ou para o portal de Microsoft Intune.

## <a name="create-and-manage-autopilot-profiles-in-partner-center"></a>Criar e gerenciar perfis do AutoPilot no Partner Center

No Partner Center, você pode criar perfis de implantação do Windows AutoPilot e aplicá-los a dispositivos.

>[!NOTE]
>Somente agentes admin podem criar e aplicar perfis.

### <a name="create-a-new-autopilot-profile"></a>Criar um novo perfil do AutoPilot

1. Selecione **clientes** no menu do centro de parceiros e, em seguida, selecione o cliente para o qual você está criando o perfil do AutoPilot.

2. Na página de detalhes do cliente, selecione **dispositivos**.

3. Em **perfis do Windows AutoPilot** , selecione **Adicionar novo perfil**.

4. Insira o nome e a descrição do perfil e defina as configurações do OOBE. Escolha:  

   - Ignorar as configurações de privacidade na instalação

   - Desabilitar a conta de administrador local na instalação
  
   - Ignorar automaticamente as páginas na instalação<br>
        (Inclui *selecionar automaticamente a instalação para trabalho ou escola* e *ignorar as páginas de configuração de registro do Cortana, onedrive e OEM*)
  
   - Ignorar contrato de licença de usuário final (EULA)<br> 
       >[!IMPORTANT] 
       >Consulte o [contrato de EULA do Windows AutoPilot](#windows-autopilot-eula-dismissal) abaixo para obter informações importantes a serem consideradas para ignorar a página de EULA durante a instalação do Windows.

5. Selecione **Enviar** quando terminado.

### <a name="apply-an-autopilot-profile-to-customer-devices"></a>Aplicar um perfil do AutoPilot aos dispositivos do cliente

>[!NOTE]
>As instruções a seguir pressupõem que você já adicionou os dispositivos do cliente ao Partner Center e que pode acessar sua lista de dispositivos. Se você ainda não tiver adicionado os dispositivos do cliente, siga as instruções em [Adicionar dispositivos à conta de um cliente](#add-devices-to-a-customers-account) e siga as etapas abaixo.

Depois de criar um perfil de AutoPilot para um cliente, você pode aplicá-lo aos dispositivos do cliente.

1. Selecione **clientes** no menu do centro de parceiros e, em seguida, selecione o cliente para o qual você criou o perfil do AutoPilot.

2. Na página de detalhes do cliente, selecione **dispositivos**.

3. Em **aplicar perfis a dispositivos** , selecione os dispositivos ou grupos de dispositivos aos quais você deseja adicionar perfis e, em seguida, selecione **aplicar perfil**. O perfil que você acabou de aplicar aparece na coluna **perfil** .

4. Siga as etapas abaixo para verificar se o perfil será aplicado com êxito ao dispositivo.

    a.  Conecte um dispositivo à rede e ligue-o.

    b.  Verifique se aparecem as telas OOBE apropriadas (se existirem).

    c.  Quando o processo OOBE for interrompido, redefina o dispositivo para as configurações padrão de fábrica para prepará-lo para um novo usuário.

### <a name="remove-an-autopilot-profile-from-a-customers-device"></a>Remover um perfil do AutoPilot do dispositivo de um cliente

1. Selecione **clientes** no menu do centro de parceiros e, em seguida, selecione o cliente para o qual você criou o perfil do AutoPilot.

2. Na página de detalhes do cliente, selecione **dispositivos**.

3. Em **aplicar perfis a dispositivos** , selecione os dispositivos dos quais você deseja remover o perfil e, em seguida, selecione **remover Perfil**.

   >[!NOTE]
   >A remoção de um perfil de um dispositivo não exclui o perfil da sua lista. Se você quiser excluir um perfil, siga as instruções em [atualizar ou excluir um perfil do AutoPilot](#update-or-delete-an-autopilot-profile).

### <a name="update-or-delete-an-autopilot-profile"></a>Atualizar ou excluir um perfil do AutoPilot

Se um cliente quiser alterar a experiência inicial do usuário depois que você enviou os dispositivos para eles, você poderá alterar o perfil no Partner Center.

Quando o dispositivo do cliente se conecta à Internet, ele baixa a versão mais recente do perfil durante o processo OOBE. Além disso, sempre que um cliente restaurar um dispositivo para suas configurações padrão de fábrica, o dispositivo baixará novamente a versão mais recente do perfil durante o processo OOBE.

1. Selecione **clientes** no menu do Partner Center e, em seguida, selecione o cliente que deseja alterar um perfil do AutoPilot.

2. Na página de detalhes do cliente, selecione **dispositivos**.

3. Em **perfis do Windows AutoPilot** , selecione o perfil que você precisa atualizar. Faça as alterações necessárias e, em seguida, selecione **Enviar**.

Para excluir esse perfil, selecione **excluir perfil** no canto superior direito da página.

### <a name="add-devices-to-a-customers-account"></a>Adicionar dispositivos à conta de um cliente

>[!NOTE]
>Agentes de vendas e agentes de Administração podem adicionar dispositivos à conta de um cliente.

Antes de aplicar perfis de AutoPilot personalizados a dispositivos de cliente, você deve ser capaz de acessar a lista de dispositivos do cliente.

Se você planeja usar o nome do OEM, o número de série e a combinação de modelos, esteja atento a essas limitações:

- Essa tupla funciona apenas para dispositivos mais recentes (hashes de 4K, por exemplo) e não tem suporte para hashes 128B (RS2 e dispositivos anteriores).

- O registro de tupla diferencia maiúsculas de minúsculas e, portanto, os dados no arquivo devem corresponder ao modelo e aos nomes dos fabricantes ***exatamente*** como fornecidos pelo provedor OEM (provedor de hardware).

Siga as instruções abaixo para adicionar dispositivos à conta de um cliente no Partner Center.

1. Selecione **clientes** no menu do centro de parceiros e, em seguida, selecione o cliente cujos dispositivos você deseja gerenciar.

2. Na página de detalhes do cliente, selecione **dispositivos**.

3. Em **aplicar perfis a dispositivos** , selecione **Adicionar dispositivos**.

4. Insira um nome para a lista de dispositivos e, em seguida, selecione **procurar** para carregar a lista do cliente (no formato de arquivo. csv) para o centro de parceiros.

    >[!NOTE]
    >Você deve ter recebido esse arquivo. csv com a compra do dispositivo. Se você não recebeu um arquivo. csv, você pode criar um por conta própria seguindo as etapas em [adicionando dispositivos ao Windows AutoPilot](https://docs.microsoft.com/windows/deployment/windows-autopilot/add-devices#collecting-the-hardware-id-from-existing-devices-using-powershell).  

5. Carregue o arquivo. csv e, em seguida, selecione **salvar**.

Se você receber uma mensagem de erro ao tentar carregar o arquivo. csv, verifique o formato do arquivo. Você pode usar somente o hash de hardware ou o nome do OEM, o número de série e o modelo (na ordem da coluna) ou a ID do produto do Windows. Você também pode usar o arquivo. csv de exemplo fornecido no link ao lado de **Adicionar dispositivos** para criar uma lista de dispositivos.

Seu arquivo. csv deve ser semelhante a este:

> **Número de série do dispositivo, ID do produto do Windows, hash de hardware, nome do fabricante, modelo do dispositivo**

> **{serialNumber},,, Microsoft Corporation, laptop Surface**

>[!NOTE]
> "Nome do fabricante" e "modelo do dispositivo" diferenciam maiúsculas de minúsculas.

Se você não souber qual valor deve ser colocado para o nome do fabricante e o modelo do dispositivo, poderá executá-lo no dispositivo para reunir os valores corretos:

<pre><code>md c:\\HWID

Set-Location c:\\HWID

Set-ExecutionPolicy -Scope Process -ExecutionPolicy Unrestricted

Install-Script -Name Get-WindowsAutoPilotInfo

Get-WindowsAutoPilotInfo.ps1 -OutputFile AutoPilotHWID.csv -Partner -Force
</code></pre>

## <a name="windows-autopilot-eula-dismissal"></a>Descartar EULA do Windows AutoPilot

### <a name="important-information"></a>INFORMAÇÕES IMPORTANTES

O Windows Autopilot permite configurar instalações personalizadas do Windows em dispositivos que você gerencia para seus clientes. Se autorizado a fazer isso pelo cliente, você poderá suprimir ou ocultar determinadas telas de configuração que normalmente são apresentadas aos usuários durante a configuração do Windows, incluindo a tela de aceitação do EULA (contrato de licença de usuário final).

Usando essa função, você concorda que suprimir ou ocultar as telas que foram projetadas para fornecer aos usuários aviso ou aceitação de termos significa que você obteve consentimento e autorização suficientes de seu cliente para ocultar os termos e que, em nome de seu cliente (seja uma organização ou um usuário individual como o caso), tenha consentimento para quaisquer avisos e aceite quaisquer termos que sejam aplicáveis ao cliente. Isso inclui o acordo com os termos e condições da licença ou o aviso que seria apresentado ao usuário caso você não o tenha suprimido ou ocultado usando essa ferramenta. Seu cliente não pode usar o software do Windows nesses dispositivos se o cliente não tiver adquirido de forma válida uma licença para o software da Microsoft ou de seus distribuidores licenciados.
