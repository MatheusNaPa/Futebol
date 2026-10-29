# Futebol

Projeto Django 5.2 LTS. O banco é o PostgreSQL do Neon, via `DATABASE_URL`.

## Requisitos

- Python 3.13
- A variável `DATABASE_URL` em `.env`

Não grave a URL de conexão no Git. `.env` está no `.gitignore`. O modelo sem segredos é `.env.example`.

## Ambiente

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1
pip install -r requirements.txt
python manage.py check
```

As migrações no banco remoto ficam para depois da confirmação da conexão:

```powershell
python manage.py migrate
python manage.py runserver
```
