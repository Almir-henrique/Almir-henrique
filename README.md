<div align="center">

# Henrique Dantas

### Full Stack Developer | Backend | Data & Systems

**Desenvolvedor Full Stack em formação, com foco em aplicações web, APIs, bancos de dados e soluções orientadas a dados.**

[![GitHub](https://img.shields.io/badge/GitHub-Almir--henrique-181717?style=for-the-badge\&logo=github)](https://github.com/Almir-henrique)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Henrique%20Dantas-0A66C2?style=for-the-badge\&logo=linkedin)](https://www.linkedin.com/in/henrique-dantas-profile)
[![Email](https://img.shields.io/badge/Email-almirhenrique18%40gmail.com-EA4335?style=for-the-badge\&logo=gmail)](mailto:almirhenrique18@gmail.com)

**Recife, Pernambuco, Brasil**

</div>

---

## Perfil

Sou desenvolvedor Full Stack em formação, atualmente no **último ano de Análise e Desenvolvimento de Sistemas**, com conclusão prevista para **2026**.

Minha atuação está concentrada no desenvolvimento de sistemas web, construção de APIs, integração entre frontend e backend, bancos de dados e implementação de regras de negócio.

Tenho experiência prática com **JavaScript, TypeScript, React, Node.js, Express, APIs REST, PostgreSQL, MySQL e MongoDB**, além de conhecimentos em **Git/GitHub, Docker, Postman, Power BI, ETL, redes e infraestrutura**.

Também atuo profissionalmente com **suporte técnico em TI**, trabalhando com atendimento de usuários, diagnóstico de incidentes, manutenção de hardware e software, redes e ambientes Windows/Linux.

Meu objetivo é unir desenvolvimento de software, infraestrutura e dados para construir sistemas organizados, escaláveis e orientados a necessidades reais.

---

# Tech Stack

## Frontend

<p>
<img src="https://skillicons.dev/icons?i=html,css,js,ts,react,tailwind" />
</p>

* HTML5
* CSS3
* JavaScript ES6+
* TypeScript
* React
* Tailwind CSS
* Interfaces responsivas
* Componentização
* Integração com APIs

---

## Backend

<p>
<img src="https://skillicons.dev/icons?i=nodejs,express" />
</p>

* Node.js
* Express.js
* APIs RESTful
* Arquitetura MVC
* Autenticação e autorização
* JWT
* CRUD
* Regras de negócio
* Integração frontend/backend
* Comunicação em tempo real com Socket.IO

---

## Databases

<p>
<img src="https://skillicons.dev/icons?i=postgres,mysql,mongodb" />
</p>

* PostgreSQL
* MySQL
* MongoDB
* SQL
* CRUD
* Modelagem relacional
* Consultas
* Persistência de dados
* Isolamento de dados por contexto empresarial

---

## Data & BI

<p>
<img src="https://skillicons.dev/icons?i=excel" />
</p>

* SQL
* Power BI
* ETL
* Modelagem de dados
* Dashboards interativos
* Excel Avançado
* Análise de dados

---

## DevOps & Ferramentas

<p>
<img src="https://skillicons.dev/icons?i=git,github,docker,nginx,postman,vscode" />
</p>

* Git
* GitHub
* Docker
* Nginx
* Postman
* VS Code
* Versionamento de código
* APIs e testes de requisições

---

## Infrastructure & Support

* TCP/IP
* DNS
* DHCP
* Redes de computadores
* Windows
* Linux
* Diagnóstico de hardware
* Diagnóstico de software
* Atendimento N1/N2
* Gestão de chamados
* Manutenção de equipamentos
* Troubleshooting

---

# Engenharia de Software

Além das tecnologias, tenho conhecimentos em conceitos fundamentais de engenharia de software:

* Programação Orientada a Objetos
* Lógica de Programação
* Estrutura de Dados
* SOLID
* DDD
* MVC
* APIs REST
* Autenticação e autorização
* Modelagem de dados
* Separação de responsabilidades
* Arquitetura modular
* Controle de versão com Git
* Integração entre sistemas

---

# Projeto em Destaque

## Nexus Ponto

### Sistema Full Stack para gestão de ponto eletrônico corporativo

O **Nexus Ponto** é uma aplicação web desenvolvida para gerenciamento de jornada de trabalho, permitindo que funcionários registrem seus pontos e que empresas acompanhem informações relacionadas à jornada dos colaboradores.

O projeto evoluiu de um MVP inicialmente baseado em armazenamento local para uma arquitetura com **backend, banco de dados PostgreSQL, autenticação JWT e comunicação em tempo real**.

### Arquitetura

```text
                    NEXUS PONTO
                         │
          ┌──────────────┴──────────────┐
          │                             │
       Frontend                       Backend
          │                             │
       React                    Node.js + Express
          │                             │
          └──────────────┬──────────────┘
                         │
                    REST API
                         │
              ┌──────────┴──────────┐
              │                     │
          PostgreSQL             Socket.IO
              │                     │
       Persistência             Real-time
        de dados               communication
```

### Stack utilizada

<p>
<img src="https://skillicons.dev/icons?i=react,js,nodejs,express,postgres,git,github" />
</p>

`React` · `JavaScript` · `Node.js` · `Express.js` · `PostgreSQL` · `REST API` · `JWT` · `Socket.IO` · `Git` · `GitHub`

### Backend

O backend foi estruturado utilizando **Node.js + Express**, disponibilizando endpoints para comunicação entre a aplicação e o banco de dados.

Principais conceitos implementados:

* API REST
* Node.js
* Express.js
* PostgreSQL
* JWT
* Autenticação
* Autorização
* Regras de negócio
* Controle de acesso
* Persistência de dados
* Comunicação em tempo real
* Socket.IO

### Autenticação e autorização

O sistema utiliza **JWT (JSON Web Token)** para autenticação e controle de acesso.

A arquitetura considera diferentes contextos de utilização, incluindo:

```text
Empresa
   │
   ├── Autenticação
   ├── Funcionários
   ├── Registros de ponto
   └── Informações da empresa

Funcionário
   │
   ├── Autenticação
   ├── Perfil
   ├── Registro de ponto
   └── Histórico de jornada
```

O sistema também trabalha com **isolamento entre empresas e funcionários**, evitando que dados de diferentes contextos sejam tratados de forma indevida.

### Controle de jornada

O registro de ponto segue uma sequência de estados definida pela regra de negócio:

```text
ENTRADA
   ↓
INÍCIO DO INTERVALO
   ↓
FIM DO INTERVALO
   ↓
SAÍDA
```

Essa estrutura permite controlar a jornada diária e validar a sequência correta dos registros.

### Comunicação em tempo real

O projeto utiliza **Socket.IO** para comunicação em tempo real entre cliente e servidor.

Isso permite trabalhar com eventos como:

```text
Funcionário registra ponto
        ↓
Backend processa registro
        ↓
Evento Socket.IO
        ↓
Interface da empresa recebe atualização
```

Dessa forma, informações podem ser atualizadas sem depender exclusivamente de atualizações manuais da página.

### Banco de dados

O projeto utiliza **PostgreSQL** como banco de dados principal.

O backend estabelece conexão com o banco para persistência dos dados relacionados a:

* Usuários
* Empresas
* Funcionários
* Registros de ponto
* Jornadas
* Autenticação
* Relacionamentos entre entidades

### Objetivos técnicos do projeto

O Nexus Ponto também serve como laboratório prático para aplicação de conceitos de:

* Desenvolvimento Full Stack
* Arquitetura cliente-servidor
* APIs REST
* Autenticação JWT
* Autorização
* Banco de dados relacional
* PostgreSQL
* Regras de negócio
* Comunicação em tempo real
* Isolamento de dados
* Organização de backend
* Versionamento com Git/GitHub

**Repository:**
https://github.com/Almir-henrique/nexus-ponto-mvp

---

# Outros Projetos

## CRUD Full Stack

Aplicação Full Stack desenvolvida para praticar construção de APIs, operações CRUD, integração com banco de dados e organização de backend.

### Tecnologias

`Node.js` `Express.js` `MySQL` `JavaScript` `REST API` `MVC`

### Conceitos

* API RESTful
* CRUD
* MVC
* MySQL
* Rotas
* Requisições HTTP
* Persistência de dados
* Integração backend/database

**Repository:**
https://github.com/Almir-henrique/crud-fullstack-app

---

## Conex Contadores

Aplicação institucional desenvolvida para presença digital e geração de leads.

### Tecnologias

`HTML5` `CSS3` `JavaScript` `EmailJS`

### Características

* Design responsivo
* Interface institucional
* Formulários
* Integração com EmailJS
* Experiência desktop/mobile
* Estrutura voltada para conversão

**Repository:**
https://github.com/Almir-henrique/CONEX-SITE

**Production:**
https://conexcontadores.com.br

---

## site-ibmemorial

Projeto institucional em desenvolvimento para a **Igreja Batista Memorial do Recife**.

A aplicação está sendo estruturada visando futuras integrações com backend, APIs e banco de dados.

### Tecnologias

`HTML5` `CSS3` `JavaScript`

### Roadmap técnico

```text
Interface
   ↓
Componentização
   ↓
API
   ↓
Backend
   ↓
Banco de Dados
   ↓
Área Administrativa
   ↓
Gerenciamento de Conteúdo
```

---

# GitHub Analytics

<div align="center">

<img height="180em" src="https://github-readme-stats.vercel.app/api?username=Almir-henrique&show_icons=true&theme=github_dark&include_all_commits=true&count_private=true&hide_border=true"/>

<img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Almir-henrique&layout=compact&theme=github_dark&hide=html,css&hide_border=true"/>

</div>

<br>

<div align="center">

<img src="https://github-readme-streak-stats.herokuapp.com/?user=Almir-henrique&theme=github-dark-blue&hide_border=true"/>

</div>

---

# Formação

## Análise e Desenvolvimento de Sistemas

**UNINASSAU**

**Último ano — conclusão em 2026**

---

## Técnico em Desenvolvimento de Sistemas

**ETE Cícero Dias**

Concluído em 2024

---

# Experiência

## Estagiário de Suporte em TI

**FOP/UPE — Universidade de Pernambuco**

Atuação envolvendo suporte aos usuários, equipamentos e infraestrutura de TI.

### Principais atividades

* Atendimento e suporte técnico
* Diagnóstico e resolução de incidentes
* Manutenção de hardware
* Manutenção de software
* Configuração e troubleshooting
* Redes de computadores
* Ambientes Windows/Linux
* Gestão de chamados
* Suporte à infraestrutura de TI

Essa experiência complementa minha formação em desenvolvimento ao proporcionar contato direto com **infraestrutura, redes, usuários e resolução de problemas em ambientes reais**.

---

# Competências

<div align="center">

| Desenvolvimento | Backend   | Dados      | Infraestrutura |
| --------------- | --------- | ---------- | -------------- |
| React           | Node.js   | SQL        | TCP/IP         |
| TypeScript      | Express   | PostgreSQL | DNS            |
| JavaScript      | REST API  | MySQL      | DHCP           |
| HTML/CSS        | JWT       | Power BI   | Windows        |
| Tailwind        | Socket.IO | ETL        | Linux          |

</div>

---

# Áreas de Interesse

```text
FULL STACK DEVELOPMENT
BACKEND DEVELOPMENT
FRONTEND DEVELOPMENT
SOFTWARE ENGINEERING
API DEVELOPMENT
DATABASE DEVELOPMENT
DATA ANALYSIS
BUSINESS INTELLIGENCE
TECHNICAL SUPPORT
IT INFRASTRUCTURE
```

---

# Atualmente evoluindo em

* Desenvolvimento Full Stack
* Arquitetura de aplicações web
* Backend com Node.js
* React e TypeScript
* APIs REST
* PostgreSQL
* Autenticação e autorização
* Comunicação em tempo real
* Docker
* Engenharia de software
* Bancos de dados
* Análise de dados
* Business Intelligence

---

# GitHub

<div align="center">

### Código, arquitetura e aprendizado contínuo.

[![GitHub](https://img.shields.io/badge/Explore%20my%20repositories-181717?style=for-the-badge\&logo=github)](https://github.com/Almir-henrique)

</div>

---

# Contato

<div align="center">

**Henrique Dantas**

Full Stack Developer | Backend | Data

[LinkedIn](https://www.linkedin.com/in/henrique-dantas-profile)

[GitHub](https://github.com/Almir-henrique)

[almirhenrique18@gmail.com](mailto:almirhenrique18@gmail.com)

**Recife — Pernambuco — Brasil**

</div>

---

<div align="center">

`BUILD` · `LEARN` · `SOLVE` · `EVOLVE`

</div>
