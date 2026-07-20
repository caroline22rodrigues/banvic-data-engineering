# banvic-data-engineering

# Estrutura do projeto

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

Passo 1 — Infraestrutura Criar repositório. 
Instalar ferramentas. 
Subir cluster Kind. 
Provisionar namespace com Terraform. 
Subir PostgreSQL. 
Subir Airflow.

Passo 2 — Pipeline Configurar Meltano. 
Configurar Tap e Target. 
Ingerir as 7 tabelas. 
Validar os dados.

Passo 3 — Orquestração Criar DAG. 
Adicionar Sensor. 
Configurar retries. 
Testar a execução.

Passo 4 — Entrega 
README. 
Diagrama. 
Vídeo. 
Revisão.
