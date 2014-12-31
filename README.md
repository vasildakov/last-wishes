# Last Wishes - DDD Sample Application

## Install assets
    bower install

## Set up the project
    curl -sS https://getcomposer.org/installer | php
    php composer.phar install

## Create the database schema
    php bin/doctrine orm:schema-tool:create

## Run your Last Will bounded context
    php -S localhost:8080 -t src/Lw/Infrastructure/Ui/Web/Silex/Public

## Notify all domain events via messaging
    php bin/console domain:events:spread
