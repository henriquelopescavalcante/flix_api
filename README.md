🎬 Flix API

**Flix API** é uma API RESTful desenvolvida em Django REST Framework para gerenciamento de um catálogo de filmes e séries.
Este projeto foi projetado com foco em escalabilidade, organização e boas práticas de desenvolvimento para aplicações modernas.



📌 Visão Geral

Esta API permite o cadastro, consulta, atualização e exclusão de obras audiovisuais,
com recursos como autenticação via token, controle de permissões e filtros de busca.
É uma base robusta para qualquer sistema de streaming, catálogos de mídia ou integrações de back-end com aplicativos front-end.


⚙️ Tecnologias Utilizadas


- **Python 3.11+**
- **Django 5.x**
- **Django REST Framework**
- **SimpleJWT (JSON Web Tokens)**
- **SQLite (para testes locais)**
- **Docker (em construção)**

📂 Estrutura do Projeto


flix_api/
├── core/              # App principal com modelos e lógica de negócio
├── users/             # App para gerenciamento de usuários e autenticação
├── flix_api/          # Configurações do projeto
├── requirements.txt   # Dependências
└── manage.py


🚀 Funcionalidades

✅ Cadastro e login de usuários

✅ Token JWT com refresh

✅ CRUD de filmes e séries

✅ Filtros por título, gênero e ano

✅ Paginação de resultados

✅ Permissões por tipo de usuário (admin/padrão)


🔐 Autenticação
A autenticação é feita via JWT:


📤 Login
http
POST /api/token/


🔄 Refresh Token
http
POST /api/token/refresh/

Inclua o token no header para acessar rotas protegidas:
Authorization: Bearer <seu_token_aqui>


📥 Instalação e Uso Local

1. Clone o repositório
git clone https://github.com/henriquelopescavalcante/flix_api.git
cd flix_api

2. Crie um ambiente virtual
python -m venv venv
source venv/bin/activate  # ou venv\Scripts\activate no Windows

3. Instale as dependências
pip install -r requirements.txt

4. Rode as migrações e o servidor
python manage.py migrate
python manage.py runserver


🧪 Testes
Os testes automatizados podem ser executados com:
python manage.py test


📌 Próximos Passos

 Integração com Swagger/OpenAPI

 Deploy com Docker

 Melhorias em segurança e logging

👨‍💻 Autor
Desenvolvido por Henrique Lopes Cavalcante
 https://github.com/henriquelopescavalcante | https://www.linkedin.com/in/henriquelopescs/

