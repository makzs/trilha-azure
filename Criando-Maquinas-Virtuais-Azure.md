# Como Criar Máquinas Virtuais no Azure

O **Microsoft Azure** oferece uma infraestrutura robusta e flexível para criar e gerenciar **Máquinas Virtuais (VMs)**. 
A plataforma garante alta disponibilidade com um **SLA (Acordo de Nível de Serviço)** que pode alcançar até **99,99%**, 
dependendo das opções de redundância e alta disponibilidade selecionadas, como zonas de disponibilidade. Isso significa 
que o tempo de inatividade é minimizado, oferecendo uma confiabilidade essencial para aplicações críticas.

Os **custos** variam de acordo com a **região**, o **tamanho da VM**, o tipo de **armazenamento** utilizado (SSD, HDD) e 
o **uso de recursos de rede**. É importante planejar a capacidade necessária, monitorar o uso dos recursos e otimizar as 
VMs para evitar gastos desnecessários. O Azure oferece ferramentas de estimativa de custos que podem ajudar a calcular o 
valor mensal de operação de uma VM, levando em consideração esses fatores.

## Etapas para Criar uma Máquina Virtual

### 1. Acessando o Portal do Azure
- Vá para o Portal do Azure e faça login com suas credenciais.

### 2. Iniciando a Criação do Recurso
- No menu lateral, clique em **"Criar um recurso"**.
- Busque por **"Máquina Virtual"** na barra de pesquisa ou selecione-a diretamente.

### 3. Configurações Básicas da VM
- **Assinatura**: Escolha a assinatura a ser usada.
- **Grupo de Recursos**: Selecione um existente ou crie um novo.
- **Nome da VM**: Defina o nome da máquina virtual.
- **Região**: Selecione a localização geográfica.
- **Opções de Disponibilidade**: Escolha opções de alta disponibilidade, como zonas ou conjuntos de disponibilidade.
- **Imagem**: Selecione o sistema operacional da VM (Windows, Linux, etc.).
- **Tamanho**: Defina os recursos de CPU e RAM necessários.

### 4. Definindo a Autenticação da VM
- **Tipo de Autenticação**: Escolha entre **Senha** ou **Chave SSH**.
- **Nome de Usuário**: Defina o nome do administrador.
- **Senha/Chave Pública SSH**: Informe a senha ou a chave pública SSH, de acordo com o método escolhido.

### 5. Configurando o Armazenamento da VM
- **Tipo de Disco**: Selecione entre **SSD Padrão**, **SSD Premium** ou **HDD**.
- Caso necessário, adicione discos adicionais para a VM.

### 6. Configurações de Rede
- **Rede Virtual**: Selecione uma rede virtual existente ou crie uma nova.
- **Sub-rede**: Defina uma sub-rede onde a VM estará conectada.
- **IP Público**: Configure um IP público para acessar a VM externamente.
- **Grupo de Segurança de Rede**: Estabeleça regras de firewall para controlar o tráfego de entrada e saída.

### 7. Definindo Regras de Acesso e Monitoramento
- Habilite o acesso por **SSH (22)** para Linux ou **RDP (3389)** para Windows, conforme necessário.
- Ative o **Monitoramento** através do Azure Monitor para acompanhar o desempenho da VM.

### 8. Finalizando a Criação
- Revise todas as configurações para garantir que estejam corretas.
- Clique em **"Criar"** para iniciar o processo de criação da máquina virtual.

## Acessando e Gerenciando a VM
- Após a criação, acesse a VM utilizando o método configurado (SSH ou RDP).
- Gerencie a VM via portal, linha de comando (CLI), ou APIs, fazendo ajustes nos recursos, monitoramento e configurações de segurança conforme necessário.
