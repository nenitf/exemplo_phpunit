# exemplo-tdd

Exemplos simples de tdd, sendo as pastas:
- `app` o código do projeto
- `tests` os testes com phpunit
- `spec` os testes com kahlan

> Necessário possuir o [composer](https://getcomposer.org/)

```sh
# Instalação:
composer require


# Execução:
# Vale reparar que não é necessário instalar os binários, pois se houver a
# chamada do comando em um script do composer, o mesmo vai procurar em sua
# respectiva pasta (vendor/bin).
# Créditos: https://stackoverflow.com/a/45410662/9881278

# phpunit
composer phpunit

# kahlan
composer kahlan
```

## Frameworks de teste

* [phpuinit](http://www.phpunit.de)
* [kahlan](https://kahlan.github.io/docs/)
* [codeception](https://codeception.com/)
* [behat](https://docs.behat.org/en/latest/quick_start.html)
* [phpspec](http://www.phpspec.net/en/stable/)

### phpunit

#### Configuração

Siga os passos abaixo em ordem, mas caso esteja iniciando um projeto utilize primeiramente ``composer init -q``.
1. Adicione dependência no `composer.json` com ``composer require phpunit/phpunit --dev``
2. Instale dependências do `composer.json` com ``composer install``
3. Configure `phpunit.xml`
4. Atualize autoload com ``composer du`` <!-- produção: ``compose du -o`` -->

#### Criação de testes

1. Em `tests`, crie um arquivo que deve ter o mesmo nome da classe testada + ``Test.php``
2. Deve ser criada uma classe com o mesmo nome do arquivo extendendo ``PHPUnit\Framework\TestCase``
3. Escrever método(s) de teste (veja mais sobre em `dicas/Testes.md`) com o nome iniciando com ``test``

