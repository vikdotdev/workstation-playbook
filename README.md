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