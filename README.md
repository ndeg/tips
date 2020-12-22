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

* [Image data cleaner](https://github.com/codepo8/image-data-cleaner) - Javascript tool to remove exif data from images.
* [Rector](https://getrector.org/) - PHP refactoring automation
