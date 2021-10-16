# Gerenciador de Variáveis de Ambiente PHP

Uma biblioteca simples para gerenciar variáveis de ambiente em PHP.

## Instalação

Para instalar esta depedência basta  execultar o comando abaixo:
```shell
composer require patric/dot-env
```
## Uso

Para usar esta biblioteca, basta criar um arquivo `.env` na raiz do projeto, seguindo o modelo abaixo (uma variável por linha):

```
DB_HOST=localhost
DB_USER=root
DB_PASS=pass
DB_NAME=database
DB_PORT=3307
```

```php
<?php

require 'vendor/autoload.php';

//CARREGAR VARIAVEIS DO AMBIENTE DO ARQUIVO NA RAIZ
Patric\DotEnv\Environment::load(__DIR__);

//OBTER AMBIENTE VAR
echo getenv('DB_HOST');

```

## Requisito

Está biblioteca precisa do PHP 7.0 ou maior.
