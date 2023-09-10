# Shell Basics

## Tiny Helpers
- TAB will attempt to autocomplete
- &uarr; will bring up history/last used command

## Commands If its the same, then its the same. otherwise order is zsh/linux and then powershell

### Print a value to the console
```$zsh
echo 'Hello World'
```

### Create a file
```$zsh
touch filename
```

```$pwsh
New-Item [-Path] <path>
```

### create a folder
```
mkdir folderName
```

### delete a folder
https://learn.microsoft.com/en-us/powershell/module/microsoft.powershell.management/remove-item?view=powershell-7.3
```
Remove-Item -LiteralPath "foldertodelete" -Force -Recurse
```
### Go down one folder level

```$zsh
cd folderToGoInto
```

### Go Up one folder level

```$zsh
cd ..
```

### run a script (specically .sh vs .bat)

```$zsh
filename.sh
```

 - this one might be wrong, let me know
```$pwsh
.\filename.bat
```


### run an executable (python, java, code w/e)

```$zsh
executableName parametername
code fileToOpen.py
```


### show everything in a directory
```$zsh
ls
```

### make a file executable
```$zsh
chmod 755 YourScriptName.sh
```

```$zsh
chmod u+x /location/**/*.sh
```

