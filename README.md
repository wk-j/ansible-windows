## Windows

```bash
vagrant up
vagrant ssh-config
vagrant winrm --command "dir"
vagrant winrm --command "choco install cpu-z -y"
vagrant winrm --command "choco install googlechrome -y"
vagrant winrm --command "winrm enumerate winrm/config/Listener"

ansible-playbook playbook.yml
ansible windows -m win_ping
```

## Resource

- https://www.linuxtechi.com/manage-windows-host-using-ansible