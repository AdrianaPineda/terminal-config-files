## 1. Homebrew
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

## 2. NVM
https://gist.github.com/nijicha/e5615548181676873118df79953cb709
```
1) brew install nvm

2) mkdir ~/.nvm

3) In bash_profile:
    # NVM
    export NVM_DIR=~/.nvm
    source $(brew --prefix nvm)/nvm.sh

4) source ~/.bash_profile

5) nvm install node

6) nvm ls

7) nvm use x.y.z
```