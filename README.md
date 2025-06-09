# Mordad

Desktop Linux Kernel Optimization

---
## Apply sysctl params
```bash
sudo mkdir -p /etc/sysctl.d

sudo mv sysctl.d/99-sysctl.conf /etc/sysctl.d

sudo sysctl -p
```

## Apply boot params on every boot
```bash
cat cmdline
sudo vim /etc/default/grub

# Add boot params in this line
GRUB_CMDLINE_LINUX_DEFAULT="..."

# Update the grub
sudo grub-mkconfig -o /boot/grub/grub.cfg
# or
sudo update-grub
```
