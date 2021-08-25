<h1>Aliases</h1>
Creating a shortcut for the long commands or the commands that you often use is called aliases.

To see the aliases you currently have in your system use

```sh
alias
```

Creating Aliases

alias [name[=value]]

```sh
alias cls='clear'
```
To remove an alias

Remove the alias

```sh
unalias name
```
To remove all aliases

```sh
unalias -a
```

Persisting Aliases

If you would to logout and log back in your aliases would be lost to make them persist add them to your .files
Eg: .bash_profile, .bashrc

```sh
alias ls='ls -al'
```

```sh
alias cl='clear'
```

