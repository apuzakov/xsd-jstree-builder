### [Установить Docker](https://docs.docker.com/install/)
### Скачиваем контейнер для сборки
```sh
docker pull shippingdocker/php-composer
```
### Клонируем репозиторий
```sh
git clone https://github.com/apuzakov/xsd-jstree-builder.git
```
### Переходим в папку с проектом
```sh
cd xsd-jstree-builder
```
## Собираем зависимости
```sh
docker run --rm -v $(pwd):/app -w /app shippingdocker/php-composer composer install
```
