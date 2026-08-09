# Base Debian playbook

Base playbook to set up a Debian box

Tested with Trixie, working on Ubuntu 26 support.

## Running

```bash
ssh-copy-id `#ip`
ansible-playbook master.yml -e tailscale_authkey=`#key` -e ansible_host=`#ip`
```

Firewall rules (& drift management) are handled externally by [OpenVox](https://voxpupuli.org/openvox/).
