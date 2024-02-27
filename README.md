Aplicativo Flask de Compartilhamento de Fotos - FakePinterest

O código representa um aplicativo Flask chamado FakePinterest, proporcionando funcionalidades como login, criação de conta, perfil de usuário, upload de fotos e um feed de imagens. A estrutura modularizada e as dependências como SQLAlchemy e Flask-WTF facilitam a manutenção e expansão do projeto.

Instalação: pip install Flask Flask-WTF Flask-SQLAlchemy Flask-Login Flask-Bcrypt  # Execute o main.py para iniciar o projeto

Estrutura do Projeto:

main.py: Arquivo principal que inicia a aplicação Flask.
routes.py: Contém as rotas da aplicação, definindo o comportamento para diferentes URLs.
models.py: Define os modelos de dados usando SQLAlchemy, representando usuários e fotos.
forms.py: Contém classes de formulários usando Flask-WTF, que são utilizadas para validar e processar dados do usuário.
init.py: Arquivo de inicialização do pacote, onde são configuradas instâncias do Flask, SQLAlchemy, Bcrypt e LoginManager.
perfil.html, navbar.html, homepage.html, feed.html, criarconta.html: São templates HTML utilizados para renderizar as páginas da aplicação.
criar_banco.py: Script utilizado para criar o banco de dados com as tabelas definidas nos modelos.
Funcionalidades Principais:

Login e Registro: As rotas "/criarconta" e "/" são responsáveis por lidar com a criação de contas de usuário e autenticação/login.
Perfil de Usuário: A rota "/perfil/int:id_usuario" exibe o perfil do usuário, permitindo o envio de fotos.
Logout: A rota "/logout" efetua o logout do usuário.
Feed de Fotos: A rota "/feed" exibe um feed de fotos, ordenadas por data de criação.
Fluxo de Execução:

O aplicativo Flask é iniciado a partir de main.py.
Rotas são definidas em routes.py, cada uma lidando com diferentes aspectos da aplicação.
Os modelos de dados são definidos em models.py, utilizando SQLAlchemy.
Formulários são definidos em forms.py para validação de entrada do usuário.
Os templates HTML (por exemplo, perfil.html, navbar.html, homepage.html, feed.html, criarconta.html) são utilizados para renderizar as páginas da aplicação.
Dependências:

Flask: Framework web para Python.
Flask-WTF: Extensão do Flask para manipulação de formulários.
Flask-SQLAlchemy: Extensão para integração do Flask com SQLAlchemy.
Flask-Login: Extensão para gerenciamento de sessões de usuários.
Flask-Bcrypt: Extensão para hashing de senhas.
Conclusão:

O código fornece uma aplicação Flask completa com funcionalidades básicas de um sistema de compartilhamento de fotos.
A estrutura modularizada facilita a manutenção e expansão do código.
O uso de SQLAlchemy facilita a interação com o banco de dados SQLite.
As dependências externas fornecem recursos adicionais, como gerenciamento de login, segurança de senha e manipulação de formulários.


by Jônatas Mascarenhas Lima
