# Pre-installation
## Dependencies
```
sudo dnf install ansible -y
ansible-galaxy collection install community.general
ansible-galaxy install rvm.ruby
```
## Usage
```
ansible-playbook -K main.yml
```

add ruby script to fill vars and run ansible
install ruby by hand?

## Configuration
Go to vars.yml file and configure it appropriately.

# Post-installation
- reboot
- configure syncthing https://docs.syncthing.net/intro/getting-started.html
- configure dark theme and fonts in lxappearance

# Helper commands
Sometimes ansible will refuse to work over ssh for reasons I was too lazy to
investigate. This command will bypass that ssh check ansible does.
```
export ANSIBLE_HOST_KEY_CHECKING=False
```

# Caveats
`nvm` installation is imperfect and any `npm` packages will fail on first run. To fix that, open new shell and run the command again. This will load `nvm` and `npm` into path.

# TODO
fix source for nvm
add xss-lock

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
