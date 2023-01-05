# MAC

```shell
brew install nvm
```



{% code title=".zshrc" %}
```shell
export NVM_DIR=~/.nvm
source $(brew --prefix nvm)/nvm.sh
```
{% endcode %}



nvm 을 통해 node 를 설치해 줍니다.

```shell
nvm install 16.16.0
nvm ls

nvm use 16.16.0
ln -s $(which node) /usr/local/bin/node
```
