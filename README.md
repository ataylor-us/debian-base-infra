# Base Debian (Trixie) playbook

Base playbook to set up a Debian box

```bash
ssh-copy-id `#ip`
ansible-playbook master.yml -e tailscale_authkey=`#key` -e ansible_host=`#ip`
```

