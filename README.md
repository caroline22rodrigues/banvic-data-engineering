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
Diagrama. <br>
Vídeo. <br>
Revisão.<br>
