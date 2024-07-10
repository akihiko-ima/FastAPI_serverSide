## Python version 3.11.7

#### FastAPI による backend 開発

- 仮想環境作成<br>
  => python -m venv env_fastAPI

- 仮想環境起動<br>
  => .\/env_fastAPI/Scripts/activate

- fastAPI 起動<br>
  => uvicorn main:app --reload

- path<br>
  cd .\main_dev

- requirements.txt<br>
  pip freeze > requirements.txt

## Docker

- 起動<br>
  => docker compose up -d

## DB

- pgAdmin
  => http://192.168.0.29:81/<br>
  PGADMIN_DEFAULT_EMAIL: fastapi@example.com<br>
  PGADMIN_DEFAULT_PASSWORD: password<br>

## alembic コマンド

- init<br>
  alembic init migrations

- migration<br>
  alembic revision --autogenerate -m "create items table"

- db に反映<br>
  alembic upgrade head
