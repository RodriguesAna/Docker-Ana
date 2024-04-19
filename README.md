Como iniciar o projeto: Entrar na pasta -> git clone: https://github.com/RodriguesAna/Docker-Ana.git

cd Docker-Ana

Subir Container docker compose up -d

Criar arquivo .env docker compose exec laravel_api cp .env.example .env

Instalar depedencias de API. docker compose exec laravel_api composer install

Execultar migração do Banco de Dados. docker compose exec laravel_api /var/www/html/artisan migrate:fresh

Criar usuario padrão do Banco de Dados. docker compose exec laravel_api /var/www/html/artisan db:seed

Stopar conteiner docker compose down

Para atualizar git pull

Docker-Ana cd laravel-nuxt

Subir containers e atualizar as imagens
docker compose up -d --build

Acessar api http://localhost:9090

Referências: Laravel Nuxt

https://www.youtube.com/watch?v=NY9yoqoN72w&t=1004s

https://www.youtube.com/watch?v=HLPoKz9j9KY&t=325s

Docker https://www.youtube.com/watch?v=ScmgXebitlQ&list=PLN_FLtIvNW0mo63rPdFBgL_UP5wF5eWLT
