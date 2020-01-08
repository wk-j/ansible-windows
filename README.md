## Windows

```bash
vagrant up
vagrant winrm-config
vagrant winrm --command "dir"
vagrant winrm --command "choco install cpu-z -y"
vagrant winrm --command "choco install googlechrome -y"
vagrant winrm --command "winrm enumerate winrm/config/Listener"

export no_proxy='*'
ansible-playbook playbook.yml
ansible windows -m win_ping
ansible windows -m shell -a 'echo Hello' -u vagrant -K
```

## Resource

- https://www.linuxtechi.com/manage-windows-host-using-ansible
- https://www.whatan00b.com/posts/debugging-a-segfault-from-ansible