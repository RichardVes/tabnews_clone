Como alterar um commit que não é o último (mais antigo)?

É possível sim, mas não apenas com o --amend sozinho. Seria preciso utilizá-lo em conjunto com outro comando, que é o git rebase. O git rebase é uma espécie de amend turbinado.

Mais para frente o Filipe vai ensinar como fazer ele em detalhes, mas resumidamente o processo seria:

Iniciar o rebase interativo: git rebase -i HEAD~N (onde N é o número de commits que você quer visualizar)
No editor, marcar o commit desejado como edit
Fazer as alterações necessárias
Executar git commit --amend
Finalizar com git rebase --continue
