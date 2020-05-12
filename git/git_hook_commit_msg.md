#!/bin/sh
# Check if it is an ammend
# https://stackoverflow.com/a/56955369
IS_AMEND=$(ps -ocommand= -p $PPID | grep -e '--amend');
if [ -n "$IS_AMEND" ]; then
  exit 0;
fi

# Get the current branch name
BRANCH_NAME=$(git symbolic-ref --short HEAD)
TRIMMED=$(echo $BRANCH_NAME | grep -io 'replaceme-\d*') # TODO

# Preprend the trimmed branch identifier to the given message
if [ -n "$BRANCH_NAME" ] ; then
  sed -i.bak -e "1s/^/$TRIMMED /" $1
fi

# https://medium.com/@nicklee1/prepending-your-git-commit-messages-with-user-story-ids-3bfea00eab5a
