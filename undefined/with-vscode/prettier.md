# Prettier 설정하기

### Prettier 란?

Prettier는 기존의 코드에 적용되어있던 스타일들을 전부 무시하고, 정해진 규칙에 따라 자동으로 코드 스타일을 정리해 주는 코드 포멧터이다.

ESLint와 다른점이라면 ESLint는 문법 에러를 잡아내고, 특정 문법 요소를 쓰도록 만드는 등 코드 퀄리티와 관련된 것을 고치기 위해 사용되지만 Prettier는 코드 한 줄의 최대 길이나, 탭의 길이는 몇으로 할 것인지, 따옴표는 홀따옴표(')나 쌍따옴표(")중 무엇을 사용 할 것인지 등등 코드 퀄리티보단 코딩 스타일을 일괄적으로 통일하는 도구에 가깝다.



{% code title=".prettierrc" %}
```json
{
  "singleAttributePerLine": false,
  "printWidth": 120,
  "tabWidth": 2,
  "jsxBracketSameLine": true,
  "singleQuote": true,
  "trailingComma": "all",
  "semi": true,
  "useTabs": false,
  "bracketSpacing": true,
  "jsxSingleQuote": true
}
```
{% endcode %}

