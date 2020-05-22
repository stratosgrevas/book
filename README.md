# book
Projeto de teste apenas para aprendizado no processo de testes automatizados do cakephp 3


https://book.cakephp.org/3/en/development/testing.html#running-tests



# FAQ

Como alterar a versão do PHP ?

* Ir nas varíaveis de ambiente do windows
* alterar o path = caminho do xampp do seu php (exemplo: D:\xampp\php)
* reiniciar o console, e executar o comando: php -v

Resultado:

$ php -v
PHP 7.3.9 (cli) (built: Aug 28 2019 09:28:48) ( ZTS MSVC15 (Visual C++ 2017) x64 )
Copyright (c) 1997-2018 The PHP Group
Zend Engine v3.3.9, Copyright (c) 1998-2018 Zend Technologies

---

Como clonar num diretório cheio ?

* cd /diretorio_cheio
* git init
* git remote add origin path_seu_git
* git add .
* git commit -am 'primeiro commit'
* git push -u origin master

Como criar um projeto cakephp 3 na linha de comando ?

* composer create-project --prefer-dist cakephp/app:^3.8 nome_do_projeto

Como rodar o cake bake na linha de comando (cakephp 3) ?

* crie o banco de dados
* configure o /app/config/app.php com o banco de dados
* cd na pasta /bin do projeto
* ./cake bake all nome_da_tabela

Como rodar os testes unitários na linha de comando (cakephp 3) ?

* cd diretorio do projeto
* vendor/bin/phpunit

Resultado dos testes:

PHPUnit 5.7.27 by Sebastian Bergmann and contributors.

...IIIII.....II                                                  15 / 15 (100%)

Time: 7.73 seconds, Memory: 15.00MB

OK, but incomplete, skipped, or risky tests!
Tests: 15, Assertions: 21, Incomplete: 7.



Como executar o coverage ?

* phpunit --coverage-html webroot/coverage tests/TestCase/Model/Table/ArticlesTableTest

Alguns erros podem ocorrer e será necessário executar com o comando:

* ./vendor/bin/phpunit --coverage-html webroot/coverage tests/TestCase

Para instalar ou atualizar o PHPUNIT:

* https://phpunit.de/getting-started/phpunit-5.html
* composer require --dev phpunit/phpunit ^5
* ./vendor/bin/phpunit --version

Será necessário instalar o XDEBUG:

$ ./vendor/bin/phpunit --coverage-html webroot/coverage tests/TestCase
PHPUnit 5.7.27 by Sebastian Bergmann and contributors.

Error:         No code coverage driver is available

Site para instalação do XDEBUG:

* https://xdebug.org/docs/install


https://phpunit.de/getting-started/phpunit-5.html
