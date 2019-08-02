# create-react-webpack

Create React Application with all standard practices, with easy formats known to users, so that users can easily modify the various config files.

## Creating an App

### npm

```
npm create-react-webpack demo-app
```

it will create a directory `demo-app` in the current folder, with below file footprint.

```
demo-app
├── README.md
├── node_modules
├── package.json
├── .gitignore
├── .babelrc
├── .eslintrc.json
├── .eslintignore
├── .prettierrc
├── .prettierignore
├── public
│   ├── favicon.ico
│   ├── index.html
│   └── manifest.json
└── src
│   ├── App.css
│   ├── App.js
│   ├── App.spec.js
│   └── index.js
├── webpack.config.base.js
├── webpack.config.dev.js
└── webpack.config.prod.js
```

## Available Scripts

After creating project directory you can run following scripts:-

### `npm run build`

builds the application for production to the `dist` folder inside directory.<br>
Uses webpack `prod` `config` along with `base` `config`

### `npm run dev`

Start the development server on default port `8080`.<br>
Starts server in hot mode but doesn't preserve state of component if any while reloading.

### `npm run dev:hot`

Start the development server on default port `8080`.<br>
Starts server in hot mode preserves state of component also if any while applying hot load patch.

### `npm test`

Launches Test Runner in the intreactive manner.

### `npm run format`

Enforces the formatting rules defined in `.prettierrc`.<br>
For inforcing your rules `replace` the `file` or `content` of `prettierrc`.

### `npm run lint`

Enforces the linting rules defined in `.eslintrc`.
<br>
For inforcing your rules `replace` the `file` or `content` of `eslintrc`.<br>
Here we are using `prettier` for formatting and `eslint` for enforcing rules related to best coding practices.