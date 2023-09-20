# zsh-systemd

> zsh-systemd is a zsh plugin that provides aliases for `systemd` commands, both system and user.

## installing

### zinit

Add this to your zinit config (.zshrc):

```zsh
zinit light redxtech/zsh-systemd

# it also works with turbo mode:
zinit ice wait lucid
zinit load redxtech/zsh-systemd
```

### oh-my-zsh

Install it with your favourite zsh package manager, or clone it directly to your `$ZSH_CUSTOM/plugins` directory with git, and add `systemd` to the plugins array in your `.zshrc` file:

```zsh
plugins=(... systemd)
```

## usage

here is a list of all the commands:

```zsh
alias ss="sudo systemctl"
alias sss="sudo systemctl status"
alias ssstart="sudo systemctl start"
alias ssstop="sudo systemctl stop"
alias ssr="sudo systemctl restart"
alias sse="sudo systemctl enable --now"
alias ssd="sudo systemctl disable --now"
alias ssm="sudo systemctl mask"
alias ssum="sudo systemctl unmask"
alias ssdr="sudo systemctl daemon-reload"

alias scu="systemctl --user"
alias ssu="systemctl --user status"
alias scus="systemctl --user start"
alias scust="systemctl --user stop"
alias scur="systemctl --user restart"
alias scue="systemctl --user enable --now"
alias scud="systemctl --user disable --now"
alias scum="systemctl --user mask"
alias scuum="systemctl --user unmask"
alias scudr="systemctl --user daemon-reload"
```

## author

**zsh-systemd** © [gabe dunn](https://github.com/redxtech), released under the [MIT](./LICENSE) License.
