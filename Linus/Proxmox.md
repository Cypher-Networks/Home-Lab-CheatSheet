# Proxmox - VM 

Proxmox VE is a complete open-source platform for enterprise virtualization. With the built-in web interface you can easily manage VMs and containers, software-defined storage and networking, high-availability clustering, and multiple out-of-the-box tools on a single solution.

[Proxmox - Powerful open-source server solutions](https://www.proxmox.com/en/)

Massive helper scripts for Proxmox. 
[GitHub - tteck/Proxmox: Proxmox Helper Scripts](https://github.com/tteck/Proxmox)


# Ignore lid closed on laptop

To ignore the laptop being close edit the below to allow for system to still run when lid is closed. 

```bash
// Edit the following file
sudo nano /etc/systemd/logind.conf

// Uncomment this line 
#HandleLidSwitch=suspend

// Change to
#HandleLidSwitch=ignore

// Restart service with the following
sudo systemctl restart systemd-logind
``` 



