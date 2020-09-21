# SalesScreen

Repository containing the requirements for the project

# Server

```
    composer create-project --prefer-dist laravel/laravel server

    php artisan make:model Order -mcr

    php artisan make:model Product -mcr

    php artisan make:model Consumer -mcr
```

# View

```
    npx create-react-app view

    npm install react-router-dom --save

    npm install react-bootstrap bootstrap

    npm install axios

    npm install react-icons --save

    sudo sysctl -w fs.inotify.max_user_watches=100000
```

# Database

```
    psql --user postgres --host 127.0.0.1

    CREATE DATABASE alfa;

    CREATE USER alfa with encrypted password 'P@ssw0rd';

    GRANT ALL PRIVILEGES ON DATABASE alfa to alfa;
```

# Run

```
    cp .env.example .env
```

# API

http://127.0.0.1:8000/api/products

http://127.0.0.1:8000/api/orders

http://127.0.0.1:8000/api/people

# Functionalities

* ordenar os itens na busca e os itens que foram adicionados

* quando informar o cliente já encontra o vender interno e abre o popup do item