# ESLint 설정하기

* `eslint`: ESLint core library
* `@typescript-eslint/parser`: parser that allows ESLint to understand TypeScript code
* `@typescript-eslint/eslint-plugin`: plugin with a set of recommended TypeScript rules

```bash
yarn add --dev eslint@7.11.0 # for react version
yarn add --dev --save-exac prettier
yarn add --dev eslint-plugin-prettier eslint-config-prettier
yarn add --dev eslint @typescript-eslint/parser @typescript-eslint/eslint-plugin
```



{% code title=".eslintrc" %}
```json
{
    "parser": "@typescript-eslint",
    "extends": [
        "eslint:recommended",
        "plugin:prettier/recommended",
        "plugin:@typescript-eslint/recommended"
    ],
  "rules": {
		"prettier/prettier": "error",
    "@typescript-eslint/ban-ts-comment": "warn",
    "object-curly-newline": ["off"],
    "function-paren-newline": ["off"],
    "react/display-name": ["off"],
    "no-constant-condition": "warn",
    "react-hooks/rules-of-hooks": "warn",
    "no-empty-pattern": "warn",
    "no-undef": "warn",
    "no-redeclare": "warn",
    "react/jsx-key": "warn",
    "no-unused-vars": "off",
    "@typescript-eslint/prefer-as-const": "warn",
    "@typescript-eslint/no-empty-function": "warn",
    "@typescript-eslint/no-empty-interface": "warn",
    "no-var": "warn"
  }
}
```
{% endcode %}

``

`tsc --noemit` 으로 타입 체크 먼저 해줌



{% code title="package.json" %}
```json
{
    "scripts":{
        "lint": "tsc --noemit && next lint"
    }
}
```
{% endcode %}

