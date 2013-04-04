*[Leia em Português](https://github.com/tisvasconcelos/proj-jsenvironment/blob/master/README-pt.md)*

# proj-jsenvironment (beta)
==================

## Environment Javascript with build and tests

Build using Closure Compiler (https://developers.google.com/closure/compiler/)

Obs.: It's necessary Java and XCopy for windows users

Tests using Jasmine (http://pivotal.github.com/jasmine/)

Obs.: It's necessary Ruby

### Recommendations:

For windows users we recommend install Link Shell Extension, if you use part of the tests, 
so you can create a symbolic link from your js files inside the tests folder.

We're using jasmine, but can be used any test framework

### Build

To run the build from the command line, run the file build.bat (soon we will create a .sh file) inside the folder build, this will createa folder call js in the same path of folder _js with all the js files minimized and without the build and tests folder, because is not necessary for production environment.

### Testes

Before you run the tests create the symbolic links from the core, modules e vendor folders inside the path tests\public

If your folders has another name, change the config file in tests\spec\support\jasmine.yml

To run the tests with jasmine go to the path tests e run this command:
```bash
rake jasmine
```