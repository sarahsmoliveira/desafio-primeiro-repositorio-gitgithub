### Conceitos Básicos

* O git bash é um terminal extendido para otimizar o uso do GIT
* Chaves de segurança - Sha1 (40 caracteres)
* Quando se cria um arquivo novo local ele fica _untracked_


#### Ciclo da vida 🦁:
* antes do git: **untracked** 
* entrou no git: `unmodified`
* se for feita alguma ateração - `➡️ Modified`
* adicionou (comando `git add`) -  `➡️ Staged`
* `➡️ Commit`  -   `➡️ unmodified 🔄` 

### Comandos Simples

* Criar pasta no workspace: `mkdir [file-name]`

* `Git config --global user.email / Git config --global user.name ` - configura informações

* `Git config --list` - _vê informações_

* `mkdir`      - _cria diretórios_

* `rm`              - _remove arquivos e diretórios_

* `echo >README.md` - _cria arquivo readme em md_

* `mv arquivo.ext ./repositoriodestino/` - _muda o arquivo.ext de pasta_
* `Git status` - _informações se existem arquivos modificados sem commit_
* `git remote -v` - _mostra quais repositórios onlines estão linkados_


* `ls`              - _mostra os diretórios e arquivos_

* `cd  / cd ..`     - _navegação_

* `Ctrl+l`       - _limpa a tela_

  

### Criando arquivos primeiro no local e enviando ao gitHub

  - Criar pasta no workspace: `mkdir [file-name]`
  - `echo >README.md`
  - `Git init` - _inicia repositório vazio_
  - criar no GitHub repositório com o mesmo nome - copiar link
  - `Git remote add origin [link do repositório no gitHub]`
  - `Git push origin master`  - _empurra para o GitHub_
  - 
  - se editar no gitHub depois, para atualizar no local - `git pull`

### Criando arquivos primeiro no gitHub e enviando para o local 

  * Criar no local repositório com o mesmo nome - NÃO iniciar git
  * `Git clone` - _clona repositório do GitHub_
  * 
  * - se editar no local depois, primeiro segue o ciclo no no git bash ->
  * `Git add`- _adiciona ao stage_
  * `Git commit -m ` - _comita com uma nota curta sobre a ação_
  *
  *  e então para atualizar no gitHub - `git push`
  *  

[Link](https://git-scm.com/downloads) para download do Git

_SH Oliveira_ 🐾
