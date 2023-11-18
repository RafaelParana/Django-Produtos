## Ambiente Python para desenvolvimento

- Após o download, dentro do [Visual Studio Code](https://code.visualstudio.com/), execute o comando para criar e utilizar o ambiente Python

Comando para criar o ambiente de desenvolvimento:

```
docker-compose build
```

Comando para utilizar o ambiente de desenvolvimento criado:

```
docker-compose up -d
```


## Rodando a API Produtos utilizando o framework Django

Acessar o diretório django-produtos

```
cd /referencial/src/django-produtos
```

Criar o ambiente virtual

```
python -m venv ./venv
```

Para ativar o ambiente virtual

```
source venv/bin/activate
```

Instalar o Django

```
pip install django
```

Criar um arquivo txt com as dependências do projeto

```
pip freeze > requirements.txt
```

Para executar o servidor Django

```
python manage.py runserver 0.0.0.0:8000
```

Para criar um app no Django

```
python  manage.py startapp produto
```

Criar a migração dos modelos Django no banco de dados

```
python manage.py makemigrations
```

```
python manage.py migrate
```

Criar um super usuário para o Django Admin

```
python manage.py createsuperuser
```

## Rodando a API Produtos utilizando o framework FastAPI

Acessar o diretório fastapi-produtos

```
cd /referencial/src/fastapi-produtos
```

Para instalar os pacotes necessários para rodar o servidor FastAPI

```
pip install fastapi uvicorn
```

Para executar o servidor FastAPI

```
uvicorn app:app --host 0.0.0.0 --port 8080 --reload
```