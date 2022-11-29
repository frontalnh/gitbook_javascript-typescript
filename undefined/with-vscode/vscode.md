# VSCode 설정하기

제일 먼저 prettier 와 eslint 를 사용하기 위해 플러그인을 설치해줍니다.

VSCode 의 Extensions: Marketplace 로 들어가 ESLint 와 Prettier 를 검색하여 설치해줍니다.



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
