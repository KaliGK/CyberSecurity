#!/usr/bin/zsh

if [ -f ~/.zsh_history ]; then
    cp ~/.zsh_history ~/.zsh_history.backup
else
    echo "No .zsh_history file found."
    break
fi

strings ~/.zsh_history > ~/.zsh_history.cleaned 

mv ~/.zsh_history.cleaned ~/.zsh_history 

fc -R ~/.zsh_history 

echo "History file successfully cleaned and reloaded."
