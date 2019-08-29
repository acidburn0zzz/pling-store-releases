# Pling-Store

Pling-Store is a Content Management App for OCS-compatible websites like opendesktop.org, gnome-look.org, etc.
It allows to download and install applications, desktop themes, icon themes, wallpapers, or mouse cursors 
under various desktop environments using the "Install"-button.

Currently supported are these desktop environments:
KDE Plasma, Gnome, XFCE, Mate, Cinnamon, Budgie, LXQt, Elementary and Enlightenment.

## Usage

Using the Appimage package format, it should work on any distro like Ubuntu, Debian, Arch, Suse, Redhat and many more.


### Best with AppImageLauncher

If you never used an Appimage before, we recommend this tool to make AppImages run, install/uninstall and update on your Linux OS:
https://www.pling.com/p/1228228/

*Please see if AppImageLauncher offers native packages for your distro, if not, you may request it in the issue section.*

After installing AppImageLauncher, you can simply Double-Click on the Pling-Store Appimage to run or install it.


###  Manual Run

To try the Pling-Store without installing, you can simply [make it executable](https://youtu.be/nzZ6Ikc7juw?t=78) and (double-)click on it. 

## Development

The Pling-Store is a regular electron app plus the [ocs-manager](https://git.opendesktop.org/akiraohgaki/ocs-manager/). The first acts as a presentation 
layer and the second is the one who handles the intallation of the different products.

### Project Setup

```
npm install
curl -fsSL -o node_modules/.bin/ocs-manager https://git.opendesktop.org/akiraohgaki/ocs-manager/uploads/d3dc42436b82d11360ebc96b38d4aaf4/ocs-manager-0.8.1-1-x86_64.AppImage
chmod +x node_modules/.bin/ocs-manager
```


### AppImage Generation

`./scripts/package appimage`
