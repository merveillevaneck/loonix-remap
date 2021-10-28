# loonix-remap
snippet for remapping caps_lock to esc alone and to ctrl when pressed with other keys

# xcape

Install the program. On recent versions of Ubuntu, you should be able to just run:

```bash
sudo apt update
sudo apt install xcape
```
Next you need to remap caps_lock to control. Check out this EmacsWiki page for options. For Ubuntu/GNOME, I use GNOME Tweaks ($ `sudo apt install gnome-tweak-tool`), which has a setting for caps_lock as control under the control section or "typing" section.

Now run xcape:

```bash
xcape -e 'Control_L=Escape'
```
To keep it working through system restarts, you can add that line to your ~/.profile or use any method for running a script on startup.
