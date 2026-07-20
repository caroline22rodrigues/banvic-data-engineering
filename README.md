# banvic-data-engineering

## Objetivo
Este projeto tem como objetivo construir uma plataforma de dados moderna utilizando boas práticas de Engenharia de Dados e infraestrutura como código.

A solução será responsável por realizar a ingestão de dados provenientes de diferentes fontes, orquestrar os processos de extração e transformação, armazenar os dados em um banco PostgreSQL e disponibilizar informações confiáveis para análises futuras.

Para tornar o ambiente reproduzível e escalável, toda a infraestrutura será provisionada com Terraform e executada em um cluster Kubernetes local (Kind). A orquestração dos pipelines será realizada pelo Apache Airflow, enquanto o Meltano será utilizado para a ingestão de dados.

Além de atender aos requisitos do desafio técnico da BanVic, o projeto busca demonstrar conhecimentos em arquitetura de dados, automação de infraestrutura, conteinerização, orquestração de workflows e boas práticas de desenvolvimento.

## Arquitetura

```text
banvic-data-platform/
├── terraform/
│   ├── main.tf
│   ├── providers.tf
│   ├── variables.tf
│   ├── outputs.tf
│   └── terraform.tfvars
│
├── kubernetes/
│   ├── namespace.yaml
│   ├── postgres/
│   ├── airflow/
│   ├── secrets/
│   └── configmaps/
│
├── airflow/
│   ├── dags/
│   ├── plugins/
│   └── requirements.txt
│
├── meltano/
│   ├── meltano.yml
│   └── plugins/
│
├── data/
│   └── raw/
│
├── docs/
│
├── README.md
│
└── .gitignore
```

# Quadro de tarefas:

Passo 1 — Infraestrutura Criar repositório. <br>
Instalar ferramentas. <br>
Subir cluster Kind. <br>
Provisionar namespace com Terraform. <br>
Subir PostgreSQL. <br>
Subir Airflow.<br>

Passo 2 — Pipeline Configurar Meltano. <br>
Configurar Tap e Target. <br>
Ingerir as 7 tabelas. <br>
Validar os dados.<br>

Passo 3 — Orquestração Criar DAG. <br>
Adicionar Sensor. <br>
Configurar retries. <br>
Testar a execução.<br>

Passo 4 — Entrega 
README. <br>

## Tecnologias Utilizadas

## Estrutura do Projeto

## Como Executar

## Roadmap

## Autor
Diagrama. <br>
Vídeo. <br>
Revisão.<br>
