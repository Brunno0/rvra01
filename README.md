
# React VR
React VR é uma biblioteca JavaScript de código aberto desenvolvida pelo Facebook para criar aplicações de realidade virtual (VR) e realidade aumentada (AR) baseadas em React.

Com o React VR, é possível criar aplicativos em VR que funcionam em diversas plataformas, como dispositivos móveis e desktops. Ele utiliza o WebGL para renderizar gráficos em 3D, e fornece um conjunto de componentes que permitem criar ambientes interativos em 360 graus, bem como integrar elementos 2D na cena. Além disso, podemos combar como WebVR e A-Frame, para aprimorar ainda mais as experiências em VR.

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

Invalid regular expression: /(node_modules[\\\]react[\\\]dist[\\\].*|website\\node_modules\\.*|heapCapture\\bundle\.js|.*\\__tests__\\.*)$/: Unterminated character class

Vá no arquivo: 
...\node_modules\metro-bundler\src\blacklist.js

e substitua o REGEX sharedBlackList por: 

var sharedBlacklist = [/node_modules[\/\\]react[\/\\]dist[\/\\].*/,/website\/node_modules\/.*/,/heapCapture\/bundle\.js/,/.*\/__tests__\/.*/]









