# Replay_Organizer
This script is intended to be used with [GPU-screen-recorder](https://git.dec05eba.com/gpu-screen-recorder/about/) and that what I'm using it for.
# How to use
use it with `-sc` flag. 
for example when starting the replay buffer.

`gpu-screen-recorder -w screen -f 60 -a "$(pactl get-default-sink).monitor" -c mp4 -r 30 -o $HOME/Vidoes/Replays -sc path/to/script`
