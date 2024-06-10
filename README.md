# ComandosGit
## Verificar se existem arquivos modificados ou que não estejam em estado tracked.

git status

## Configurar um usuário no diretório local

 git config user.name "nome_da_pessoa"
 git config user.email "e-mail da pessoa"
 
## Configurar um usuário globalmente
 
 git config --global user.name "nome_da_pessoa" (sem aspas)
 git config --global user.email "e-mail da pessoa" (sem aspas)
 
## Inserir arquivo para ser monitorado
 
 git add "nome_do_arquivo"
 
## Realizar commit dos arquivos
 
 git commit -m "frase de identificação"
 
## Verificar log dos commits realizados
 
 git log
 
## Resumo dos commit
 
 git log --oneline
 
 ![GitLogOneline](https://github.com/WraSouza/ComandosGit/assets/15219047/630e036c-ad64-4a5d-85bc-a4f76e324ba8)

## Buscar Commits por Data
É possível buscar commits antes ou depois de uma determinada data

ANTES: 
git log --before="data_desejada"
Ex.: git log --before="2023-05-03"

DEPOIS: 
git log --after="data_desejada"
Ex.: git log --before="2023-05-03"
 
## Renomear nome do Arquivo pelo Git
 
 git mv nome_do_arquivo novo_nome_do_arquivo
 
 Obs.: Realizar a alteração pelo git já deixa o arquivo pronto para realizar o commit.
 
 Obs2.: É necessário realizar o commit depois de renomear o arquivo
 
## Deletar arquivo
 
 git rm nome_do_arquivo
 
 Obs.: É necessário realizar o commit depois de deletar o arquivo

## Alternando entre Commits

Você pode "viajar" entre os commits para verificar situação dos arquivos/pastas em um determinado commit. Para isso, basta digitar o seguite comando:

git checkout "hash_do_commit_desejado"

Na imagem abaixo, é possível visualizar o hash dos commits

 ![Screenshot_4](https://github.com/WraSouza/ComandosGit/assets/15219047/e6d1f00e-33e3-408b-b25c-55c6dff0e013)

 No momento atual, estamos no commit 796f282. Se desejarmos navegar para o commit f35f2a1, o comando é como mostrado na imagem abaixo.

 ![Screenshot_1](https://github.com/WraSouza/ComandosGit/assets/15219047/ebb845ac-2e10-44fa-bc5a-bd9df553355e)
 
## Verificar o que foi alterado
 
 git diff --staged
 
 Isso irá mostrar o que foi alterado quando o arquivo tiver sido commitado. Pode ajudar o desenvolvedor a ver o que tem de diferente antes de realizar o commit.
 Para verificar alterações antes do commit, basta digitar:

 git diff
 
## Verificar diferença entre o estado atual e um determinado commit
 
 git diff hash_id_do_commit_desejado

## Verificar diferença entre dois commits, que não seja o atual
 
 git diff hashid_commit_mais_antigo..hashid_commit_mais_novo
 
 ## Adicionar arquivos no último commit
 
 git commit --amend -m "frase_qualquer_de_identificação"

 ## Reverter Alterações
 git reset HEAD --hard

 Este comando fará com que todos os arquivos que tiveram modificações, retornem ao status do último commit.

 Obs.: Este comando deve ser utilizado com os arquivos antes da fase de staged.

 ## Revertendo Commits
 git reset HEAD^ --hard

 Depois de todos os arquivo serem comitados, digitando o comando, você irá retornar ao penúltimo commit.


