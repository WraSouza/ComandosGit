# ComandosGit
## Verificar se existem arquivos modificados ou que não estejam em estado tracked.

git status

## Configurar um usuário no diretório local

 git config user.name "nome_da_pessoa"
 git config user.email "e-mail da pessoa"
 
## Configurar um usuário globalmente
 
 git config --global user.name "nome_da_pessoa" (sem aspas)
 git config --global user.email "e-mail da pessoa" (sem aspas)
 
# Inserir arquivo para ser monitorado
 
 git add "nome_do_arquivo"
 
 # Realizar commit dos arquivos
 
 git commit -m "frase de identificação"
 
# Verificar log dos commits realizados
 
 git log
 
 # Resumo dos commit
 
 git log --oneline
 
 # Renomear nome do Arquivo pelo Git
 
 git mv nome_do_arquivo novo_nome_do_arquivo
 
 Obs.: Realizar a alteração pelo git já deixa o arquivo pronto para realizar o commit.
 
 Obs2.: É necessário realizar o commit depois de renomear o arquivo
 
 # Deletar arquivo
 
 git rm nome_do_arquivo
 
 Obs.: É necessário realizar o commit depois de deletar o arquivo
 
 # Verificar o que foi alterado
 
 git diff --staged
 
 *Isso irá mostrar o que foi alterado antes de ser commitado. Pode ajudar o desenvolvedor a ver o que tem de diferente antes de realizar o commit.
 
 # Verificar diferença entre o estado atual e um determinado commit
 
 git diff hash_id_do_commit_desejado
 
 # Verificar diferença entre dois commits, que não seja o atual
 
 git diff hashid_commit_mais_antigo..hashid_commit_mais_novo


