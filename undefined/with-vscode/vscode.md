# VSCode 설정하기

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
