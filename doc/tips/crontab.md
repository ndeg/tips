# Crontab

## Disable/Enable a crontab

If you use *vi* with the *crontab* command, you can comment each line of the crontab.

```bash
crontab -e
```

```vi
:%s/^/#/
:wq
```

To uncomment, do this :

```bash
crontab -e
```

```vi
:%s/^#//
:wq
```

[Back to index](../../README.md)
