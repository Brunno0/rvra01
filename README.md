
# React VR
React VR é uma biblioteca JavaScript para criar aplicações de realidade virtual (VR) e realidade aumentada (AR) baseadas em React.

## Instalação
Para instalar o React VR, você precisa ter o Node.js e o React Native CLI instalados em sua máquina. Depois, basta executar o seguinte comando no terminal:

npm install -g react-vr-cli

## Executando a primeira aplicação

Crie um novo projeto React VR usando o seguinte comando no terminal:

  react-vr init HelloWorld

Entre na pasta do projeto criado:

  cd HelloWorld

Execute o seguinte comando para iniciar o servidor de desenvolvimento:

  npm start

Acesse http://localhost:8081/vr/ em seu navegador para ver sua aplicacao rodando!

## Caso esbarre no erro: 

Error: invalid regular expression. React-rv 

https://stackoverflow.com/questions/75270065/error-invalid-regular-expression-react-rv 


Fala galera, não sei postar soluções mas encontrei esse erro ao instalar o react-rv. Após alguams buscas, encontrei a solução aqui no stack. Porém, em um caminho(path) diferente do comum. 

Invalid regular expression: /(node_modules[\\\]react[\\\]dist[\\\].*|website\\node_modules\\.*|heapCapture\\bundle\.js|.*\\__tests__\\.*)$/: Unterminated character class

Vá no arquivo: 
...\node_modules\metro-bundler\src\blacklist.js

e substitua o REGEX sharedBlackList por: 

var sharedBlacklist = [/node_modules[\/\\]react[\/\\]dist[\/\\].*/,/website\/node_modules\/.*/,/heapCapture\/bundle\.js/,/.*\/__tests__\/.*/]

Como não encontrei a solução por aí, resolver tentar postar aqui. :D 







