# 🖧 Windows Network Sharing Fix

Download here: https://github.com/ibay770/enablenetworklogon/blob/main/enablenetworklogon.reg


This fixes the error:

You might not have permission to use this network resource.


This repository contains a comprehensive `.reg` file and batch script to fix common Windows file-sharing and network discovery issues.  

If you're getting errors like:
The network is not present or not started. ``` — this solution can help. --- ## 🛠 What's Included ### ✅ `network_sharing_fix.reg` Applies registry tweaks to: - Start essential networking services (Workstation, TCP/IP, Netlogon, etc.) - Enable **Network Discovery** and **File & Printer Sharing** - Open necessary **Windows Defender Firewall** exceptions - Disable anonymous access restrictions (`restrictanonymous` / `restrictanonymoussam`) ### ✅ `restart_network_services.bat` Restarts the required Windows services after applying the `.reg` file — helpful for avoiding a reboot. --- ## 📥 How to Use ### Step 1: Apply the Registry Fix 1. Double-click `network_sharing_fix.reg` 2. Accept the UAC and Registry prompts 3. (Optional) Reboot your PC ### Step 2: Restart Services (Optional) Run `restart_network_services.bat` as Administrator to restart all necessary services immediately: 

```bash Right-click > Run as Administrator ``` --- ## 🧩 When to Use This Use this fix when: - You're unable to access shared drives or folders across local PCs - Network Discovery or File Sharing is not working properly - You're seeing errors related to permissions or network services not being started --- ## ⚠️ Notes & Warnings - This is intended for **trusted LAN environments** only. - Disabling anonymous restrictions may reduce security on untrusted networks. - Works best when both PCs apply the same fix. --- ## 📄 License This project is provided "as-is" with no warranty. Use at your own risk in personal or internal environments. ``

