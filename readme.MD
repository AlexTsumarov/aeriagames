1. What have been implemented
    1. Simple REST API with one model (user)
    1. Basic auth
    1. ACL
    1. Fields validation
    1. Swagger/OpenAPI interface
1.  How to install
    1. composer install
    1. update DATABASE_URL in .env file
    1. bin/console doctrine:database:create
    1. php bin/console doctrine:migrations:migrate
    1. php -S 127.0.0.1:8000 -t public
    1. open browser page 127.0.0.1:8000/api
    1. use credentials admin/admin in basic auth dialog
1. How to extend
    1. https://api-platform.com/docs/distribution#installing-the-framework
    1. http://symfony.com/doc/current/doctrine.html#migrations-creating-the-database-tables-schema
    1. http://symfony.com/doc/current/doctrine.html#security 
1. Implementation goals
    1. Should be spent around 1-2 hours for implementation
    1. Should be used only sophisticated 3rd party parts with a good community
    1. Should be written as less code as possible
    1. The solution should require minimum efforts to be extented (SOLID)
1. Implementation flow
    1. Installed: api-platform.com (sf4 min), doctrine migrations, sf4 security
    1. Added: App\[Entity\User,Repository\UserRepository]
    1. Updated configs: .env, routing, security

