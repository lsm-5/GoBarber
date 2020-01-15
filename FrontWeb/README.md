# Passo a passo

### yarn create react-app <nome>

### yarn add eslint -D

### yarn eslint --init

### remove package-lock.json

### yarn

### yarn prettier eslint-config-prettier eslint-plugin-prettier babel-eslint -D

### config eslintrc

module.exports = {
env: {
es6: true,
jest: true,
browser: true
},
extends: ["airbnb", "prettier", "prettier/react"],
globals: {
Atomics: "readonly",
SharedArrayBuffer: "readonly",
**DEV**: true
},
parserOptions: {
ecmaFeatures: {
jsx: true
},
ecmaVersion: 2018,
sourceType: "module"
},
plugins: ["react", "jsx-a11y", "import", "react-hooks", "prettier"],
rules: {
"prettier/prettier": "error",
"react/jsx-filename-extension": ["error", { extensions: [".js", ".jsx"] }],
"import/prefer-default-export": "off",
"no-unused-vars": ["error", { argsIgnorePattern: "^_" }],
"react/jsx-one-expression-per-line": "off",
"global-require": "off",
"react-native/no-raw-text": "off",
"no-param-reassign": "off",
"no-underscore-dangle": "off",
camelcase: "off",
"no-console": ["error", { allow: ["tron"] }],
"react-hooks/rules-of-hooks": "error",
"react-hooks/exhaustive-deps": "warn"
},
settings: {
"import/resolver": {
"babel-plugin-root-import": {
rootPathSuffix: "src"
},
},
},
};

### config .prettierrc

{
"singleQuote": true,
"trailingComma": "es5"
}
