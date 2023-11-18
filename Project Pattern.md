# Project Pattern

Este arquivo lista informações sobre a estrutura e tecnologias utilizadas no projeto, inclusive no processo de desenvolvimento do mesmo.

# Tabela de Conteúdos

- [Estrutura do Projeto](#estrutura-do-projeto)
- [Design Pattern](#Design-Pattern)
- [Desenvolvimento Orientado à Testes (TDD)](#desenvolvimento-orientado-à-testes-(TDD))
- [Tecnologias](#tecnologias)
    - [Projeto](#projeto)
        - [Node.js](#nodejs)
        - [NPM](#npm)
        - [Express](#express)
        - [Pug](#pug)
        - [Bootstrap](#bootstrap)
        - [Javascript](#javascript)
        - [CSS](#css)
        - [Jest](#jest)
        - [Heroku](#heroku)
        - [JawsDB MySQL](#jawsdb-mysql)
    - [Desenvolvimento](#desenvolvimento)
        - [VS Code](#vs-code)
        - [GitHub Copilot](#github-copilot)
        - [Git/Github](#gitgithub)
        - [MySQL Workspace](#mysql-workspace)
        - [Trello](#trello)
        - [Slack](#slack)
        - [Draw.io](#drawio)
        - [BR Modelo](#br-modelo)
        - [Figma](#figma)

# Estrutura do Projeto

![Diagrama da Estrutura de Diretórios](/Diagramas/Estrutura%20dos%20Diretórios.png "Estrutura de Diretórios")

| Diretório/Arquivo | Função |
| ----------------- | ------ |
| /src | Diretório onde estão os arquivos principais do projeto, como arquivos de configuração, controladores, rotas, etc. |
| /configs | Diretório de configuração do projeto, onde ficam armazenadas variáveis de configuração do projeto, como .env, db.config.js, general.config.js, etc. Todos os arquivos desse diretório tem a extensão .config.js. |
| /controllers | Diretório dos controladores do projeto, que recebem e processam as requisições http vindas das rotas. Todos os arquivos dese diretório tem a extensão .controller.js. |
| /middlewares | Diretório das middlewares do projeto, cuidam dos processos de autenticação da aplicação, como login, verificação de pagamento, etc. Todos os arquivos desse diretório tem a extensão .middleware.js. |
| /public | Diretório onde os arquivos públicos do projeto são alocados, esses arquivos são os únicos que o usuário tem acesso direto. |
| /assets | Diretório onde todos os assets do projeto estão, como imagens, fontes, ícones, etc. |
| /css | Diretório onde as folhas de estilo da aplicação são criadas. |
| /js | Diretório onde os scripts da aplicação são criadas |
| /views | Diretório onde as views do projeto estão, as views não são mostradas diretamente para o usuário, mas são renderizadas e convertidas para html no backend e enviadas para o usuário como resposta para a requisição http. |
| /routes | Diretório das rotas do projeto. Cada arquivo de rota agrupa um conjunto de rotas com finalidades relacionadas, como login e cadastro, etc. Todos os arquivos desse diretório tem a extensão .route.js. |
| /models | Diretório dos modelos dos dados da aplicação, contém o modelo dos dados do banco de dados que serão manipulados durante a execução da aplicação. Todos os arquivos desse diretório tem a extensão .model.js |
| /services | Diretório dos arquivos que controlam a lógica do sistema, como cadastrar um usuário ou gerar um cartão. Todos os arquivos desse diretório tem a extensão .service.js. |
| /utils | Diretório dos arquivos que controlam a lógica do sistema, como cadastrar um usuário ou gerar um cartão. Todos os arquivos desse diretório tem a extensão .service.js. |
| /test | Diretório onde são armazenados os testes do projeto, são separados em testes unitários, testes de integração e testes de sistema. Todos o arquivos desse diretório tem a extensão .test.js. |
| /unit | Diretório dos arquivos de teste que testam um módulo ou uma parte de uma funcionalidade, são subdivididos da mesma maneira que o /src. Todos os arquivos desse diretório tem a extensão .unit.test.js. | 
| /integration | Diretório dos arquivos de teste que testam funcionalidades inteira, com todos os seus módulos de uma vez. Todos os arquivos desse diretório tem a extensão .integration.test.js. |
| /system | Diretório dos arquivos de teste que fazem uma simulação do uso de uma funcionalidade como se fosse feita por um usuário real. Todos os arquivos desse diretório tem a extensão .system.test.js. |
| /index.js | Arquivo raiz do projeto, onde todos os módulos do projeto são unidos para a criação efetiva da aplicação. |
| /package.json | Arquivo que contém informações sobre o projeto, como o nome e a versão. |
| /.gitignore | Diretório onde estão os arquivos principais do projeto, como arquivos de configuração, controladores, rotas, etc. |

# Design Pattern

(Explicação Breve Sobre o que é)

# Desenvolvimento Orientado à Testes (TDD)

(Explicação Breve Sobre o que é)

# Tecnologias

Esta seção lista as tecnologias utilizadas no projeto, tanto no desenvolvimento quanto no projeto em si.

## Projeto (Sob Mudança)

As tecnologias utilizadas no projeto final são:
* [Node.js](#nodejs) - Interpretador de Javascript para o backend
* [Node Package Manager (NPM)](#npm) - Gerenciador de pacotes do Node.js
* [Express](#express) - Framework de Node.js para criação de aplicações web
* [Pug (Jade)](#pug) - Motor de template para Node.js
* [Bootstrap](#bootstrap) - Framework de CSS para criação de interfaces web
* [Javascript](#javascript) - Linguagem de programação para web
* [Cascading Styles Sheets (CSS)](#css) - Linguagem de estilização para web
* [Jest](#jest) - Framework de testes para Javascript
* [Heroku](#jest) - Plataforma de hospedagem de aplicações web
* [JawsDB MySQL](#jawsdb-mysql) - Banco de dados MySQL hospedado na nuvem

### Node.js

Node.js é um ambiente de execução de código aberto, multi-plataforma de Javascript. Roda a partir do motor de execução V8, o mesmo utilizado em navegadores como Google Chrome, possibilitando uma grande performance so código sem comprometer o uso de recursos do sistema.

O amplo suporta de sistemas de hospedagem e sistemas operacionais, o uso da linguagem javascript, que diminui a curva de aprendizado, e o caráter assíncrono orientado a eventos da linguagem a tornam uma ótima opção para o desenvolvimento de aplicações web.

### NPM

Node Package Manager, ou NPM, é o gerenciador de pacotes do Node.js. Ele é responsável por instalar e gerenciar as dependências do projeto, além de permitir a execução de scripts de teste, build, etc.

A sua facilidade de uso e o fato de já vir instalado junto com o Node.js o tornam uma ótima opção para o gerenciamento de pacotes.

### Express

Express é um framework de Node.js para criação de aplicações web. Ele é responsável por gerenciar as rotas da aplicação, além de permitir a criação de middlewares para a aplicação.

A sua flexibilidade e facilidade de aprendizado são os principais motivos para a sua escolha.

### Pug

Pug, anteriormente conhecido como Jade, é um motor de template para Node.js. Ele é responsável por renderizar as views da aplicação, convertendo-as para html e enviando-as para o usuário.

Por ser a linguagem padrão utilizada pelo Express e pelo código mais limpo e legível criado com sua linguagem, ele foi escolhido como motor de template.

### Bootstrap

Bootstrap é um framework de CSS para criação de interfaces web. Ele é responsável por criar a interface da aplicação, além de facilitar a criação de interfaces responsivas.

A facilitação na criação de aplicações mobile-friendly, além do aumento na produtividade durante a criação das páginas, foram os principais motivos para a sua escolha.

### Javascript

Javascript é uma linguagem de programação para web. Ela é responsável por criar a lógica da aplicação, além de permitir a criação de interfaces dinâmicas. Javascript é a linguagem padrão para o desenvolvimento de aplicações web.

### CSS

Cascade Style Sheets, ou CSS, é uma linguagem de estilização para web. Ela é responsável por estilizar a interface da aplicação, além de permitir a criação de interfaces responsivas.

Junta com o Bootstrap, o CSS é responsável por criar a interface da aplicação.

### Jest

Jest é um framework de testes para Javascript. Ele é responsável por executar os testes unitários e de integração na aplicação.

Seu foco na simplicidade e facilidade de aprendizado foram os principais motivos para a sua escolha.

### Heroku

Heroku é uma plataforma de hospedagem de aplicações web. Ela é responsável por hospedar a aplicação, além de permitir a criação de pipelines de CI/CD.

Sua grande poppularidade e extensa documentação, além do plano de estudante em parceria com o GitHub Students Pack, foram os principais motivos para a sua escolha.

### JawsDB MySQL

JawsDB MySQL é um banco de dados MySQL hospedado na nuvem. É utlilizado como um plugin do Heroku, permitindo a criação de um banco de dados MySQL na nuvem.

A existência de um plano gratuito, além da facilidade de uso, foram os principais motivos para a sua escolha.

## Desenvolvimeto

As tecnologias utilizadas no desenvolvimento do projeto são:
* [VS Code](#vs-code) - Editor de código
* [GitHub Copilot](#github-copilot) - Inteligência artificial para auxiliar no desenvolvimento
* [Git/GitHub](#gitgithub) - Sistema de controle de versão
* [MySQL Workspace](#mysql-workspace) - Ambiente de desenvolvimento de banco de dados
* [Trello](#trello) - Sistema de gerenciamento de projetos
* [Slack](#slack) - Sistema de comunicação
* [Draw.io](#drawio) - Ferramenta de criação de diagramas
* [BR Modelo](#br-modelo) - Ferramenta de criação de modelos de dados
* [Figma](#figma) - Ferramenta de criação de interfaces

### VS Code

VS Code é um editor de código. Ele é responsável por criar e editar os arquivos do projeto. Seu grande suporte para javascript, além de sua grande bibloteca de extenções, o tornam uma ótima opção para o desenvolvimento de aplicações web.

### GitHub Copilot

GitHub Copilot é uma inteligência artificial que auxilia no desenvolvimento de código. Ele é responsável por sugerir trechos de código para o desenvolvedor, além de sugerir nomes para variáveis e funções.

### Git/GitHub

Git é um sistema de controle de versão. Ele é responsável por gerenciar as versões do projeto, além de permitir o trabalho em equipe.

### MySQL Workspace

MySQL Workspace é um ambiente de desenvolvimento de banco de dados. Ele é responsável por criar e editar o banco de dados da aplicação.

### Trello

Trello é um sistema de gerenciamento de projetos. Ele é responsável por organizar as tarefas do projeto, além de permitir a criação de pipelines de desenvolvimento.

### Slack

Slack é um sistema de comunicação. Ele é responsável por permitir a comunicação entre os membros da equipe.

### Draw.io

Draw.io é uma ferramenta de criação de diagramas. Ele é responsável por criar os diagramas do projeto.

### BR Modelo

BR Modelo é uma ferramenta de criação de modelos de dados. Ele é responsável por criar os modelos do banco de dados do projeto.

### Figma

Figma é uma ferramenta de criação de interfaces. Ele é responsável por criar as interfaces do projeto.
