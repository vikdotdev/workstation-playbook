# Pre-installation
## Usage
Go to vars.yml file and configure it appropriately.
```
bin/prepare
bin/run
```

# Helper commands
Sometimes ansible will refuse to work over ssh for reasons I was too lazy to
investigate. This command will bypass that ssh check ansible does.
```
export ANSIBLE_HOST_KEY_CHECKING=False
```

# Potentially useful commands
udevadm control --reload-rules
udevadm trigger
modprobe --first-time uinput

# fedora minimal things to do
setfont laratcyrheb-sub32.psfu.gz

# what dotfiles might need to do to compete with ansible
enable flathub remote
install flatpaks
install rpms
write to /etc
enable repos
installing packages
downloading and unpacking
settings hostname
enabling user service?
creating folders
unarchive
add usergroups
add user to group
chmod
make
nvm
npm packages
symlink



