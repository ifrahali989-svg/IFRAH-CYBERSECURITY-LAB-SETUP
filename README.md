# Cybersecurity Lab Environment Setup 

## Project Overview
Setting up an isolated cybersecurity testing laboratory using VirtualBox and Kali Linux on a custom NAT Network subnet for NetworkWalks Internship Program.

## Network Configurations
- **Subnet:** 10.0.0.0/24
- **Kali Linux Static IP:** 10.0.0.2/24
- **Gateway:** 10.0.0.1
- **DNS:** 8.8.8.8

## Implementation Steps
1. Configured NAT Network on VirtualBox with subnet `10.0.0.0/24`.
2. Allocated resources for Kali Linux VM and set graphics controller to `VBoxSVGA`.
3. Configured static IP `10.0.0.2/24` using NetworkManager (`nmcli`) for persistence.
4. Resolved IP dad-timeout and established full internet access.
5. Configured Shared Folder (`Downloads`) and Drag & Drop/Clipboard integration.
6. Created VM Snapshot for environment rollback.

## Troubleshooting & Verification
- **Display Hang Issue:** Resolved by changing Graphics Controller to `VBoxSVGA`.
- **Network Persistence:** Fixed IP resetting issue using `sudo nmcli connection modify` commands.
- **Internet Connectivity:** Verified via `ping google.com` (0% packet loss).

  <img width="766" height="510" alt="VirtualBox_Snapshot" src="https://github.com/user-attachments/assets/c1584094-924c-4160-a9d2-44a9fff99eba" />
<img width="767" height="486" alt="Kali_Terminal" src="https://github.com/user-attachments/assets/ae02d12f-fcbc-4db1-b1eb-f3f2aa9f15ec" />
