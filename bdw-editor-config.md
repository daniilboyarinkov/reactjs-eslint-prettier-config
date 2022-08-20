# My EditorConfig configuration for projects

## .editorconfig

```ini
root = true

[{*js, *jsx, *ts, *tsx}]
indent_style = space
indent_size = 2
tab_width = 2
end_of_line = lf

[*.min.*]
indent_style = ignore
trim_trailing_whitespace = false
insert_final_newline = ignore
```

## .vscode

### extension.json

```js
{
    "recommendations": [
        ...,
        EditorConfig.EditorConfig
    ],
}
```
