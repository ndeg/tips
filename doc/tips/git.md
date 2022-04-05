# Git

## Useful shortcuts

These commands will let you use shorten git commands, as :
*  `git br`
*  `git ci`
*  `git co`
*  `git st`

```bash
git config --global alias.br branch
git config --global alias.ci commit
git config --global alias.co checkout
git config --global alias.st status
git config --global alias.wip "for-each-ref --sort='authordate:iso8601' --format=' %(color:green)%(authordate:relative)%09%(color:white)%(refname:short)' refs/heads"
```

## Set meld as merge tool

```bash
git config --global merge.tool meld
```

## User-specific gitignore

Useful to avoid multiple IDE-specific .gitignore files in project .gitignore

```bash
touch $HOME/.gitignore
git config --global core.excludesfile $HOME/.gitignore
```

[Back to index](../README.md)
