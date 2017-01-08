# Update .bash_profile

## Git branch in prompt.
```
parse_git_branch() {
    git branch 2> /dev/null | sed -e '/^[^*]/d' -e 's/* \(.*\)/ (\1)/'
}
```

## PS1
export PS1="\A\[$(tput sgr0)\] \w\[\033[38;5;5m\]\$(parse_git_branch)\[\033[00m\] $ "
