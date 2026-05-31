# Todo API

Estudo de API RESTful de gerenciamento de tarefas construída com FastAPI. Projeto desenvolvido para estudo prático de Git workflow, FastAPI e Docker.

## Stack

- **Python** 3.12+
- **FastAPI** — framework web assíncrono
- **Uvicorn** — servidor ASGI
- **Pydantic** — validação de dados

## Pré-requisitos

- Python 3.12 ou superior
- pip
- Git

## Setup local

Clone o repositório:

```bash
git clone https://github.com/carlosLima565/Teste-FastApi.git
cd Teste-FastApi
```

Crie e ative o ambiente virtual:

```bash
# Windows
python -m venv venv
venv\Scripts\activate

# Linux/Mac
python -m venv venv
source venv/bin/activate
```

Instale as dependências:

```bash
pip install -r requirements.txt
```

Rode a aplicação:

```bash
uvicorn app.main:app --reload
```

A API estará disponível em `http://127.0.0.1:8000`.

## Endpoints

| Método | Rota      | Descrição                  |
|--------|-----------|----------------------------|
| GET    | `/`       | Status da API              |
| GET    | `/health` | Health check               |
| GET    | `/docs`   | Documentação Swagger (auto)|

## Documentação interativa

Com a aplicação rodando, acesse:

- **Swagger UI:** http://127.0.0.1:8000/docs
- **ReDoc:** http://127.0.0.1:8000/redoc

## Estrutura do projeto