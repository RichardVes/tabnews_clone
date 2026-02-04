# Lista de comandos abordados

    git log - listar os commits do repositório.
    git add - sobe alterações para a staging area.
    git commit - realiza novos commits.
    git commit --amend - substitui o commit anterior por um novo, mas aproveita as alterações dele.
    git diff - calcula a diferença entre as versões/alterações dos arquivos.

Os arquivos podem estar entre 3 tipos de estatus
.Modified
Arquivos modificados, com novas alterações
.Staged
Estão em uma área de preparo, coloca em evidencia os que vao ser comitados
.Commit
Arquivos

# COMANDOS GIT

> git status

    mostra o status dos arquivos

> git log
> git log --stat

    Compara os arquivos do git com os local.

> git log --stat

    Mostra os estatus dos commits

> git log --oneline

    mostra todos os status em 1 linha (resumido)

> git diff

    mostra a diferença do que tem no servidor .git e o que tem local

> git commit --amend

Como remover um arquivo do stage após git add (antes do commit)

Se você adicionou arquivos ao stage por engano, não tem problema, você pode tirar o que quiser do palco antes de fazer o commit, executando o comando:

git restore --staged nome-do-arquivo.js

Isso remove o arquivo do stage (palco), mas mantém as alterações no seu arquivo local.
