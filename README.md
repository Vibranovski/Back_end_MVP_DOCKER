# PUC - Pontifícia Universidade Católica do Rio de Janeiro

<p align="center">
  <img src="https://images.squarespace-cdn.com/content/v1/59a8480fccc5c52fff14d38a/1529026153457-7W1EX1C6VUVUNIQN0CE1/image-asset.png" alt="PUC logo" border="0" width="100px">
</p>

# MVP desenvolvido para a Sprint: Desenvolvimento de back-end do curso de Pós Graduação em Engenharia de Software da PUC-RIO

### 🚀 Desenvolvedor
- <a href="https://www.linkedin.com/in/daniel-vcosta/">Daniel Vibranovski Costa</a> - daniel.vc7@gmail.com

## 🔍 Sumário

| Tópicos|
|---|
| [Definição do Problema](#-definição-do-problema)|
| [Estrutura do Repositório](#-estrutura-do-repositório)|
| [Tecnologias Utilizadas](#-tecnologias-utilizadas)|
| [Licença/License](#-licençalicense)|
| [Referências](#-referências)|
| [Agradecimentos](#-agradecimentos)|


## 📜 Definição do Problema

A proposta deste MVP surge da necessidade de melhorar a organização de tarefas dentro de equipes em uma empresa. Atualmente, a falta de centralização e transparência pode dificultar o acompanhamento do que cada membro está executando. Com a solução, cada usuário poderá visualizar não apenas suas próprias tarefas, mas também as dos demais integrantes do time, promovendo colaboração, alinhamento de prioridades e maior eficiência no fluxo de trabalho.

O presente MVP tem como meta desenvolver um Kanban funcional, estruturado por meio da criação de uma API que fará a integração entre o back-end e o front-end. Essa API será responsável por garantir a comunicação eficiente entre as camadas da aplicação, permitindo que os dados sejam processados, armazenados e exibidos de forma clara e organizada. Além disso, o sistema realiza integração com APIs externas, ampliando suas funcionalidades e possibilidades de uso. Todos os componentes da aplicação foram containerizados utilizando Docker, proporcionando portabilidade, isolamento e facilidade na implantação em diferentes ambientes. O resultado esperado é uma ferramenta prática e escalável para gerenciamento de tarefas, que possa evoluir conforme novas necessidades e funcionalidades forem sendo incorporadas.

Este repositório refere-se ao Projeto MVP (Minimum Viable Product) desenvolvido para a Sprint: Desenvolvimento Full Stack Básico do curso de Pós Graduação em Engenharia de Software da PUC-RIO.


## 📁 Estrutura do Repositório

- O **Back-end** do projeto está disponível em: [Back-end_MVP_DOCKER](https://github.com/Vibranovski/Back_end_MVP_DOCKER)  
- O **Front-end** do projeto está disponível em: [Front-end_MVP_DOCKER](https://github.com/Vibranovski/Front_end_MVP_DOCKER/tree/main)  

```
├── 📁 Back-end_MVP_DOCKER
│   ├── 📁 back-end
│   │   ├── 🐋 Dockerfile
│   │   ├── 🐋 docker-compose.yaml
│   │   ├── 🐋 .dockerignore
│   │   ├── 🐍 back_end.py
│   │   └── 🗄️ database.db
│   ├── 🏛️ arquitetura.drawio.png
│   └── 📄 README.md
│
├── 📁 Front-end_MVP_DOCKER
│   ├── 📁 front-end
│   │   ├── 🐋 Dockerfile
│   │   ├── 🐋 docker-compose.yaml
│   │   ├── 🐋 .dockerignore
│   │   ├── 🌐 index.html
│   │   ├── 🎨 style.css
│   │   └── ⚡ script.js
│   ├── 🏛️ arquitetura.drawio.png
│   └── 📄 README.md
```

Dentre os arquivos e pastas presentes na raiz do projeto, definem-se:  

- **README.md**: Arquivo que serve como guia e explicação geral sobre o projeto (arquivo atual).
- **Back-end_MVP_DOCKER**: Diretório responsável pela lógica do servidor e banco de dados.  
  - **back_end.py**: Arquivo Python que implementa a API do back-end — define rotas, valida entradas, aplica regras de negócio e realiza operações no banco de dados SQLite.  
  - **database.db**: Banco de dados SQLite utilizado pelo projeto, contendo as tabelas e os registros persistentes.  
  - **Dockerfile**: Instruções para construir a imagem Docker do back-end.  
  - **docker-compose.yaml**: Arquivo de orquestração que descreve como executar o serviço de back-end em containers, definindo serviços, redes e volumes para facilitar o ambiente de execução.  
  - **.dockerignore**: Lista de arquivos e diretórios a serem excluídos do contexto de build do Docker.
- **Front-end_MVP_DOCKER**: Diretório responsável pela interface do usuário.  
  - **index.html**: Estrutura principal da aplicação web.  
  - **style.css**: Estilos e layout da aplicação.  
  - **script.js**: Lógica de interação e comunicação com a API.  
  - **Dockerfile**: Instruções para construir a imagem Docker do front-end.  
  - **docker-compose.yaml**: Arquivo de orquestração que descreve como executar o serviço de back-end em containers, definindo serviços, redes e volumes para facilitar o ambiente de execução.  
  - **.dockerignore**: Lista de arquivos e diretórios a serem excluídos do contexto de build do Docker.



## 👨‍💻 Tecnologias Utilizadas

Bibliotecas:  

- [Flasgger](https://pypi.org/project/flasgger/0.5.4/): Utilizada para gerar automaticamente a documentação da API no formato Swagger, facilitando testes e visualização dos endpoints.  
- [Flask](https://flask.palletsprojects.com/en/stable/): Framework leve e flexível para criação do back-end da aplicação e definição das rotas da API.  
- [Flask-CORS](https://pypi.org/project/flask-cors/): Responsável por habilitar o compartilhamento de recursos entre diferentes origens (CORS), permitindo que o front-end acesse a API sem bloqueios.  

Linguagens:

- [HTML5](https://pt.wikipedia.org/wiki/HTML5): Linguagem de marcação usada para estruturar o conteúdo e os elementos da interface do usuário.  
- [CSS3](https://www.w3schools.com/css/): Linguagem de estilo utilizada para definir o design, layout e aparência visual da aplicação.  
- [JavaScript](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript): Linguagem de programação responsável por implementar a lógica do front-end e interações dinâmicas.  
- [Python3](https://www.python.org/): Linguagem de programação utilizada no back-end para construir a API, conectar ao banco de dados e processar as regras de negócio.  

Tecnologias:

- [Docker](https://www.docker.com/): é uma plataforma de tecnologia que permite empacotar e executar software em unidades padronizadas e isoladas, chamadas contêineres.

## 🏛️ Arquitetura

A arquitetura adotada para este MVP é composta por três camadas principais: interface (front-end), lógica de aplicação (back-end) e persistência (banco de dados). O front-end comunica-se com o back-end exclusivamente por meio de APIs REST, consumindo endpoints que expõem os recursos e ações necessárias para a interação do usuário. O back-end centraliza a lógica de negócio, valida entradas, orquestra chamadas a serviços externos e realiza operações de leitura e escrita no banco de dados SQLite.

Além da API interna, foi implementada uma integração com uma API externa que provê dados complementares. Essa API externa troca informações com o back-end; o back-end processa e normaliza os dados recebidos e os disponibiliza ao front-end através de seus próprios endpoints, permitindo que as informações adquiridas sejam apresentadas na interface do usuário de forma consistente e segura.

Arquitetura - C4 model Container:

<img src="https://res.cloudinary.com/dujx0hv4e/image/upload/v1764768985/arquitetura.drawio_ad7r7c.png">

Vale destacar que, dentre as alternativas avaliadas, a arquitetura selecionada corresponde ao cenário 1.1, pois refletia com maior fidelidade os requisitos do projeto e o fluxo de dados esperado entre interface, serviço e persistência.

## ⬇️ Instruções para Execução do Projeto

### 1️⃣ Executando o Back-end

1. Acesse a pasta do back-end:

   ```bash
   cd .\Back-end_MVP_1_Eng_Software\
   ```

Inicie o servidor executando o arquivo principal:

   ```bash
   python back_end.py
   ```

### 2️⃣ Executando o Front-end

Para executar e acessar o front-end via Docker, abra um terminal na pasta do projeto Front-end_MVP_DOCKER (ou em Front-end_MVP_DOCKER/front-end) e execute `docker-compose up -d` (ou, se preferir, `docker build -t front-end-mvp .` seguido de `docker run -d -p 8080:80 front-end-mvp`); depois, abra o navegador em http://127.0.0.1:8080  para visualizar a aplicação. P

ara parar os containers use `docker-compose down`.

### 3️⃣ Acessando a API via Swagger

Para acessar a documentação Swagger da API quando o back-end estiver em containers Docker, siga um dos fluxos abaixo.

Opção A — com docker-compose
1. Abra um terminal na pasta do back-end (ex.: Back-end_MVP_DOCKER/back-end).
2. Suba os containers:
```bash
docker-compose up -d
```
3. No navegador, abra:
http://127.0.0.1:5000/apidocs


## 📋 Licença/License

Todos os créditos estão reservados a Daniel Vibranovski Costa. O uso do recurso é livre, desde que para fins não comerciais.

## 🎓 Referências

### 1. Arquitetura de Software e Microserviços (CORE)
FOWLER, S. J. Microsserviços prontos e para a produção: construindo sistemas padronizados
em uma organização de engenharia de software. São Paulo: Novatec, 2017.

LEWIS, J.; FOWLER, M. Microservices: a definition of this new architectural term. 2014. Disponível em: https://martinfowler.com/articles/microservices.html. Acesso em: 01 dez. 2025.

NEWMAN, S. Building microservices: designing fine-grained systems. 2. ed. Sebastopol: O’Reilly
Media, 2021.

RICHARDS, M.; FORD, N. Fundamentals of software architecture: an engineering approach.
Sebastopol: O’Reilly, 2020.

EVANS, E. Domain-driven design: tackling complexity in the heart of software. Addison-Wesley,2003.

### 2. APIs, Protocolos e Integração

BIEHL, M. REST API design rulebook: designing consistent RESTful web service interfaces. Sebastopol: O’Reilly Media, 2011.

GEEWAX, J. J. API design patterns. Shelter Island: Manning, 2021. GRPC. Introduction to gRPC. 2023. Disponível em: https://grpc.io/docs/what-is-
grpc/introduction/. Acesso em: 01 dez. 2025.

## 3. DevOps, Cloud e Boas Práticas Organizacionais

KIM, G.; DEBOIS, P.; WILLIS, J.; HUMBLE, J. The DevOps handbook: how to create world-class
agility, reliability, and security in technology organizations. Portland: IT Revolution Press, 2016.

DOCKER. Docker Documentation. 2023. Disponível em: https://docs.docker.com/. Acesso em: 01 dez. 2025.

KUBERNETES. Kubernetes Documentation. Disponível em: https://kubernetes.io/docs/home/.
Acesso em: 01 dez. 2025.

### 4. Engenharia de Software e Qualidade

MARTIN, R. Clean code: a handbook of agile software craftsmanship. Prentice Hall, 2008.

PRESSMAN, R. S. Engenharia de software. 5. ed. Rio de Janeiro: McGraw-Hill, 2011.

FOWLER, M. Specification by Example. 2004. Disponível em:
https://martinfowler.com/bliki/SpecificationByExample.html. Acesso em: 01 dez. 2025. 


## 🙏 Agradecimentos

Agradeço à PUC-RIO e aos meus professores pela oportunidade de fazer esse MVP a partir da Sprint: Desenvolvimento Full Stack Básico do curso de Pós Graduação em Engenharia de Software da PUC-RIO
