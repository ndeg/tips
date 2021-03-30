# Tips

/!\ /!\ /!\ Use at your own risks /!\ /!\ /!\

## Firefox

### Prevents copy-paste disabling on website

```bash
about:config
dom.event.clipboardevents.enabled => false
```

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
git config --global alias.wip "for-each-ref --sort='authordate:iso8601' --format=' %(color:green)%(authordate:relative)%09%(color:white)%(refname:short)' refs/heads"
```

### Set meld as merge tool

```bash
git config --global merge.tool meld
```

### User-specific gitignore

Useful to avoid multiple IDE-specific .gitignore files in project .gitignore

```bash
touch $HOME/.gitignore
git config --global core.excludesfile $HOME/.gitignore
```

## Video

### How to get technical information about a video

```bash
mediainfo myfile.avi
```

### How to rotate a video to 90 degrees.

```bash
ffmpeg -i input -vcodec libx264 -preset medium -crf 24 -threads 0 -vf transpose=1 -acodec copy output.mkv
```


## Useful tools
* [Git Elephant](https://github.com/matteosister/GitElephant) - Abstraction layer to manage git repositories with PHP.
* [Image data cleaner](https://github.com/codepo8/image-data-cleaner) - Javascript tool to remove exif data from images
* [Parsica](https://parsica.verraes.net/) - Build robust parser in PHP
* [Rector](https://getrector.org/) - PHP refactoring automation tool
