# Arquivos de anotações

nvm = Node Version Manager
para usar a mesma versão trocamos a versão padrao pelo comando **nvm alias default\*\***lts/hydrogen\*\*

- nvm é o comando
- alias é o apelido
- default é o padrão
- lts/hydrogen é a versão escolhida

## Criando o arquivo .nvmrc

    rc significa **run commands** ou comendo de carregamendo, são comandos que serão usados ao chamar o nvm , como por exemplo se eu usar o comando install nvm, agora irá escolher a versão que eu colocar dentro desse arquivo. ""lts/hydrogen""

# Manifesto "package.json "

    arquivo que serve para colocar as versões das tecnologias usadas no projeto
        - **npm init**        para criar esse arquivo

Site do framework: https://nextjs.org/
Site da empresa por trás: https://vercel.com/

# criando servidor na nuvem

    Criamos dentro do arquivo package.json, um script dentro de  "scripts" chamado
        "dev": "next dev"
        serve para criar o arquivo na nuvem
