## Ambiente Python para desenvolvimento

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
cd Main/django-produtos
```

Criar o ambiente virtual

```
python -m venv ./venv
```

Para ativar o ambiente virtual

```
source venv/bin/activate (. venv/bin/activate)
```

Para Desativar o ambiente virtual

```
deactivate
```

Instalar o Django

```
pip install django
```

Criar um arquivo txt com as dependências do projeto

```
pip freeze > requirements.txt
```

Criar projeto

```
django-admin startproject setup .
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
