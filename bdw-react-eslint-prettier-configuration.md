# React Eslint-Prettier Configuration

[eslint]: https://github.com/daniilboyarinkov/reactjs-eslint-prettier-config/bdw-react-eslint-prettier-configuration.md#Eslint
[prettier]: https://github.com/daniilboyarinkov/reactjs-eslint-prettier-config/bdw-react-eslint-prettier-configuration.md#Prettier
[stylelint]: ./bdw-react-stylelint-purecss-configuration.md
[vscode]: ./bdw-react-vscode-eslint-configuration.md

## Content:
+ [Eslint][eslint]
+ [Prettier][prettier]
+ [Stylelint][stylelint]
+ [.vscode][vscode]

## Eslint

Everything here is for yarn pm.

```shell
yarn create react-app <project-name>
```

### Initializing an eslint locally for project

```shell
yarn run eslint --init
```

### React 

[eslint-plugin-react](https://www.npmjs.com/package/eslint-plugin-react)

- [x] Required

```shell
yarn add eslint-plugin-react -D  
```

### React Hooks

[eslint-plugin-react-hooks](https://www.npmjs.com/package/eslint-plugin-react-hooks)

From React Documentation:

>Only Call Hooks at the Top Level
>Don’t call Hooks inside loops, conditions, or nested functions.   
>Instead, always use Hooks at the top level of your React function, before any early returns.
>
>Don’t call Hooks from regular JavaScript functions. Instead, you can:
>
> - ✅ Call Hooks from React function components.
> - ✅ Call Hooks from custom Hooks
>  
> ...
> 
> This plugin is included by default in Create React App.

- [ ] Optional

```shell
yarn add eslint-plugin-react-hooks -D
```

### JSX accessibility rules

- [x] Required

[eslint-plugin-jsx-a11y](https://www.npmjs.com/package/eslint-plugin-jsx-a11y)

```shell
yarn add eslint-plugin-jsx-a11y -D 
```

###

[eslint-plugin-import](https://www.npmjs.com/package/eslint-plugin-import)

From Documentation: 

> This plugin intends to support linting of ES2015+ (ES6+) import/export syntax, 
> and prevent issues with misspelling of file paths and import names. 
> 
> All the goodness that the ES2015+ static module syntax intends to provide, 
> marked up in your editor.

- [x] Required

```shell
yarn add eslint-plugin-import -D  //  plugin:import/recommended
```
Ignoring things you don't need...

```shell
echo .prettierrc.json *.html > .eslintignore 
```

## .eslintrc.json 

### extends: 

```js
"extends": [
        "eslint:recommended",
        "plugin:react/recommended",
        "plugin:react/jsx-runtime",
        "plugin:react-hooks/recommended",
        "plugin:jsx-a11y/recommended",
        "plugin:import/recommended",
        "airbnb",
        "prettier"
    ],
```

### plugins

```js
"plugins": [
        "react",
        "prettier",
        "jsx-a11y"
    ],
```

### rules

```js
"rules": {
    "react/jsx-filename-extension": [1, { "extensions": [".js", ".jsx"] }],
    "prettier/prettier": [
        "error",
        {
          "endOfLine": "auto"
        }
      ],
    "import/order": [
        2,
        {
          "groups": ["external", "builtin", "index", "sibling", "parent", "internal", "type"],
          "alphabetize": {
            "order": "asc",
            "caseInsensitive": true
          },
          "newlines-between": "always-and-inside-groups"
        }
      ]
}
```

## Prettier

```shell
yarn add prettier -D -E
```

### Eslint config Prettier

[eslint-config-prettier](https://github.com/prettier/eslint-config-prettier)

From Documentation: 

> Turns off all rules that are unnecessary or might conflict with Prettier.
>
> This lets you use your favorite shareable config without letting its 
> stylistic choices get in the way when using Prettier.

```shell
yarn add -D eslint-config-prettier 
```

Ignoring things you don't need...

```shell
echo .eslintrc.json > .prettierignore 
```

## .prettierrc.json

```js
{
  "semi": false,
  "endOfLine": "auto"
}
```

# Airbnb для Eslint

```shell
yarn add eslint-config-airbnb -D
```

## StyleLint

[Using pure CSS? Here is standard stylelint config...](./bdw-react-stylelint-purecss-configuration.md)

## VS code configuration

[Using VS code editor? Here is my .vscode config...](./bdw-react-vscode-eslint-configuration.md)
