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
    }
  ],
}
```
