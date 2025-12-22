# Homelab server running on KVM/QEMU virtualization

## Requirements

### Arch

#### Needed packages

``` shell
paru -Syu libvirt qemu-full dnsmasq openbsd-netcat virt-manager
```

#### Start required daemons(maybe enable in the future)

```
systemctl start libvirtd.service
systemctl start virtlogd.service
```

#### (Optional)Enable required daemons(maybe enable in the future)

```
systemctl enable libvirtd.service
systemctl enable virtlogd.service
```

## TODO

- Start virtual machine(OpenSuse Leap 16)
- Migrate to minimal KVM iso(OpenSuse Leap 16)
- Set up networking
- Set up firewall
- Set up wireguard(or tailscale)
- Set up ssh
- Set up redundancy(raid)
- Make it all repeatable with a simple script and a .env file
