# Replay_Organizer
This script is intended to be used with [GPU-screen-recorder](https://git.dec05eba.com/gpu-screen-recorder/about/) and that's what I'm using it for. Just wanted it to archive it here.

# Requirement


| Dependency            | DE/WM                                                                |
| ----------------- | ------------------------------------------------------------------ |
| xdotool | X11 |
| [kdotool](https://github.com/jinliu/kdotool) | KDE (Wayland) |
| jq | Hyprland |


# How to use

use it with the `-sc path/to/the/script' argument when starting GSR reply buffer.

Example:
```bash
`gpu-screen-recorder -w screen -f 60 -a "$(pactl get-default-sink).monitor" -c mp4 -r 30 -o $HOME/Vidoes/Replays -sc path/to/script`
```


# Limitations
The way it works that it checks for the window class if it has `steam_app_` followed by the game id,  or ends with `exe` , which games on proton & wine do. 
You could add or remove classes to serve your needs, so change WhiteListApps variable to your needs.

