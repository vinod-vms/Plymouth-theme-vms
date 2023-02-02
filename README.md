# Plymouth-theme-vms

A theme that shows splash animation at startup.


https://user-images.githubusercontent.com/25525969/216385345-c9f6184a-7c92-464a-a374-4abddf01ebbf.mp4





## To install this theme:

### Make sure you have the packages for plymouth
sudo apt install plymouth

### After downloading or cloning themes, copy the selected theme in plymouth theme dir
sudo cp -r vms /usr/share/plymouth/themes/

### Install the new theme (vms)
sudo update-alternatives --install /usr/share/plymouth/themes/default.plymouth default.plymouth /usr/share/plymouth/themes/vms/vms.plymouth 100

### Select the theme to apply
sudo update-alternatives --config default.plymouth
#(select the number for installed theme, vms in this instance)

### Update initramfs
sudo update-initramfs -u
