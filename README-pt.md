*[Read in English](https://github.com/tisvasconcelos/proj-jsenvironment/blob/master/README.md)*

# proj-jsenvironment (beta)
==================

## Ambiente Javascript com build e testes

Build usando Closure Compiler (https://developers.google.com/closure/compiler/)

Obs.: Necessário Java e XCopy para usuário de windows

Testes usando Jasmine (http://pivotal.github.com/jasmine/)

Obs.: Necessário Ruby

### Recomendações:

Para usuários de windows recomendo Link Shell Extension caso usem a parte de testes, 
assim você pode criar o link simbolico dos seus aquivos dentro da pasta tests.

Estamos usando jasmine mas pode ser usado qualquer framework de teste.

### Build

Para rodar o build na linha de comando use rode o arquivo build.bat 
(em breve criaremos um arquivo .sh), o build irá criar uma pasta js no mesmo 
diretória da pasta _js com todos os .js minimizados e sem a pasta build e tests 
já que não são necessárias quando for para produção.

### Testes

Antes de rodar os teste crie os link simbólicos das pastas core, modules e vendor dentro da pasta tests\public

Caso suas pastas tenham outro nome altere o arquivo tests\spec\support\jasmine.yml

Para rodar os testes com o jasmine va até a pasta tests e digite o seguinte comando:
```bash
rake jasmine
```