
# Kali Linux Network Configuration | Cybersecurity Lab

**By Yogeshwaran S.**
Cybersecurity | VAPT | Linux Networking | Hands-on Lab Practice

## About This Project

I am building my practical cybersecurity skills by learning Linux fundamentals, network configuration, and troubleshooting.

In this lab, I worked with Kali Linux running inside Oracle VirtualBox. I explored virtual machine network settings, configured manual IPv4 settings, and used NetworkManager commands to reactivate the wired network connection.

This project documents my lab setup and the steps I performed with screenshots.

## What I Worked On

- Set up and launched Kali Linux in Oracle VirtualBox.
- Reviewed VirtualBox network adapter settings.
- Explored NAT Network configuration.
- Configured a manual IPv4 address, gateway, and DNS server.
- Used NetworkManager commands to reactivate the wired connection.
- Documented the process with screenshots.

## Lab Environment

| Component | Details |
|---|---|
| Operating System | Kali Linux 2026.1 |
| Virtualization Software | Oracle VirtualBox |
| IPv4 Method | Manual |
| IP Address | `10.0.0.2` |
| Network Prefix | `/24` |
| Default Gateway | `10.0.0.1` |
| DNS Server | `8.8.8.8` |

## 1. Kali Linux Installation

I launched Kali Linux inside Oracle VirtualBox and reviewed the desktop environment used for this lab.

![Kali Linux Desktop](screenshots/kali-desktop.jpg)

## 2. VirtualBox Network Settings

I reviewed the virtual machine's network adapter settings and explored the NAT Network configuration.

### VirtualBox Adapter

![VirtualBox Network Settings](screenshots/virtualbox-adapter.png)

### NAT Network Configuration

![NAT Network Configuration](screenshots/nat-network.png)

## 3. Kali Linux Network Configuration

I opened the wired connection's IPv4 settings and configured the IP address, network prefix, gateway, and DNS server manually.

![Kali Linux IPv4 Settings](screenshots/ipv4-settings.jpg)

## 4. Network Connection Management

I used NetworkManager commands to modify a connection setting and reactivate the wired connection.

### Commands Used

```bash
sudo nmcli connection modify "Wired connection 1" ipv4.dad-timeout 0
sudo nmcli connection down "Wired connection 1"
sudo nmcli connection up "Wired connection 1"
```

The terminal displayed successful deactivation and activation messages for the connection.

![NetworkManager Troubleshooting](screenshots/network-commands.jpg)

## What I Learned

- Using Kali Linux inside Oracle VirtualBox.
- Understanding virtual machine network settings.
- Learning about IPv4 addresses, gateways, and DNS.
- Exploring NAT and NAT Network configurations.
- Managing network connections using NetworkManager.
- Documenting technical work with screenshots.

## Security and Ethical Practice

This project is intended for educational purposes. Any cybersecurity testing should be performed only in authorized lab environments or on systems for which permission has been granted.

## Tools Used

- Kali Linux
- Oracle VirtualBox
- Linux Terminal
- NetworkManager (`nmcli`)
- IPv4 Networking

## References

- [Kali Linux Documentation](https://www.kali.org/docs/)
- [Oracle VirtualBox Documentation](https://www.virtualbox.org/manual/)

## Author

**Name:** Yogeshwaran S.  
**Project:** Kali Linux Network Configuration  
**Category:** Cybersecurity Lab Practice

---

*Learning by doing and building practical cybersecurity skills one lab at a time.*
