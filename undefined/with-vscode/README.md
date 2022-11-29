# 린터 설정하기 (with vscode)

{% code title="package.json" %}
```json
{
    "scripts":{
        "lint": "tsc --noemit && next lint"
    }
}
```
{% endcode %}



### VScode 설정

{% code title=".vscode/settings.json" %}
```json
{
  // Set the default
  "editor.formatOnSave": false,
  // Enable per-language
  "[javascript]": {
    "editor.formatOnSave": true
  },
  "editor.codeActionsOnSave": {
    // For ESLint
    "source.fixAll.eslint": true
  },
	"eslint.validate": ["javascript", "javascriptreact", "typescript", "typescriptreact"],
	"eslint.format.enable": true
}
```
{% endcode %}

