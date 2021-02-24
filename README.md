# LEMP React infra
nginx
composer
mysql
node

## instructions

### src directory
backend => ./backend/src<br>
react => ./frontend/src<br>

### copy vendor and node_modules to host
run<br>
    docker-compose run --rm -v $pwd/backend/src:/lib-tmp -w /lib-tmp backend composer install<br>
    <br>
    docker-compose run --rm -v $pwd/frontend/src:/lib-tmp -w /lib-tmp frontend yarn install<br>