# react-webpack-ts-boilerplate

## Steps to create a starter with react webpack and typescript

1. Initialize the repository

   - git init
   - create .ignore file

2. Create two folders

   - src
   - build

3. Initialize the package.json file in the root directory

   - npm init --y
   - create index.html in src folder

4. Create index.html in the src folder

5. add dependencies - react react-dom

   - yarn/npm add react react-dom

6. install typescript and types for react and react-dom as dev dependencies

   - yarn/npm add -D typescript @types/react @types/react-dom

7. configuration for typescript compiler

   - create tsconfig.json

8. set-up root component of application

   - in src folder create App.tsx

9. Install babel with necessary plugs as dev dependencies

   - yarn/npm add -D@babel/core @babel/preset-env @babel/preset-react @babel/preset-typescript
   - create file .babelrc and add presets and plugins

10. Install webpack related packages as dev dependencies (make use of webpack which is module bundler)

    - yarn/npm add -D webpack webpack-cli webpack-dev-server html-webpack-plugin

    - we also need babel loader package which allows transpiling JavaScript file using babel and webpack.
    - run the following command
    - yarn/npm add -D babel-loader

11. Webpack configuration

    - create webpack folder
    - webpack.config.js

12. add npm script to run our application
    - in package.json add the following in "scripts"
    - "start": "webpack serve --config webpack/webpack.config.js --open",
    - run application with 'yarn start' or 'npm start'

fix error:

- Install the missing Babel plugin
- npm install --save-dev @babel/plugin-transform-runtime

13. add npm script to run our application

- css-loader & style-loader to process the style file and instruct webpack to use them for all css files

```bash
yarn add -D css-loader style-loader
npm install --save-dev css-loader style-loader
```

14. Add a type declaration for images

- create global.d.ts file
