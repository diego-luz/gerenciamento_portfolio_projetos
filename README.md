
# Documentação do Projeto: Gerenciamento de Portfólio de Projetos

## Introdução
O projeto **Gerenciamento de Portfólio de Projetos** é uma aplicação desenvolvida para facilitar o controle e organização de projetos. Ele oferece funcionalidades para visualização, edição, remoção de projetos e suporte para exportação/importação de dados em formato HTML. É baseado no framework Flask e usa containerização com Docker para facilitar sua implementação.

---

## Funcionalidades
- **Visualização de Projetos**: Listagem de todos os projetos cadastrados.
- **Edição e Exclusão**: Capacidade de editar ou remover projetos.
- **Exportação de Dados**: Exportação de dados do portfólio em formato HTML.
- **Importação de Dados**: Permite importar dados no formato HTML para atualização do portfólio.

---

## Tecnologias Utilizadas
- **Linguagem de Programação**: Python
- **Framework Web**: Flask
- **Frontend**: HTML, CSS, JavaScript
- **Containerização**: Docker

---

## Estrutura do Projeto

### Diretórios e Arquivos Principais

- **`app.py`**: Arquivo principal da aplicação Flask.
- **`database.py`**: Gerenciamento do banco de dados local.
- **`templates/`**: Contém os templates HTML.
- **`static/`**: Arquivos estáticos como CSS e JavaScript.
- **`Dockerfile`**: Configuração para criar a imagem Docker.
- **`.dockerignore`**: Arquivos/diretórios ignorados pelo Docker.
- **`.gitignore`**: Arquivos/diretórios ignorados pelo Git.
- **`requirements.txt`**: Lista de dependências Python.
- **`README.md`**: Documentação inicial do projeto.

---

## Configuração do Ambiente

### Requisitos
- Python 3.8 ou superior
- Docker (opcional para containerização)
- Git

### Passos para Configurar o Ambiente Localmente

1. **Clonar o Repositório**
   ```bash
   git clone https://github.com/diego-luz/gerenciamento_portfolio_projetos.git
   cd gerenciamento_portfolio_projetos
   ```

2. **Criar e Ativar um Ambiente Virtual**
   ```bash
   python -m venv venv
   source venv/bin/activate   # Para Linux/Mac
   venv\Scripts\activate     # Para Windows
   ```

3. **Instalar Dependências**
   ```bash
   pip install -r requirements.txt
   ```

4. **Executar a Aplicação**
   ```bash
   python app.py
   ```
   A aplicação estará acessível em `http://localhost:5000`.

---

## Configuração com Docker

1. **Construir a Imagem Docker**
   ```bash
   docker build -t gerenciamento_portfolio_projetos .
   ```

2. **Executar o Contêiner**
   ```bash
   docker run -p 5000:5000 gerenciamento_portfolio_projetos
   ```
   A aplicação estará acessível em `http://localhost:5000`.

---

## Testes da Aplicação

1. **Verificar a Interface Web**
   - Acesse `http://localhost:5000` no navegador.
   - Verifique se os projetos estão sendo listados corretamente.

2. **Testar Funcionalidades**
   - Adicione novos projetos pela interface.
   - Edite e exclua projetos existentes.
   - Exporte os dados em formato HTML e verifique o arquivo gerado.
   - Importe dados de um arquivo HTML e valide sua inclusão na aplicação.

