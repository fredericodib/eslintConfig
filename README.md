# eslintConfig

### Instalar

```
yarn add eslint -D
```

```
yarn add prettier eslint-config-prettier eslint-plugin-prettier babel-eslint -D
```

```
yarn eslint --init
```

### Responder da seguinte maneira para React:
- To check syntax, find problems, and enforce code style
- JavaScript modules (import/export)
- React
- Sua escolha
- Browser
- Use a popular style guide
- AirBnb
- JavaScript

#### .eslintrc.js
```
module.exports = {
  env: {
    browser: true,
    es2021: true,
  },
  extends: ['plugin:react/recommended', 'airbnb', 'prettier'],
  parser: 'babel-eslint',
  parserOptions: {
    ecmaFeatures: {
      jsx: true,
    },
    ecmaVersion: 12,
    sourceType: 'module',
  },
  plugins: ['react', 'prettier'],
  rules: {
    'prettier/prettier': 1,
    'react/state-in-constructor': 0,
  },
};
```

#### .prettierrc.json
```
{
  "tabWidth": 2,
  "singleQuote": true,
  "jsxSingleQuote": true
}
```
