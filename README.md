
# Setup Docker Laravel 11 com PHP 8.3
[Assine a Academy, e Seja VIP!](https://academy.especializati.com.br)

### Passo a passo
Clone Repositório
```sh
git clone -b laravel-11-with-php-8.3 https://github.com/especializati/setup-docker-laravel.git app-laravel
```
```sh
cd app-laravel
```

Suba os containers do projeto
```sh
docker-compose up -d
```


Crie o Arquivo .env
```sh
cp .env.example .env
```

Acesse o container app
```sh
docker-compose exec app bash
```


Instale as dependências do projeto
```sh
composer install
```

Gere a key do projeto Laravel
```sh
php artisan key:generate
```

OPCIONAL: Gere o banco SQLite (caso não use o banco MySQL)
```sh
touch database/database.sqlite
```

Rodar as migrations
```sh
php artisan migrate
```

Acesse o projeto
[http://localhost:8000](http://localhost:8000)


Leia esse artigo do Macoratti
```sh
https://www.macoratti.net/19/02/dock_limp1.htm
```

Leia esse artigo para traduzir o laravel portugues brasil
```sh
https://github.com/lucascudo/laravel-pt-BR-localization
```


"watch": "vite build --watch"


No terminal bash
```sh
rm -rf .git

git init

 git add .

 git commit -m 'primeiro commit'

 git remote add origin git@github.com:moacirx/laravel11.git

 git branch -M main

 git push -u origin main
```






https://www.macoratti.net/19/02/dock_limp1.htm


Docker apagar todas as container
Contêineres:  docker container rm $(docker container ls -a -q)

Docker apagar todas as imagens
docker image rm $(docker image ls -a -q)
