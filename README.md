# Desktop Applications: Web Apps
## Brave:
```
[Desktop Entry]
Version=1.0
Type=Application
Name=ChatGPT
Exec=brave --app="https://chatgpt.com/" --class=WebApp-ChatGPT --name=WebApp-ChatGPT --new-window
Icon=/home/dale/Pictures/AppLogos/ChatGPT.png
Categories=Network;Chat;
Terminal=false
StartupWMClass=chatgpt.com
```

- You can add any URL you want. Adjust `Comment`, `Icon`, `Categories` as you see fit.

# Desktop Applications: Shortcuts
```
[Desktop Entry]
Type=Application
Name=Battle.net
Icon=/home/dale/Pictures/Logos/Battle.net.png
Exec=env LUTRIS_SKIP_INIT=1 lutris lutris:rungameid/1
Categories=Game
TryExec=lutris
StartupWMClass=battle.net.exe
```

- `StartupWMClass` should be the same as the `--class` and `--name` for correct identifications.
- `xprop | grep WM_CLASS` from the Terminal, click on the window created, `StartupWMClass` should match this.

# Improving Your Terminal
- Find Your Shell: `echo $SHELL`
## `/bin/bash`
- Open `~/.bashrc` - `sudo nano ~/.bashrc`
- `\u`: Username.
- `\w`: Current Directory.
- `\e`: Escape Sequence - Used for Specific Styling.
- `$`: Normal User. | `#`: Root User.
- `dale > ~ : $` is my current style.
    - `PS1='\u > \w : '` can be added to the `~/.bashrc`.
    - `PS1='\[\e[1;34m\]\u > \[\e[1;32m\]\w \[\e[1;36m\]: \[\e[1;37m\]\$ \[\e[0m\]'`.
    - The second command is a coloured, bolded version. Feel free to play around with colours.
- Once you have added: `Ctrl + S` > `Ctrl + X` and restart your Terminal.

# Terminal Commands
- If you need to copy files, `cp` is the way. `cp /path/to/file /path/to/dest_file`, you can run this as `sudo`.
- If you need to move / rename files, `mv` is the way. `mv /path/to/file /path/to/dest_file`, you can run this as `sudo`. If you `mv` to the same location as the existing file, it will rename.
## Arch Specific:
- `pacman -Q | wc -l` will list the number of installed packages.
- `pacman -Qqdt` will list all orphaned packages.

# File Manager Tips
- `Ctrl + L` will access the address bar > `admin:/` will enter root mode.