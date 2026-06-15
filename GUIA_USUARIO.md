# Guia do Utilizador - Radar Cidadão 🏛️

Este guia prático explica, de forma simples e direta, como descarregar, configurar e executar o **Radar Cidadão** no teu próprio computador (ambiente local) ou num servidor na nuvem (como a AWS EC2).

---

## 1. Pré-requisitos

Antes de iniciar a configuração, garante que tens as seguintes ferramentas instaladas no teu sistema:
* **Git**: Para clonar o repositório com o código fonte.
* **Docker**: Para isolar e executar a aplicação e o banco de dados.
* **Docker Compose**: Para orquestrar e subir todos os serviços com um único comando.

---

## 2. Como Baixar o Projeto

Abra o seu terminal (ou linha de comandos) e execute os seguintes comandos para clonar este repositório e entrar na pasta do projeto:

```bash
git clone [https://github.com/eugeniojonatas/Radar-Cidadao-Froggrammers.git](https://github.com/eugeniojonatas/Radar-Cidadao-Froggrammers.git)
cd Radar-Cidadao-Froggrammers

## 3. Como instalar o projeto e Como configurar o arquivo .env
O sistema precisa das suas credenciais para se conectar ao banco de dados MySQL.

Dentro da pasta do projeto, crie o ficheiro definitivo a partir do exemplo:

Bash
cp .env.example .env
Abra o ficheiro .env criado e substitua os dados falsos pelas suas credenciais reais. (Atenção: não altere o mysqlhost=db nem a port=5000).

Como rodar com Docker e Como subir os containers
Com o ficheiro .env pronto, inicie o sistema executando o seguinte comando:

Bash
docker compose up -d
O Docker irá baixar as imagens necessárias (incluindo a imagem publicada no Docker Hub) e colocar o sistema a funcionar em segundo plano.

Como acessar o sistema e Como acessar pelo navegador
Assim que os containers estiverem a rodar, abra o seu navegador de internet e aceda a:

Ambiente Local: http://localhost:5000

Nuvem (AWS EC2): http://IP_PUBLICO_DA_SUA_EC2:5000

Como parar o sistema
Para encerrar a aplicação e desligar o banco de dados de forma segura, execute no terminal:

Bash
docker compose down