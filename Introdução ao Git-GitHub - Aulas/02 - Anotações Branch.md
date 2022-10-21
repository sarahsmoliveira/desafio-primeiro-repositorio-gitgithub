# BRANCH

## Conceitos Básicos

### 1. O que é

- Possibilita trabalhar no repositório sem fazer mudanças imediatas na linha principal

  - Alterações ficam salvas no servidor

- Cria uma "Linha Paralela" provisória

- Permite fundir as duas linhas após finalizar novas implementações

  > Não existe Branch sem Commit e Commit sem Branch

  

- `Main` x `Mater` : sugerido `Main`

  - GitHub - padrão `main`

  - Se criar local como `master`, e remoto estiver `main`:

    - Primeiro fazer `git pull origin main` - merge as duas branches

    - Ao fazer o push pro servidor: gitHub cria uma nova branch chamada `master`

      

- HEAD tag

  - Aponta último commit
  - Mostra em qual branch trabalhou por último

  

### 2. Criando e Navegando entre Branches (checkout)

- Local: `git checkout -b NOVA-BRANCH` - cria e vai para a nova branch
  -  `-b` - cria nova branch
- Remoto: `git pull origin NOVA-BRANCH`

- `git checkout` - navega entre as branchs



> ao navegar entre branches: leva arquivos novos junto (usar stash)



- `git branch`- lista as branchs e indica em qual está

### 3. Merge

- Na branch que receberá a nova: `git merge NOVA-BRANCH`

  

### 4. Renomeando e Deletando Branches

- Da branch: `git branch -m NOVO-NOME`
- De uma branch:`git branch -m nome-antigoNOME-ATIGO NOVO-NOME`

- `git branch -d NOME-BRANCH`

  - `-d`- deletar

  

### 5. STASH/ POP

- Guarda arquivos do index em uma "pasta provisória"
- Funciona como array: {0} , {1} ...{n} 
- Importante adicionar nota
- `git stash save "NOTA"`
  - se não colocar NOTA , salva como `wip `(work in progress)
- `git stash list`
  - recebe: `stash@{0}: on NOME-BRANCH: NOTA`
- `git pop n.stash`  -  ex `git pop 1` 
- `git stash clear` - limpa o stash

> pode pedir para resolver conflitos se alterações simultâneas



### 6. Histórico de Alterações (LOG)

- `git log`
- `git log PASTA` -  histórico de pasta específica

- `git log ARQUIVO`- histórico de arquivo específico
- `git log --one`- histórico resumido em 1 linha
  - recebe: `sha1 "NOTA"`
- `git log --graph` - forma mais ilustrada (movimentações / criações de branches)
- Ferramenas gráficas - 
  - `gitk` - windows (já instala junto com o gtHub)
  - gitkdestop - do GitHub ([link](https://desktop.github.com/) download)
  - gitkraken - Linux ([link](https://www.gitkraken.com/download) para download)

