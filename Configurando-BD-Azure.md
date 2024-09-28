# Passos para Configurar uma Instância de Banco de Dados no Azure

Configurar uma instância de banco de dados no **Azure** é um processo rápido, realizado através do **Portal do Azure**, **CLI** ou **scripts**. O **Azure SQL Database** é uma solução popular para quem busca escalabilidade e segurança em bancos de dados relacionais.

## 1. Acessando o Ambiente do Azure
- Entre no Portal do Azure utilizando suas credenciais.

## 2. Iniciando a Criação de um Novo Banco de Dados
- No menu lateral, clique em **"Criar um recurso"**.
- Pesquise por **"Azure SQL"** e selecione **"SQL Database"** na lista de opções.

## 3. Configurações Básicas do Banco de Dados
- **Assinatura**: Escolha a assinatura que será usada.
- **Grupo de Recursos**: Selecione um grupo existente ou crie um novo.
- **Nome do Banco de Dados**: Defina o nome desejado.
- **Servidor**: Escolha um servidor existente ou crie um novo. Ao criar um novo servidor, defina:
    - **Nome do Servidor**: Crie um nome exclusivo.
    - **Login de Administrador**: Insira o nome de usuário do administrador.
    - **Senha**: Defina uma senha segura e confirme-a.
    - **Localização**: Escolha a região para hospedar o servidor.

## 4. Configurando Pool de Elasticidade (Se Necessário)
- Caso precise gerenciar múltiplos bancos de dados, configure um **pool elástico**. Caso contrário, escolha **"Não"** para usar um banco de dados único.

## 5. Escolhendo o Desempenho e Capacidade
- **Compute + Storage**: Defina o modelo de desempenho:
    - **DTU (Database Transaction Unit)**: Um modelo simples que combina CPU, memória e I/O.
    - **vCore (Virtual Core)**: Dá mais controle sobre os recursos de CPU, memória e I/O.
- Selecione o tamanho do banco de dados e o tipo de armazenamento (Standard, Premium, Business Critical).

## 6. Definindo o Acesso à Rede
- Configure as opções de rede. O banco de dados é acessível somente dentro do Azure por padrão, mas é possível criar regras de firewall para acesso externo, se necessário.

## 7. Configurações de Segurança e Backup
- Habilite a segurança com **Azure Active Directory (AAD)**, caso necessário.
- Configure as políticas de backup e retenção de dados para proteger suas informações.

## 8. Revisão Final e Criação
- Revise todas as configurações definidas e certifique-se de que estão corretas.
- Clique em **"Criar"** para provisionar o banco de dados.

## Após a Configuração

- Uma vez criada, a instância pode ser gerenciada através do **Portal do Azure**, com opções de ajuste para **dimensionamento**, **segurança** e **acessibilidade**.
- Utilize a **Connection String** fornecida para conectar sua aplicação ao banco de dados.
- Administre o banco de dados usando ferramentas como **Azure Data Studio**, **SQL Server Management Studio (SSMS)** ou outros clientes SQL.
