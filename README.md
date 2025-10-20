# 🗂️ Sistema de Cadastro em Java com PostgreSQL

Este projeto foi desenvolvido com o objetivo de praticar a integração entre Java e PostgreSQL utilizando JDBC (Java Database Connectivity).

## 🚀 Funcionalidades

O sistema realiza operações básicas de CRUD em uma tabela tab_cadastro:

**Incluir**: adiciona um novo registro no banco de dados

**Alterar**: atualiza os dados de um cadastro existente

**Excluir**: remove um registro pelo ID

**Listar**: exibe todos os cadastros

**Buscar**: encontra um cadastro específico pelo ID

## 🧩 Estrutura do Projeto

Cadastro.java → Classe modelo representando a entidade com atributos id, nome e idade.

FabricaConexao.java → Classe responsável por criar e gerenciar a conexão com o banco de dados PostgreSQL.

CadastroRepository.java → Classe que implementa os métodos de persistência (CRUD) utilizando JDBC.

SistemaCadastro.java → Classe principal que executa o sistema e demonstra o uso das operações.

### ⚙️ Tecnologias Utilizadas

- Java 17

- PostgreSQL

- JDBC

- IDE: DBeaver / IntelliJ

### 📦 Como Executar

Crie o banco de dados rocket_db no PostgreSQL

Execute o script SQL:

<pre>CREATE TABLE public.tab_cadastro (
    id SERIAL PRIMARY KEY,
    nome VARCHAR(50) NOT NULL,
    idade INT NOT NULL
);</pre>


Configure as credenciais no arquivo FabricaConexao.java

Compile e execute SistemaCadastro.java

