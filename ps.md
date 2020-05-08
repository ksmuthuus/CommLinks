# Key PS commands

## Recursively delete "node_modules"

### Check spac

```sh
FOR /d /r . %d in (node_modules) DO @IF EXIST "%d" rm -rf "%d"
```

### Remove folder

```sh
Get-ChildItem -Path "." -Include "packages" -Recurse -Directory | Remove-Item -Recurse -Force
```
