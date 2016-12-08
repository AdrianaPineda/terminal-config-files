## Run
curl https://raw.githubusercontent.com/git/git/master/contrib/completion/git-completion.bash -o ~/.git-completion.bash

## Update .bash_profile
vim ~/.bash_profile

if [ -f ~/.git-completion.bash ]; then
  . ~/.git-completion.bash
fi

## Source
http://apple.stackexchange.com/questions/55875/git-auto-complete-for-branches-at-the-command-line
