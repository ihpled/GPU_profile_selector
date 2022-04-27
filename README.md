# GPU profile selector Gnome-Shell-Extension

## Description
A simple gnome shell extension for switching GPU profiles on Nvidia Optimus systems (i.e laptops with Intel + Nvidia or AMD + Nvidia configurations).
In particular this extension is a graphic interface for [envycontrol](https://github.com/geminis3/envycontrol) program.

![screenshot example](./extension_screenshot.png)


## Dependencies
- [bash](https://www.gnu.org/software/bash/)
- [pkexec command](https://command-not-found.com/pkexec)
- [envycontrol](https://github.com/geminis3/envycontrol)


## Installation

### Gnome-shell Extension website
- Install all the [dependencies](#Dependencies)
- Enable extension in official [Gnome Extension](https://extensions.gnome.org/extension/5009/gpu-profile-selector/) store

### Manual
- Install all the [dependencies](#Dependencies)
- Clone this repo with:
```
git clone https://github.com/LorenzoMorelli/GPU_profile_selector.git ~/.local/share/gnome-shell/extensions/GPU_profile_selector@lorenzo9904.gmail.com
```


## Debuging

### For looking command line logs
```journalctl -f -o cat /usr/bin/gnome-shell```

### For looking updates using wayland (open a new wayland session in a window)
```dbus-run-session -- gnome-shell --nested --wayland```


## TODO
- Add a confirm dialog with restart later and restart now
- After profile is changed add a text at the end (reboot needed)
- Add support for other shell (not only bash)
