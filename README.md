# book
Projeto de teste apenas para aprendizado no processo de testes automatizados do cakephp 3


https://book.cakephp.org/3/en/development/testing.html#running-tests



# FAQ

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
