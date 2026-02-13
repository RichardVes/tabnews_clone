# Estudos sobre Packge.json

    Arquivo
    "dependencies": {
    "next": "^13.1.6",
    "react": "^18.2.0",
    "react-dom": "^18.2.0"
    },
    "devDependencies": {
    "prettier": "^3.8.1"
    }

# Para instalar alguma coisa no npm

    npm install prettier --save-dev

# Diferença de "dependencies" e "devDependencies"

- dependencies
  - Motra todas as dependencias para o projeto funciar.

- devDependencies
  - Mostra dependencias extras não necessarias para o projeto funcionar,
  - São dependencias do desenvolvedor que ele usa na maquina dele e de todos do projeto

---

---

# Scripts

    "dev": "next dev",
      Cria um servidor local e roda o projeto localmente.
    "lint:check":"prettier --check ."
      Verifica se os arquivos estão formatados
