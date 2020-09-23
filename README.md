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

# Sqlite

```
    touch database/database.sqlite

    php artisan migrate:fresh --seed
```

# Run

```
    cp .env.example .env

    sed -i '/DB_HOST/s/^/# /g' .env

    sed -i '/DB_PORT/s/^/# /g' .env

    sed -i '/DB_DATABASE/s/^/# /g' .env

    sed -i '/DB_USERNAME/s/^/# /g' .env

    sed -i '/DB_PASSWORD/s/^/# /g' .env

    php artisan key:generate
```

# API

* `http://127.0.0.1:8000/api/products`

* `http://127.0.0.1:8000/api/orders`

* `http://127.0.0.1:8000/api/people`

# Functionalities

* [x] Na tela principal, adicionar um filtro (`<input />`) por `CLIENTE`;

* [x] Na tela principal, adicionar um filtro (`<input />`) por `VENDEDOR`;

* [x] Na tela principal, o filtro por `CLIENTE` e `VENDEDOR` deve abrir um modal, em que seja permitida a navegação com as setas do teclado entre as linhas da tabela, adicionando o mesmo ao pressionar enter;

* [x] Na tela principal, adicionar um (`<button />`), que abrirá um modal para cadastrar um produto no carrinho;

* [x] Na tela principal, abaixo dos filtros, devem ser exibidos os produtos cadastrados no carrinho;

* [x] A listagem dos produtos deve permitir ordenação, ao clicar no nome da coluna em questão;

* [x] Ao abrir a página, o (`<input />`) do `CLIENTE` deve receber o foco;

* [x] Colocar um (`<input />`) de data ao lado da coluna data, na listagem dos produtos adicionados ao carrinho;

* [ ] Quando for informado um `CLIENTE`, se o mesmo tiver um `VENDEDOR INTERNO`, preencher o campo `VENDEDOR` e abrir o modal para cadastro do item;

* [x] No select `VENDA`, na listagem dos produtos, quando mesmo estiver com foco, expandí-lo a fim de permitir escolher o preço. (`SPACE KEY`)