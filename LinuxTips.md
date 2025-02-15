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
- `StartupWMClass` should be the same as the `--class` and `--name` for correct identifications.
- `xprop | grep WM_CLASS` from the Terminal, click on the window created, `StartupWMClass` should match this.