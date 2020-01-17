1. Recursively delete "node_modules": 
Check space: FOR /d /r . %d in (node_modules) DO @IF EXIST "%d" rm -rf "%d"
Remove folder: Get-ChildItem -Path "." -Include "node_modules" -Recurse -Directory | Remove-Item -Recurse -Force
