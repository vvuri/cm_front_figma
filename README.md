# cm_front_figma
Course frontend 2023

## FrontEnd course CSS 
Home Work 6 - Figma

## Buid env
- staging: ``` $ npm run dev ```
- production: ``` $ npm run build ```
- local development: ``` $ npm run serve ```

## Steps
1. Create new repository on github
2. ``` $ npm init ```
3. ``` $ npm i -D webpack webpack-cli ```
4. Configure package.json, add ```"dev": "webpack --mode development",```
5. Run ``` $ npm run dev``` -> /dev/main.js
6. Add plugin ``` $ npm i -D html-webpack-plugin ```
7. Create webpack.config.js with copy index.html to /dist
8. Add local web server ``` $ npm install -D webpack-dev-server ```
9. In package.json add  "serve": "webpack serve --open --mode development"
10. No need add file serve.config.js '--config dev/serve.config.js'
11. Run ``` $ npm run serve ``` -> open http://localhost:8080/
12. Do not auto reboot page after save
13. Add 'devServer' param in webpack.config.js -> autoreboot page http://localhost:9000
14. Add entry point in webpack.config.js -> ``` $ npm run dev ``` -> /dist/index.2a807a189b9b51451290.js  
15. Clear /dist ``` $ npm i -D filemanager-webpack-plugin ``` + FileManagerPlugin in config
16. Create production script "build": "webpack --mode production" -> ``` $ npm run build ```
17. Babel: [Can I use](https://caniuse.com/) 
18. ``` $ npm i -D @babel/core @babel/preset-env babel-loader ```
19. Create config .babelrc and add in webpack.config.js
20. Support SCSS: ``` $ npm i -D sass-loader postcss-loader postcss-preset-env css-loader style-loader sass ```
21. Extract CSS from JS ``` $ npm i -D mini-css-extract-plugin ``` 
22. Add module.rules for SCSS in webpack.config.js
23. Add postcss.config.js for support old browsers -> ``` $ npm run serve ``` 
24. Add "import './main.scss';" in src/index.js -> ``` $ npm run build ```
25. For images use Asset Modules webpack module and in html ```<img src=<%=require("./images/logo.svg")%> alt="logo">```

## Documentation
- [Habr step by step](https://habr.com/ru/articles/701724/)
- [Material RUS](https://gruzdevv.ru/stati/materialnyj-dizajn-spetsifikatsii-google/)
- [Material](https://m3.material.io/develop/android/jetpack-compose) 
- [CSS](https://www.w3schools.com/css/default.asp)
- [SASS](https://sass-lang.com/)
- [mdn: grid](https://developer.mozilla.org/en-US/docs/Web/CSS/grid)
- [БЭМ](https://ru.bem.info/methodology/)
- [Matirial Navigation](https://m3.material.io/components/navigation-drawer/specs)