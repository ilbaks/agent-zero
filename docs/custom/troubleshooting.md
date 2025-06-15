## when python run_ui.py
in gitbash
`$ echo "HOME is →  $HOME"`

got somethin like this
C:\Users?aksa/.config/git/config


added in .vscode/settings.json
```
    "terminal.integrated.profiles.windows": {
        "Git Bash": {
            "path": "C:\\Program Files\\Git\\bin\\bash.exe",
            "args": [
                "--login",
                "-i"
            ],
            "env": {
                "HOME": "C:\\Users\\baksa"
            }
        }
    },
    "terminal.integrated.defaultProfile.windows": "Git Bash"
```

