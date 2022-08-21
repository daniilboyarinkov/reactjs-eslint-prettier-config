# My React .vscode configuration

    📝 Everything happens inside .vscode folder

## extension.json

```js
{
    "recommendations": [
        // en words spell checker
        "streetsidesoftware.code-spell-checker",
        // ru words spell checker
        "streetsidesoftware.code-spell-checker-russian",
        "dsznajder.es7-react-js-snippets",
        "dbaeumer.vscode-eslint",
        "esbenp.prettier-vscode",
        "hex-ci.stylelint-plus",
        "mikestead.dotenv"
    ],
    
    "unwantedRecommendations": []
}
```

## settings.json

```js 
{
    // default alt+shift+F formater
  "editor.defaultFormatter": "esbenp.prettier-vscode",

    // Format code on ctrl+S
  "editor.formatOnSave": true,
  
    // Langs for cSpell extension
  "cSpell.language": "en,ru",

    // Использование локальных правил Stylelint
  "stylelint.useLocal": true,
    // Форматирование при сохранении файла
  "stylelint.autoFixOnSave": true,

    // custom keywords highlighting
  "todohighlight.keywords": [
    {
      "text": "TODO:",
      "color": "white",
      "border": "1px solid white",
      "backgroundColor": "#808080"
    },
    
    // Fira code to improve code readability
  "editor.fontFamily": "Fira Code",
  "editor.fontLigatures": true,

    // vs code prompts on 
  "javascript.inlayHints.enumMemberValues.enabled": true,
  "javascript.inlayHints.functionLikeReturnTypes.enabled": true,
  "javascript.inlayHints.parameterNames.enabled": "all",
  "javascript.inlayHints.parameterTypes.enabled": true,
  "javascript.inlayHints.propertyDeclarationTypes.enabled": true,
  "javascript.inlayHints.variableTypes.enabled": true,
  "typescript.inlayHints.enumMemberValues.enabled": true,
  "typescript.inlayHints.parameterTypes.enabled": true,
  "typescript.inlayHints.propertyDeclarationTypes.enabled": true,

  // Превью предложения
  "editor.suggest.preview": true
  ],
}
```
