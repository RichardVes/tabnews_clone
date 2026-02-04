# Git Estudos

    Os arquivos podem estar entre 3 tipos de estatus
        .Modified
        Arquivos modificados, com novas alterações
        .Staged
        Estão em uma área de preparo, coloca em evidencia os que vao ser comitados
        .Commit
        Arquivos

# Como remover um arquivo do stage após git add (antes do commit)

    Se você adicionou arquivos ao stage por engano, não tem problema, você pode tirar o que quiser do palco antes de fazer o commit, executando o comando:
    git restore --staged nome-do-arquivo.js
    Isso remove o arquivo do stage (palco), mas mantém as alterações no seu arquivo local.

# Como alterar um commit que não é o último (mais antigo)?

    É possível sim, mas não apenas com o --amend sozinho. Seria preciso utilizá-lo em conjunto com outro comando, que é o git rebase. O git rebase é uma espécie de amend turbinado.
    Mais para frente o Filipe vai ensinar como fazer ele em detalhes, mas resumidamente o processo seria:
    Iniciar o rebase interativo: git rebase -i HEAD~N (onde N é o número de commits que você quer visualizar)
    No editor, marcar o commit desejado como edit
    Fazer as alterações necessárias
    Executar git commit --amend
    Finalizar com git rebase --continue

# Como remover um arquivo do stage após git add (antes do commit)

    Se você adicionou arquivos ao stage por engano, não tem problema, você pode tirar o que quiser do palco antes de fazer o commit, executando o comando:
    git restore --staged nome-do-arquivo.js
    Isso remove o arquivo do stage (palco), mas mantém as alterações no seu arquivo local.
    Quando você digita git status, o próprio Git mostra o comando para realizar esta ação.

# Existe uma alternativa mais segura ao --force?

    Sim! Uma opção seria usar o git push --force-with-lease, que é a forma "segura" de forçar o push, pois só sobrescreve o remoto se a sua cópia local estiver atualizada. Ou seja, ele evita apagar commits que outros possam ter enviado para o remoto.
    Outra alternativa é resolver o conflito localmente usando git pull e depois enviar normalmente para o GitHub. Apesar de "poluir" um pouco o histórico com um commit de resolução de conflito, é uma opção válida. 🤝

# Quando usar amend vs criar um novo commit para corrigir erros?

    Depende do cenário. Criar um novo commit corrigindo seria menos "destrutivo". A vantagem do amend é que o histórico dos commits fica mais limpo, mas ele deve ser aplicado com cautela.
    Quando é uma alteração muito simples e você está trabalhando sozinho (como no caso desta aula), vale a pena usar o amend. Num contexto colaborativo, principalmente se tratando da branch main, e dependendo da complexidade da alteração, um novo commit pode ser mais adequado.
