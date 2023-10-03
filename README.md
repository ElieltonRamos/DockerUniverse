<h1 align="center">Docker Universe - Aprendendo sobre Docker</h1>

<p align="center">
  <img src="docker.png" alt="Docker Universe" width="300px">
</p>

<p align="center">
  <a href="https://github.com/ElieltonRamos/DockerUniverse">Repositório</a>
</p>

<p align="center">Apresento o resultado do projeto Docker-todo-list do módulo back-end da Trybe. Neste projeto, desenvolvi meus conhecimentos em Docker, enfrentando uma série de desafios para aprofundar minha compreensão sobre o funcionamento dessa incrível ferramenta. Com o Docker, fui capaz de criar ambientes de desenvolvimento altamente isolados e portáteis, tornando mais eficiente a execução de aplicativos e serviços em diferentes plataformas. Além disso, aprendi a definir configurações de contêineres por meio de arquivos Dockerfile e a gerenciar vários contêineres usando o Docker Compose. Essas habilidades são inestimáveis para minha carreira no desenvolvimento de software, pois permitem uma implantação mais rápida, um gerenciamento de recursos mais eficaz e a adoção de práticas DevOps modernas. Em resumo, o projeto Docker-todo-list foi uma oportunidade valiosa para solidificar meu conhecimento em Docker e sua aplicação prática no desenvolvimento de software.</p>

## O que e Docker?

<p>O Docker é um software de código aberto usado para implantar aplicativos dentro de containers virtuais. A conteinerização permite que vários aplicativos funcionem em diferentes ambientes complexos. Por exemplo: o Docker permite executar o WordPress em sistemas Windows, Linux e macOS, sem problemas.</p>

## Índice

- [Sobre o Projeto](#sobre-o-projeto)
- [Tecnologias Utilizadas](#tecnologias-utilizadas)
- [Funcionalidades](#funcionalidades)
- [Instalação e Uso](#instalação-e-uso)
- [Testes](#testes)
- [Autor](#autor)
- [Agradecimentos](#agradecimentos)
- [Licença](#licença)

## Sobre o Projeto

Durante o desenvolvimento deste projeto Docker, adquiri habilidades fundamentais em relação à criação, configuração e gerenciamento de contêineres Docker. Isso incluiu a compreensão dos princípios de isolamento de aplicativos e o uso eficiente de imagens para garantir a consistência em diferentes ambientes. Além disso, aprendi a automatizar tarefas de infraestrutura e a orquestrar serviços com o Docker Compose, tornando possível criar ambientes escaláveis e altamente eficientes para implantação de aplicações. Essas habilidades são cruciais para o desenvolvimento e gerenciamento eficaz de aplicações e ambientes em contêineres Docker, permitindo implantações consistentes e eficientes.

## Tecnologias Utilizadas

- [Docker](https://www.docker.com/)
- [Docker-Compose](https://docs.docker.com/compose/)
- [Jest](https://jestjs.io/pt-BR/)

## Funcionalidades

Cria um container em modo interativo sem inicia-lo e ele estará no estado "created" e não estará em execução.

Inicialização, listagem e remoção de contêineres.

Execução de comandos em contêineres sem acoplar a eles.

Download de imagens sem a criação de contêineres.

Configuração de contêineres em segundo plano com mapeamento de portas.

Construção de imagens personalizadas a partir de Dockerfiles.

Exposição de portas e definição de diretórios de trabalho nas imagens.

Manipulação de arquivos e comandos específicos durante a criação de imagens.

Integração de imagens personalizadas em um ambiente de orquestração com Docker Compose.

Compreensão de como contêineres e imagens podem ser usados para isolar, implantar e gerenciar aplicativos de forma eficiente.

## Instalação e Uso

Siga os passos abaixo para rodar o projeto localmente:

1. Clone o repositório:
```
 git clone git@github.com:ElieltonRamos/DockerUniverse.git
```
2. Navegue para o diretório do projeto:
```
cd DockerUniverse
```
3. Instale as dependências:
```
npm install
```
4. Navegue ate a pasta docker-commands
```
cd ./docker/docker-commands
```

Os arquivos principais do projeto estão na pasta `docker`, na raiz do projeto. Nela estão contidos:

Pasta `docker-commands`: onde ficarão os comandos exigidos pelos requisitos
</br>
Pasta `todo-app`: onde fica a nossa **pseudo-aplicação**, que servirá como base para nossos `Dockerfile`s e `Compose`

<details>
<summary><strong> ⚠️ Configurações mínimas para execução do projeto</strong></summary><br />

Na sua máquina você deve ter:

 - Sistema Operacional Distribuição Unix
 - Node versão 16
 - Docker
 - Docker-compose versão >=1.29.2

➡️ O `node` deve ter versão igual ou superior à `16.14.0 LTS`:
  - Para instalar o nvm, [acesse esse link](https://github.com/nvm-sh/nvm#installing-and-updating);
  - Rode os comandos abaixo para instalar a versão correta de `node` e usá-la:
    - `nvm install 16.14 --lts`
    - `nvm use 16.14`
    - `nvm alias default 16.14`

➡️ O `docker-compose` deve ter versão igual ou superior à`ˆ1.29.2`:
  * Caso necessário, acesse o [link da documentação oficial com passos para desinstalar](https://docs.docker.com/compose/install/#uninstallation) a versão atualmente instalada e instalar e versão requisitada.

</details>


## Testes
Certifique-se de que o Docker esteja instalado corretamente para que o avaliador funcione adequadamente. [Link para Instalação do docker](https://docs.docker.com/desktop/install/linux-install/)

Aqui também é importante que o seu usuário esteja no grupo `docker` (para que 
não haja a necessidade de rodar comandos utilizando o `sudo`)

O avaliador cria um **container especial** para executar a avaliação de `comandos`, `Dockerfiles` e `docker-compose`.

Esse container é temporário, portanto, ao começar ou terminar os testes locais, o avaliador remove automaticamente esse mesmo container, assim como seu volume associado.

O volume desse container mapeia a pasta `./docker/` do seu projeto, para dentro dele, ou seja, a raiz desse container vai conter as pastas `./docker-commands/`, `./todo-app/` e seu arquivo `./docker-compose.yml` quando estiver pronto.

Obs.: Caso o seu projeto esteja localizado em um diretório que contenha espaço no nome, os testes falharão (Exemplo: Area de trabalho). Nesse caso basta mover o projeto de pasta ou renomeá-lo (Exemplo: area-de-trabalho). Isso acontece porque o comando docker usado nos testes irá entender que o espaço no nome significa que está passando algum tipo de opção ou complemento extra.

**É necessário ter o Docker instalado corretamente na sua máquina para rodar os testes locais**.

Todos os requisitos do projeto serão testados automaticamente por meio do Jest. Basta executar o comando abaixo:

```bash
npm test
```

## Autor

Elielton Ramos

[![Envie-me um e-mail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:elieltonramos14@gmail.com)
[![Linkedin](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/elielton-ramos/)

## Agradecimentos

Sou grato à Trybe por proporcionar esse desafio enriquecedor e pela oportunidade de aprimorar minhas habilidades como desenvolvedor. Estou empolgado para aplicar os conhecimentos adquiridos em projetos futuros e continuar minha jornada de evolução profissional.

## Licença
Código Aberto (Open Source)

Este projeto é de código aberto e está disponível para toda a comunidade. Fique à vontade para explorar, clonar e contribuir para o projeto.