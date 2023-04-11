# Module bundlers example

Followed along "Module Bundlers explained" video: https://www.youtube.com/watch?v=5IG4UmULyoA

1. Initiate the project
   npm init -y
   npm i lodash

2. try to open in Browser
   src/index.js
   Use lodash and open public/index.html in browser. Wont print Hello World to the Console.

3. Fix with webpack
   npm install --save-dev webpack webpack-cli
   npm run build
   dist/main.js will contain the bundled file.
   open public/index.html in browser. Will print helloWorld to the Console.

4. Config Webpack with loaders
   create style.scss
   import from index.js
   configure loaders with npm install --save-dev css-loader style-loader sass-loader
   add module rules in webpack config
   npm install sass

5. Plugins
   npm install --save-dev webpack-bundle-analyzer
   add plugins in webpack config

6. Dev server
   npm install --save-dev webpack-dev-server
   add dev server config to webpack
   npm run dev
