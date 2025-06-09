# Mordad

Desktop Linux Kernel Optimization

---
## Apply sysctl conf
```bash
sudo mkdir -p /etc/sysctl.d

sudo mv sysctl.d/99-sysctl.conf /etc/sysctl.d

sudo sysctl -p
```

## Apply cmdline on every boot
```bash
cat cmdline
sudo vim /etc/default/grub

# Add boot params in this line
GRUB_CMDLINE_LINUX_DEFAULT="..."
```
