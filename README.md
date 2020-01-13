# Tips

## Git

### Useful shortcuts

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
```

### User-specific gitignore

Useful to avoid multiple IDE-specific .gitignore files in project .gitignore

```bash
touch $HOME/.gitignore
git config --global core.excludesfile $HOME/.gitignore
```