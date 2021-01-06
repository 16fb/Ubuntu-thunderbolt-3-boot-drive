# Ensure Ubuntu has Nvidia GPU Drivers and Support.
[Original Guide](https://linuxconfig.org/how-to-install-the-nvidia-drivers-on-ubuntu-18-04-bionic-beaver-linux)

### Detect model of nvidia graphics card + reccomended driver
`$ ubuntu-drivers devices`

### Install Reccomended Drivers
`$ sudo ubuntu-drivers autoinstall` 

### Specific Driver
`$ sudo apt install nvidia-340`

## IF Error: you have held broken packages
[Original Reference / Solution](https://askubuntu.com/questions/1077493/unable-to-install-nvidia-drivers-on-ubuntu-18-04)
### Try run package fixer
```
$ sudo apt -f install
$ sudo apt autoremove
```

### Remove all Nvidia packages, start with clean slate.
```
$ sudo apt-add-repository -r ppa:graphics-drivers/ppa
$ sudo apt update
$ sudo apt remove nvidia*
$ sudo apt autoremove
$ sudo ubuntu-drivers autoinstall
```

## Finally Reboot
REMEMBER IF SECURE BOOT IS ON, TO ENROLL KEY USING MOK \
DONT JUST BOOT WITHOUT VERIFYING 3RD PARTY DRIVERS.

### Why?
Ubuntu have to use 3rd party drivers to run GPU. \
If you have SECURE_BOOT on, you need to verify the drivers on restart using MOK manager before they can be used.

## Test Nvidia-Drivers work
Run:
* `nvidia-smi`