# Git e Github

Essa documentação irá apresentar alguns 
comandos básicos do Git.

## Apêndice
**Tópicos que serão apresentados:**

- Configuração Inicial
- Repositórios
- Ramificação - Gestão de Branches
- Criando/Clonando um Repositório
- Salvando alterações sem commit

### Configuração Inicial
**Configuração inicial, na primeira vez utilizando o Git.**

- Definir o nome:
`git config --global user.name “Nome Sobrenome”`

- Definir o email:
`git config --global user.email “example@hotmail.com”`

### Repositórios
**Comandos relacionados aos repositórios.**

- Lista os arquivos/pastas na área onde foi aberta o terminal: `ls`

- Inicia um repositório vazio: 
`git init`

- Adiciona um arquivo editado, antes de fazer o commit: 
`git add nome_do_arquivo`

- Adiciona todos os arquivos editados: 
`git add .`

- Verifica o status do repositório: 
`git status`

- Desfaz a ação de adicionar: 
`git rm --cached nome_do_arquivo`

- Realiza commit do versionamento do projeto:
`git commit -m “mensagem a ser escrita”`

- Mostra o histórico de commits:
`git log`

### Ramificação - Gestão de Branches
**Comandos para realizar a gestão das branches**

- Mostra todas as branches locais e, a branch que está sendo utilizada: `git branch`

- Usado para criar uma branch: 
`git branch nome_da_branch`

- Remove a branch: 
`git branch -d nome_da_branch`

- Acessa uma branch: 
`git checkout nome_da_branch`

- Cria e acessa a branch: 
`git checkout -b nome_da_branch`

- Faz a unificação da branch que está acessando com outra branch ,que deseja trazer, unindo as alterações:
`git merge nome_da_branch`

### Criando/Clonando um Repositório
**Comandos relacionados a crição de repositórios remotos**

- Exibe os arquivos de um diretório local: `dir`

- Acessa a pasta do diretório local: 
`cd ./nome da pasta`

- Serve para clonar o repositório que foi criado no github para a máquina local:
`git clone {link do repositório ou chave ssh}`

- Exibe as URL’s dos possíveis diretórios remotos:
`git remote -v`

- Empurrar(Mandar) as alterações para o Github:
`git push`

- Utilizado quando uma branch é criada, mas não está no repositório remoto(origin):
`git push --set-upstream origin nome_da_branch`

- Puxa(Baixa) as alterações que estão no repositório remoto: `git pull`

### Salvando alterações sem commit
**Reservar as alterações para serem trabalhadas em 
um outro momento.**

- Arquiva as alterações feitas: `git stash`

- É usado para arquivos não rastreáveis, ou seja, recém criados:
`git stash --include-untracked`

- Lista as stashs: `git stash list`

- Chama a última stash feita: `git stash pop`

- Chama uma stash específica: 
`git stash pop stash@{id}`
