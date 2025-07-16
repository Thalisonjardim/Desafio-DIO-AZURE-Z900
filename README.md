# Desafio-DIO-AZURE-Z900
Resumos, anotações e dicas sobre o uso da Azure

# Laboratório: Criando uma Instância de Banco de Dados no Azure

Este repositório contém anotações, dicas e um resumo prático sobre como criar e configurar uma **Instância Gerenciada de Banco de Dados SQL no Microsoft Azure**, com base no laboratório proposto no curso.

---

##  Objetivo do Laboratório

Praticar o processo de criação e configuração de uma instância de banco de dados no Azure, documentando os passos realizados para futuras consultas, revisões e uso profissional.

---

## O que você vai aprender neste laboratório

- Como criar um banco de dados SQL gerenciado no Azure
- Como configurar firewall, credenciais e conexões seguras
- Como acessar e testar o banco de dados usando ferramentas como o Azure Data Studio ou SQL Server Management Studio (SSMS)
- Noções básicas de segurança, autenticação e precificação no Azure SQL

---

##  Etapas do Processo

### 1. Acessar o Portal do Azure
- URL: [https://portal.azure.com](https://portal.azure.com)
- Acesse com sua conta Microsoft.

### 2. Criar um recurso de Banco de Dados SQL
- Clique em **"Criar um recurso" > "Banco de Dados SQL"**
- Preencha os campos:
  - **Nome do banco**
  - **Grupo de recursos** (ou crie um novo)
  - **Servidor lógico** (com nome único, login e senha)
  - Escolha o tipo de camada (ex: básica ou DTU padrão)

### 3. Configurar regras de firewall
- Permita acesso ao IP atual para conseguir conectar ao banco
- Registre os IPs necessários para conexão local ou de apps externos

### 4. Acessar o banco de dados
- Use o **Azure Data Studio** ou **SSMS**
- Insira o servidor (ex: `seuservidor.database.windows.net`)
- Faça login com as credenciais criadas
- Teste com um comando SQL simples (`SELECT 1`)

---

##  Dicas Importantes

- **Anote o nome do servidor e as credenciais**, pois são exigidos para conectar depois.
- Utilize **tags** nos recursos para ajudar na organização de projetos reais.
- Prefira regiões próximas à sua localização para melhor desempenho.
- Avalie o **custo estimado** antes de concluir a criação (as camadas impactam o valor).
- Para ambientes de teste, utilize a camada **Básica** para economizar.

---

## 📂 Estrutura de Pastas
📁 azure-sql-lab
├── README.md
└── images/
├── passo1_criar_recurso.png
├── passo2_configurar_servidor.png
└── passo3_conectar_sql.png


---

## ✅ Resultado Esperado

Ao final do processo, você terá uma instância de Banco de Dados SQL funcional e pronta para ser utilizada em aplicações ou consultas, com acesso documentado e seguro.

---

