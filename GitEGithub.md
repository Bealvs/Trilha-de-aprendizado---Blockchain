# Git e Github

|Git|Github|
|-|-|
|Software|Serviço de hospedagem na nuvem|
|Controle de versão de arquivos|Colaboração e versionamento em repositórios remotos|
|Distribuídos|Gerenciamento de repositórios Git|
|Gratuítos|Planos gratuítos e pagos|
|Código aberto|Funcionalidades de código aberto e privadas|

## Git

Agora serão citados alguns comandos apresentados em vídeo:

Para configurar o seu Git Bash após tê-lo baixado:
```
git config --global user.name "NomeDeUsuario"
git config --global user.email "xxxxx@example.com"
git config --global init.default branch main
```
Para fazer o teste de comandos basta criar uma pasta, colocar um nome e arastar ela para o terminal do Git Bash.

**OBS.:** *cd* troca de diretório. Eu fiz para Windows.

```
cd: dir

```

Para iniciar:

```
git init
```

Informações Úteis:

|Untracked|Staged|
|-|-|
|Não pode criar cópias para criar outra versão depois|Pronto para fazer commit|

Estágios dos arquivos:  

1. Working;
2. Staging;
3. Commit.



Após baixar os arquivos oferecidos pela aula:
## Comando para adicionar o arquivo

```
git add . 

ou

git add index.html
```
## Verficar os status do arquivo

```
git status

```

## Para remover de staged e voltar a ficar untracked

```
git rm --cached index.html

```

## Para fazer o commit

```
git commit -m "Texto"

```

## Para ver as alterações feitas

```
git log

```

## Para ver as alterações de forma mais resumida

```
git log --oneline

```

## Para ver as alterações de forma ainda mais detalhada

```
git log -p

```

## Para pular diretamente para o commit

```
git commit -a -m "Texto"
```

## Uma forma de retirar do estágio *working*

```
git rm index.html
```

## Para restaurar arquivos

```
git restore --staged index.html
```

## Para renomear

```
git mv index.html newName.html
```

## Para alterar a mensagem do commit (o último feito)

```
git commit -m "Nome alterado do último commit" --amend
```

## Git reset

Existem 3 maneiras de resetar os dados:

|Soft|Mixed|Hard|
|-|-|-|
|Ele volta para o ponto anterior e coloca o que estava antes (mais recente) como *staged* (tá pronto para o *commit*), mas que ainda não foi commitado.|Da mesma forma que o *soft* mas não deixa *staged*, fica *unstaged*, neste caso, torna necessário fazer o *add .* e o *commit*|Remove tudo que foi feito depois do ponto escolhido para voltar e não tem como restaurar|
**OBS.:** O *mixed* é o default.

Exemplo:

```
git reset --soft <código do commit tirado do git log>
git reset --mixed <código do commit tirado do git log>
git reset --hard <código do commit tirado do git log>

```

## Git alias

Serve para criar um atalho local ou global:

```
git config alias.log1 "log --oneline"
git config --global alias.log1 "log --oneline"

```

## Branch

É recomendável não mexer na *main* e sim copiar, fazer a sua e depois fazer o *merge*.

Para criar a nova branch:

```
git branch AddBranch
```

Para trocar a branch:

```
git switch AddBranch
ou
git checkout AddBranch
```
Fazer o merge (mesclar branchs):

```
git merge AddMenu -m "Merge da branch AddMenu para a Main"
```
Remover branch

```
git branch -d AddMenu
```
---
## Github

É possível criar e nomear o repositório, e fazer as configurações iniciais:
```
git remote add origin <link do repositório>
git branch -M main
git push -u origin main
```
É importante que antes já tenham sido colocadas as credenciais, no VScode para e o token de acesso. 

Também existe a possibilidade de dar *push* de outras branchs que consiste em criar outras branchs,trocar para elas e dar *add .* e *commit*, voltar para a *main* e *git push --all*.

### Issues

Para "comentar" uma observação, problema e/ou melhoria no repositório de alguém, basta utilizá-lo para alertar o indivíduo:

1. Selecione *Issues* ao lado de *<> Code*;
2. Clique em *New Issue*;
3. Preencha os campos e logo abaixo selecione *Submit new Issue*;

### Release

Serve como uma espécie de lançamento de versões, para criar basta seguir os seguintes passos:

1. *<> Code*;
2. Logo abaixo de *About*, está *Release*;
3. *Create a new release*;

### Pull

Consiste em pegar do *github* para a máquina local, é equivalente a realizar *git fetch* e *git merge*:

```
git pull
```
---
## OBS.:

##### *É importante destacar que além do que foi visto nas aulas, também foram adicionadas informações de meu conhecimento. Tendo em vista que se trata de anotações, achei pertinente.*
---
