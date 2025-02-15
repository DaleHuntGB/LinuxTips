# Desktop Applications: Web Apps
## Brave:
```
[Desktop Entry]
Version=1.0
Type=Application
Name=ChatGPT
Comment=Chat with ChatGPT
Exec=brave --app="https://chatgpt.com/" --class=WebApp-ChatGPTIsolated --name=WebApp-ChatGPTIsolated --new-window
Icon=/home/dale/Pictures/AppLogos/ChatGPT.png
Categories=Network;Chat;
Terminal=false
StartupWMClass=WebApp-ChatGPTIsolated
```
- You can add any URL you want. Adjust `Comment`, `Icon`, `Categories` as you see fit.
- `StartupWMClass` should be the same as the `--class` and `--name` for correct identifications.