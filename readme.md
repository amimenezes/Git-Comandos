# Comandos Git

## Versão: 2022-07-19

## Melhores Práticas no Github

| Comando | Descrição |
| ------- | --------- |
| WIP | Trabalho em Progresso |
| FEAT | Funcionalidade Nova |
| FIX | Correção |
| REFACTOR | Refatoração de uma funcionalidade que estava funcionando, mas estava meio feia, mudança de estrutura, etc.|
| BUG | Resolução de bug |
| TEST | Para algum teste que venha a implementar |

## Criar um novo repositório na linha de comando (terminal)

| Comando | Descrição |
| ------- | --------- |
| `echo "# Git-Comandos" >> README.md` | ... |
| `git init` | ... |
| `git add README.md` | ... |
| `git commit -m "first commit"` | ... |
| `git branch -M main` | ... |
| `git remote add origin https://github.com/amimenezes/Git-Comandos.git` | ... |
| `git push -u origin main` | ... |
___

## Empurrar um repositório existente pela linha de comando (terminal)

`git remote add origin https://github.com/amimenezes/Git-Comandos.git`
`git branch -M main`
`git push -u origin main`

### Uma lista dos comandos Git mais usados

--

### Resumo - Passo a Passo

| Comando | Descrição |
| ------- | --------- |
| `git status` | Verifica se têm arquivos para subir do repositório local para o remoto |
| `git add .` | Adiciona todos os arquivos que foram alterados/criados |
| `git status` | Verifica se os arquivos estão prontos para serem adicionados |
| `git commit -m "Meu texto descritivo."` | Escreve a mensagem com a descrição. |
| `git pull origin main` | Atualiza a branch atual (version-1, local) com a main (remot no site do Git) |
| `git push origin version-1` | Sobe as atualizações para a branch version-1 remota |

Ir no site do github, acesar o git remoto e fazer a solicitação de Pull Request da versão atual: version-1, para a main.
Se tudo estiver correto no código, aí aprova o Merge Request para a main remota.

| Comando | Descrição |
| ------- | --------- |
| `git pull origin main` | Mantém atualizada a branch local (version-1) |

### Criar nova Branch

| Comando | Descrição |
| ------- | --------- |
| `git checkout main` | Salta para a main local |
| `git pull origin main` | Busca a atualização da remota para a local |
| `git checkout -b nomeDaBranch` | Cria uma nova branch |

### Obtendo & Criação de Projetos

| Comando | Descrição |
| ------- | --------- |
| `git init` | Inicializa um repositório Git local |
| `git clone ssh://git@github.com/[usuario]/[nome-repositorio].git` | Cria uma cópia local de um repositório remoto |

### Básicos

| Comando | Descrição |
| ------- | --------- |
| `git status` | Checa o status |
| `git add [nome-arquivo.txt]` | Adiciona um arquivo para área de stage |
| `git add -A` | Adiciona todos os arquivos novos ou modificados para a área de stage |
| `git commit -m "[Mensagem de Commit]"` | Comita as alterações |
| `git rm -r [nome-arquivo.txt]` | Remove um arquivo (ou pasta) |

### Branching & Merging

| Comando | Descrição |
| ------- | --------- |
| `git branch` | Lista as branches (o asterisco denota a branch atual) |
| `git branch -a` | Lista todas as branches (local e remoto) |
| `git branch [nome da branch]` | Cria uma nova branch |
| `git branch -d [nome da branch]` | Deleta uma branch |
| `git push origin --delete [nome da branch]` | Deleta uma branch remota |
| `git checkout -b [nome da branch]` | Cria uma nova branch e muda para ela |
| `git checkout -b [nome da branch] origin/[nome da branch]` | Clona uma branch remota e muda para ela |
| `git checkout [nome da branch]` | Seleciona uma branch |
| `git checkout -` | Muda para a última branch |
| `git checkout -- [nome-arquivo.txt]` | Descarta modificações de um arquivo |
| `git merge [nome da branch]` | Faz um merge de uma branch na branch atual |
| `git merge [source branch] [branch alvo]` | Faz um merge de uma branch em outra branch |
| `git stash` | Tirar o estado sujo do seu diretório de trabalho |
| `git stash clear` | Remove todas as entradas 'stash' |

### Sharing & Updating Projects

| Comando | Descrição |
| ------- | --------- |
| `git push origin [nome da branch]` | Enviar uma branch para seu repositório remoto |
| `git push -u origin [nome da branch]` | Envia as alterações da branch informada para um repositório remoto (and selecionar a branch) |
| `git push` | Envia as alterações para o repositório remoto (branch atual) |
| `git push origin --delete [nome da branch]` | Deletar uma branch remota |
| `git pull` | Atualiza o repositório local para o último commit |
| `git pull origin [nome da branch]` | Recebe alterações do repositório remoto |
| `git remote add origin ssh://git@github.com/[usuario]/[nome-repositorio].git` | Adicionar um repositório remoto |
| `git remote set-url origin ssh://git@github.com/[usuario]/[nome-repositorio].git` | Seta um repositório da origin branch para o SSH |

### Inspeção & Comparação

| Comando | Descrição |
| ------- | --------- |
| `git log` | Ver modificações |
| `git log --summary` | Ver modificações (detalhadas) |
| `git diff [branch original] [branch alvo]` | Visualizar alterações antes de mesclar |

The default branch has been renamed!
main is now named master

If you have a local clone, you can update it by running the following commands.

| Comando | Descrição |
| ------- | --------- |
| `git branch -m main master` |
| `git fetch origin` |
| `git branch -u origin/master master` |
| `git remote set-head origin -a` |

## Comandos
Crédito: Matheus Battisti - Hora de Codar
https://www.youtube.com/watch?v=Zwv9qRyVeU4

| Comando | Descrição |
| `git init` | cria uma pasta escondida com o nome ".git", sem as aspas, e as configurações do git para o projeto |
| `git status` | Verifica os arquivos. |
| `git commit -a -m "Meu texto descritivo."` | Adiciona todo tipo de arquivo a esse commit; Escreve a mensagem com a descrição. |
| `-a` | Adiciona todo tipo de arquivo a esse commit. |
| `-m` | Adiciona uma mensagem a esse commit. |
| Ir no github.com/seuGithub | Para criar um repositório vazio. |
| Retornar para o terminal acessar a pasta do seu projeto | Para adicionar um repositório remoto. |
| `git remote add origin https://github.com/amimenezes/Git-Comandos.git` | Faz a conexão entre a pasta do PC e a pasta do Github. |
| `git branch -M main` | Afirma que o branch principal é o "main" |
| `git push -u origin main` | Envia o código atual da branch local para a branch do repositório remoto. |

O ideal é ter um branch para cada tarefa e cada dev trabalhar no seu branch. Depois uni-los em um forma coordenada e ordenada.

| `git checkout -b "teste"` | `-b` Cria a branch "teste" e, `checkout` muda da branch "main" para a branch "teste". |
Também tem que criar a branch no remoto (github.com/amimenezes/Git-Comandos).
| `git push --set-upstream origin teste` | Afirma que o branch principal é o "main" |
| `git commit -a -m "Nova tarefa."` | Adiciona todo tipo de arquivo a esse commit; Escreve a mensagem com a descrição. |
Depois de criado o branch no remoto, basta dar um `git push` para empurrar para o remoto os arquivos
| `git checkout main` | Pula para a branch main local. |
| `git branch` | Mostra a branch que está e todas as branchs criadas para o repositório. |
| `git merge teste` | Quando estiver na branch `main` e iserir esse comando, o `merge` irá unir o que tem na branch `main` com a branch `teste`. |
| `git push` | Pareia os códigos. |
| `git pull` | Pega todas as atualizações do remoto e põe no local. |
| `git clone https://github.com/amimenezes/Git-Comandos.git nomeDoPastaLocal` | Clona o repositório remoto e clona o projeto para uma pasta chamada `nomeDoPastaLocal`. |
| `git branch` | Verifica em qual branch está. |
| `git commit -a -m "Outra Demanda"` | ... |
| `git push` | ... |
Obs: quem clona sofre menos. ;)
| `git checkout teste` | Pula para a branch main local. |
| `git clearn -f` | Remove todos os arquivos adicionados com o `git add .`. |
| `git checkout .\index.html` | Última alteração não comitada será excluída do arquivo informado. |
| `git log` | Possui o tracker das mudanças realizadas, do mais recente para o mais antigo. |