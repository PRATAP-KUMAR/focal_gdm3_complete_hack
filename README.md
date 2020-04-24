# focal_gdm3_complete_hack
css file to edit like previous versions in Ubuntu starting from 17.10 to 19.10 for controlling login screen background in Ubuntu 20.04

Disclimer: editing the .css file is very risky. If any errors occur. you wont be able to use the desktop.
Proceed only if you know what you are going to edit.

for the freedom of editing the css file like in previous versions of Ubuntu starting from 17.10 to 19.10,
download the two files. `mygdm3.css` and `mygdm3.gresource`.

`mygdm3.gresource` is the copy of original file `/usr/share/gnome-shell/theme/Yaru/gnome-shell-theme.gresource` but to use `mygdm3.css` file.

1. `install -dv /usr/local/share/gnome-shell/theme/mygdm3`
2. put the above said downloaded files `mygdm3.css` and `mygdm3.gresource` in the above directory.
3. `update-alternatives --install /usr/share/gnome-shell/gdm3-theme.gresource gdm3-theme.gresource /usr/local/share/gnome-shell/theme/mygdm3/mygdm3.gresource 0`
4. `update-alternatives --set gdm3-theme.gresource /usr/local/share/gnome-shell/theme/mygdm3/mygdm3.gresource`

now you can edit the file `/usr/local/share/gnome-shell/theme/mygdm3/mygdm3.css` as before.
