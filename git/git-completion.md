## Run
```
curl https://raw.githubusercontent.com/git/git/master/contrib/completion/git-completion.bash -o ~/.git-completion.bash
```


## Update .bash_profile
```
source ~/git-auto-complete.bash
```

## Source
https://dev.to/dsc_ciet/how-to-enable-git-auto-completion-in-apple-terminal-40l2

http://apple.stackexchange.com/questions/55875/git-auto-complete-for-branches-at-the-command-line

## Error handling
If this error is happening:
```
unknown option: --list-cmds=list-mainporcelain,others,nohelpers,alias,list-complete,config
usage: git [--version] [--help] [-C <path>] [-c <name>=<value>]
  [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
  [-p | --paginate | --no-pager] [--no-replace-objects] [--bare]
  [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
  <command> [<args>]
```

Download the specific git version, for example: https://raw.githubusercontent.com/git/git/v2.17.1/contrib/completion/git-completion.bash

Source: https://apple.stackexchange.com/a/328144/318157
