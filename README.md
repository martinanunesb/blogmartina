# Blog da Martina

Aplicação web estilo blog desenvolvida com **Django** como **Projeto Final do Curso de Python da Coderhouse**.  
O foco é praticar autenticação, perfis de usuário, CRUD de páginas e troca de mensagens entre usuários.

## Funcionalidades principais

- **Home** com visão geral do site.
- Página **“Sobre mim”** com informações da autora.
- Seção de **páginas/posts**:
  - listagem de páginas com botão **“Leia mais”**;
  - detalhe de cada página;
  - mensagem de aviso quando não há páginas ou resultados de busca.
- **CRUD de páginas** (criar, editar e excluir) disponível apenas para usuários logados.
- **Autenticação de usuários**:
  - registro, login e logout;
  - app dedicado para contas/usuários.
- **Perfil de usuário**:
  - nome, sobrenome, e-mail, avatar, biografia e outros dados editáveis;
  - opção de alterar senha.
- **Sistema de mensagens privadas**:
  - envio de mensagens entre usuários;
  - caixa de entrada e de saída.

## Navegação

Principais seções disponíveis pelo menu:

- **Home**
- **Sobre mim**
- **Páginas** (lista e detalhe dos posts)
- **Mensagens** (inbox / outbox / nova mensagem)
- **Perfil**
- **Login / Logout / Registrar**

## Stack utilizada

- **Python 3**
- **Django**
- HTML / CSS
- Banco de dados **SQLite** (ambiente de desenvolvimento)

## Aprendizados principais

- Organização de um projeto Django em múltiplos apps (contas, páginas, mensagens).
- Implementação de autenticação e autorização (login, logout, cadastro de usuários).
- CRUD completo de páginas com templates, herança e mensagens de feedback.
- Criação de um sistema simples de mensagens privadas entre usuários.
- Uso de SQLite e migrações do Django para estruturar o banco de dados.


## Como rodar o projeto localmente

Pré-requisitos:  
Python 3 instalado e `git` configurado.

```bash
# Clonar o repositório
git clone https://github.com/martinanunesb/blogmartina.git
cd django-blog-messages

# Criar ambiente virtual
python -m venv .venv

# Ativar o ambiente virtual
# No Windows:
.venv\Scripts\activate


# No macOS / Linux:
source .venv/bin/activate

# Instalar dependências
pip install -r requirements.txt

# Aplicar migrações
python manage.py migrate

# Rodar o servidor de desenvolvimento
python manage.py runserver

