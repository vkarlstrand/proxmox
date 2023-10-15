#

## Installation

### Proxmox installation
Insert USB and boot and install.
On SSD with ext4.
192.168.1.99/24
Gateway: 192.168.1.1
DNS: 127.0.0.1


## First setup
1. Disable enterprise repositories in Updates -> Repositories under the pve node.
2. Upgrade Proxmox: `apt-get update && apt-get upgrade`.
3. Insert `GRUB_CMDLINE_LINUX_DEFAULT="quiet intel_iommu=on iommu=pt pcie_acs_override=downstream,multifunction nofb nomodeset video=vesafb:off,efifb:off"` into `nano /etc/default/grub`.
4. `update-grub`

### Windows 11 Home


### Ubuntu 22.04 Desktop
