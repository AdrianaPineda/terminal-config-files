## PS1
Update .bash_profile
```
export PS1="\A\[$(tput sgr0)\] \w\[\033[38;5;5m\]\$(parse_git_branch)\[\033[00m\] $ "
```
