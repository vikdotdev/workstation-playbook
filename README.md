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

# TODO
fix source for node

# Potentially useful commands
udevadm control --reload-rules
udevadm trigger
modprobe --first-time uinput
