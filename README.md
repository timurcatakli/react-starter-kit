## React Starter Kit

It might be boring to configure `.babelrc`, `package.json` and rest of the React files everytime you start a new project. So here is a starter kit for you, especially for beginners. 

Here are the steps 


1- ```npm init```

2- ```npm install --save react react-dom && npm install --save-dev html-webpack-plugin webpack webpack-dev-server babel-{core,loader} babel-preset-react```

Use `--save` lets you seperate dev dependencies. `{core, loader}` means install them both

Webpack will take `index.js` file under app and will compile and move it under `dist/` folder with the name `index_bundle.js`

7- Next we created `.babelrc` file and configured Babel

8- In `package.json` file we have the following code
```
"scripts": {
    "start": "webpack-dev-server",
    "prod": "webpack -p"
 },
```
These are the shortcuts for webpack. You will use them as follows in the terminal

To bundle and transform the jsx, js and html files manually.
```
$ npm run start
```

Best approach is to run webpack server using the command below...
```
$ npm run prod
```
