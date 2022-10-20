### Conceitos

* O git bash é um terminal extendido para otimizar o uso do GIT

### Comandos Simples

* Criar pasta no workspace: ' mkdir [file-name]'

* Git config --global user.email / Git config --global user.name - configura informações

* Git config --list     - _vê informações_

* mkdir          - _cria diretórios_

* rm                - _remove arquivos e diretórios_

* echo >README.md

* mv arquivo.ext ./repositoriodestino/ 

* ls                  - _mostra os diretórios e arquivos_

* cd  / cd ..     - _navegação_

* Ctrl+l           - _limpa a tela_

  

  > Criando arquivos primeiro no local e enviando ao gitHub

  * Criar pasta no workspace: ' mkdir [file-name]'
  * echo >README.md
  * "Git init" - _inicia repositório vazio_
  * criar no GitHub repositório com o mesmo nome - copiar link
  * Git remote add origin [link do repositório no gitHub]
  * Git push origin master  - _empurra para o GitHub_
  * Git status

  > Criando arquivos primeiro no gitHub e enviando para o local 

  * Criar no local repositório com o mesmo nome - NÃO iniciar git
  * Git clone - _clona repositório do GitHub_
  * Git add - _adiciona ao stage_
  * Git commit -m - _comita com uma nota curta sobre a ação_
  * Git status

