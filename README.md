# Como Criar uma Máquina Virtual no Azure: Passo a Passo

Criar uma máquina virtual (VM) no Azure é um processo simples que permite implementar servidores de forma rápida e escalável. Neste guia, abordaremos todos os detalhes e recursos do Azure envolvidos na criação de uma VM. Vamos ao passo a passo!

## Passo 1: Acessar o Portal do Azure

1. **Entre no Portal do Azure**:
   - Acesse [portal.azure.com](https://portal.azure.com) e faça login na sua conta do Azure.

## Passo 2: Iniciar a Criação da Máquina Virtual

1. **Clique em "Criar um recurso"**:
   - No menu à esquerda, clique em "Criar um recurso".

2. **Escolha "Máquina Virtual"**:
   - Na barra de pesquisa, digite "Máquina Virtual" e selecione a opção correspondente.

## Passo 3: Configurar a Máquina Virtual

### 3.1: Detalhes da Máquina Virtual

- **Assinatura**: 
  - Selecione a assinatura do Azure que deseja usar.
  
- **Grupo de Recursos**: 
  - Escolha um grupo de recursos existente ou crie um novo. Um grupo de recursos, também conhecido como **Resource Group**, é um contêiner que armazena recursos relacionados à sua VM.
  
- **Nome da Máquina Virtual**: 
  - Insira um nome exclusivo para sua VM.
  
- **Região**: 
  - Escolha a região onde a VM será implantada (ex: Leste dos EUA, Oeste da Europa).
  
- **Disponibilidade**: 
  - Se desejar, escolha uma zona de disponibilidade (Availability Zone) para aumentar a resiliência.

### 3.2: Imagem do Sistema Operacional

- **Escolha uma Imagem**: 
  - Selecione uma imagem de sistema operacional disponível, como **Windows Server**, **Ubuntu**, **CentOS**, ou outras distribuições Linux.

### 3.3: Tamanho da Máquina Virtual

- **Selecionar Tamanho**: 
  - Escolha um tamanho para a VM, que determina a quantidade de CPU e memória. O Azure oferece várias opções de tamanhos, como **Dv3 Series** ou **Fsv2 Series**, com diferentes preços e capacidades.

### 3.4: Configurações de Administração

- **Nome de Usuário**: 
  - Insira um nome de usuário que você usará para acessar a VM.
  
- **Senha**: 
  - Crie uma senha segura para a conta de administrador.
  
- **Autenticação SSH** (para Linux): 
  - Você pode optar por usar uma chave SSH em vez de uma senha, o que é recomendado para maior segurança.

## Passo 4: Configurações de Rede

### 4.1: Configurar Rede Virtual

- **Rede Virtual**: 
  - Selecione uma **Virtual Network (VNet)** existente ou crie uma nova. As redes virtuais permitem que suas VMs se comuniquem entre si e com outros recursos.

### 4.2: Configurações de Sub-rede

- **Sub-rede**: 
  - Escolha uma **subnet** dentro da rede virtual selecionada. Isso ajudará a organizar suas VMs e recursos de rede.

### 4.3: Configurações de IP

- **Endereço IP Público**: 
  - Marque a opção para criar um **Endereço IP Público** se você deseja acessar sua VM pela Internet.

### 4.4: Configurações de Firewall

- **Grupo de Segurança da Rede (NSG)**: 
  - Crie ou selecione um **Network Security Group (NSG)** para controlar o tráfego de entrada e saída da sua VM. Você pode definir regras para permitir ou bloquear portas específicas, como SSH (22) ou RDP (3389).

## Passo 5: Revisar e Criar

1. **Revisar as Configurações**: 
   - Confira todas as configurações que você selecionou. Você pode voltar e editar qualquer uma delas, se necessário.

2. **Criar a Máquina Virtual**: 
   - Clique em "Criar" para iniciar a implantação da sua VM. O Azure levará alguns minutos para criar e configurar a máquina virtual.

## Passo 6: Conectar-se à Máquina Virtual

1. **Acessar a VM**: 
   - Após a implantação, vá até o painel da VM e clique em "Conectar".
   - Se for uma VM do Windows, você pode usar o **Remote Desktop Protocol (RDP)**. Para VMs Linux, use **SSH**.

2. **Inserir Credenciais**: 
   - Utilize o nome de usuário e a senha que você criou para acessar a máquina virtual.

## Conclusão

Parabéns! Você criou sua primeira máquina virtual no Azure. Com essa VM, você pode começar a implementar suas aplicações, realizar testes ou executar cargas de trabalho específicas.

Para gerenciar sua VM, você pode usar o portal do Azure, **Azure CLI** ou **Azure PowerShell**. Explore as funcionalidades e comece a aproveitar a flexibilidade e escalabilidade que a nuvem oferece!

---

Para mais informações e recursos, acesse a [Documentação do Azure sobre Máquinas Virtuais](https://docs.microsoft.com/pt-br/azure/virtual-machines/).
