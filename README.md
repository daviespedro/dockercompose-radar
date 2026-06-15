# Radar Cidadão 🏛️

## Descrição do Sistema
O **Radar Cidadão** é uma plataforma web focada na transparência de dados legislativos. O sistema permite o acompanhamento detalhado das despesas parlamentares e das proposições legislativas no Brasil, consumindo dados diretamente da API de Dados Abertos da Câmara dos Deputados. 

O objetivo do projeto é facilitar o acesso à informação pública de forma intuitiva e centralizada, permitindo que qualquer cidadão audite e analise o trabalho dos deputados federais.

## Tecnologias Utilizadas
* **Frontend:** HTML, CSS, JavaScript
* **Backend:** Python
* **Base de Dados:** MySQL
* **Infraestrutura/DevOps:** Docker, Docker Compose, AWS EC2

## Funcionalidades Principais
* Integração em tempo real com a API da Câmara dos Deputados.
* Consulta e filtragem de proposições legislativas por ano e por deputado específico.
* Página de relatórios dedicada à visualização de despesas parlamentares.
* Dashboard interativo e responsivo.

## Prints das Telas

- ![Dashboard Principal](dash.png)
- ![Deputados](depu.png)
- ![Relatorios](rela.png)
## Estrutura de Pastas
```text
/
├── app/                  # Código fonte da aplicação (HTML, CSS, JS, Python)
├── Dockerfile            # Instruções de construção da imagem Docker
├── docker-compose.yml    # Orquestração dos serviços (App + MySQL)
├── .env.example          # Modelo de variáveis de ambiente
├── README.md             # Documentação principal
└── GUIA_USUARIO.md       # Manual de execução para utilizadores# dockercompose-radar
