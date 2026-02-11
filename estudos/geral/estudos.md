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
    -**npm instal** instala essas dependencias
    Site do framework: https://nextjs.org/
    Site da empresa por trás: https://vercel.com/

# criando servidor na nuvem

    Criamos dentro do arquivo package.json, um script dentro de  "scripts" chamado
        "dev": "next dev"
        serve para criar o arquivo na nuvem

# Por que precisamos commitar o package-lock.json se ele é gerado automaticamente?

    Para entender a importância de enviar o package-lock.json para o repositório remoto, é preciso esclarecer qual é o seu papel e qual é a diferença dele para o package.json.
    A pista está na palavra "lock", que significa "trava". O package-lock.json é uma versão "travada" do seu irmão, no que diz respeito à lista de dependências.
    Mesmo instalando versões específicas de pacotes, o package.json ainda permite uma certa flexibilidade quando o comando npm install for executado para instalar as mesmas dependências do zero. Isso será explicado em detalhes quando o Filipe abordar o conceito de Versionamento Semântico.
    Enquanto o ambiente de desenvolvimento permite essa flexibilidade, o mesmo não pode ser dito para outros ambientes como o de produção. Nesses ambientes, a flexibilidade para instalação de pacotes com pequenas atualizações pode levar a comportamentos inesperados e bugs.
    O package-lock.json fornece uma versão fixa de todas as dependências e sub-dependências, para que em ambientes onde erros não podem ser tolerados, não tenhamos surpresas. Por isso também é importante mantê-lo no repositório remoto.
    Se isso ainda não ficou 100% claro, não se preocupe. À medida que você progredir no curso, isso vai melhorar, e o Filipe mais para frente vai se aprofundar nesse assunto.

# Tipos de Modelos

    Organico e Impressora 3d
        Na programação Orgânica as funcionalidades do programa vão sendo adicionadas uma a uma, conforme a necessidade vai surgindo. E as próprias funcionalidades não são adicionadas de modo 100% pronto, mas vão sendo melhoradas gradualmente também. É entregar o mínimo necessário.

    Na já no modo Impressora 3D busca-se entregar todas as funcionalidades do programa 100% prontas e de uma vez. Ou seja, é tudo ou nada. O projeto só é entregue quando todas as features que imaginamos que ele deve ter estão funcionando.

    O modelo Impressora 3D acaba travando a gente em muitos casos, enquanto desenvolver de forma orgânica é uma experiência bem menos estressante e ajuda a destravar o desenvolvimento dos projetos, dando um passo de cada vez.
