# Pre-installation
## Dependencies
```
sudo dnf install ansible -y
ansible-galaxy collection install community.general
```

## Configuration
Go to vars.yml file and configure it appropriately.

# Post-installation
- configure dark theme and fonts in lxappearance

# Helper commands
Sometimes ansible will refuse to work over ssh for reasons I was too lazy to
investigate. This command will bypass that ssh check ansible does.
```
export ANSIBLE_HOST_KEY_CHECKING=False
```
# TODO
fix source for rvm and node
fix kmonad kernel module permissions
```

sudo usermod -aG input $USER 
sudo groupadd uinput
sudo usermod -aG uinput $USER

echo 'KERNEL=="uinput", MODE="0660", GROUP="uinput", OPTIONS+="static_node=uinput"' | sudo tee /etc/udev/rules.d/90-uinput.rules
```
