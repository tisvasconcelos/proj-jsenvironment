proj-jsenvironment (beta)
==================

##Environment Javascript with build and tests
Ambiente Javascript com build e testes

Build usando Closure Compiler (https://developers.google.com/closure/compiler/)
Obs.: Necess�rio Java e XCopy para usu�rio de windows

Testes usando Jasmine (http://pivotal.github.com/jasmine/)
Obs.: Necess�rio Ruby

Recomenda��es:

Para usu�rios de windows recomendo Link Shell Extension caso usem a parte de testes, 
assim voc� pode criar o link simbolico dos seus aquivos dentro da pasta tests.

Estamos usando jasmine mas pode ser usado qualquer framework de teste.

Build

Para rodar o build na linha de comando use rode o arquivo build.bat 
(em breve criaremos um arquivo .sh), o build ir� criar uma pasta js no mesmo 
diret�ria da pasta _js com todos os .js minimizados e sem a pasta build e tests 
j� que n�o s�o necess�rias quando for para produ��o.