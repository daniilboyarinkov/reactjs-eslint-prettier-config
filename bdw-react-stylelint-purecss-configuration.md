# React StyleLint Pure CSS configuration

```shell
yarn add -D stylelint
```

## Standard config

[stylelint-config-standard](https://www.npmjs.com/package/stylelint-config-standard)

From documentation: 

> Turns on additional rules to enforce common conventions 
> found in the specifications and in a handful of CSS styleguides, 
> including: The Idiomatic CSS Principles, Google's CSS Style Guide, 
> Airbnb's Styleguide, and @mdo's Code Guide.

```shell
yarn add -D stylelint-config-standard
```

## Clean Order

| Before                                                                                                           | After                                                                                                           |
| ---------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------- |
| ![before](https://user-images.githubusercontent.com/10108377/173256557-88f5098b-dad7-4339-a571-6850ed82828f.png) | ![after](https://user-images.githubusercontent.com/10108377/173256556-e29e892a-2d21-437c-8093-a345d5de920e.png) |

[stylelint-config-clean-order](https://github.com/kutsan/stylelint-config-clean-order)

```shell
yarn add -D stylelint-config-clean-order
```

## .stylelintrc

```js 
{
  "extends": ["stylelint-config-standard", "stylelint-config-clean-order", "stylelint-config-prettier"],
  "plugins": ["stylelint-order"],
  "rules": {
    "no-empty-source": null,
    "declaration-empty-line-before": null,
    "no-missing-end-of-source-newline": null,
    "selector-class-pattern": null,
    "keyframes-name-pattern": null
  }
}
```

## .stylelintignore

Ignore things you don't need...

```txt
*.tsx
*.jsx
*.ts
*.js
*.md
*.svg
*.html
/node_modules
```
