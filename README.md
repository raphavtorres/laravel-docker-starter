# Setup Docker Laravel 11 com PHP 8.3

### Step by step

Clone project

Create .env file

```sh
cp .env.example .env
```

Upload project containers

```sh
docker compose up -d
```

Access app container

```sh
docker compose exec app bash
```

> All inside container

Install project dependencies

```sh
composer install
```

Generate Laravel project key

```sh
php artisan key:generate
```

OPTIONAL: Generate SQLite database (if you are not using MySQL)

```sh
touch database/database.sqlite
```

Run migrations

```sh
php artisan migrate
```

Access Project
[http://localhost:8000](http://localhost:8000)

# NOTES

[Laravel e-commerce](https://www.youtube.com/watch?v=kR4fhanxOf4&list=PLm8sgxwSZofdmlPxaDB7fRLv_NVe2uFKl&ab_channel=WebTechKnowledge)
[Laravel with NextJS](https://www.youtube.com/watch?v=Ri65-XNBtYA&ab_channel=Laravel)
[Laravel Projects](https://laraveldaily.com/post/large-laravel-open-source-projects)
[Youtube Laravel Channel](https://www.youtube.com/@eraufi/videos)

### List commands with artisan

```sh
php artisan
```

## Authentication

[Breeze Docs](https://laravel.com/docs/11.x/starter-kits#laravel-breeze)

```sh
composer require laravel/breeze --dev
```

Check the dependency instalation in compose.json and .lock

Go to terminal to install with npm

```sh
npm install
```

Build files and generate manifest.json

```sh
npm run build
```
