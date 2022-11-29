# MAC

```shell
brew install nvm
```



{% code title=".zshrc" %}
```shell
export NVM_DIR=~/.nvm
source $(brew --prefix nvm)/nvm.sh
nvm install 16.16.0
nvm ls
nvm use 16.16.0
ln -s $(which node) /usr/local/bin/node
```
{% endcode %}
