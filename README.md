# Windows HWID & MAC Address Utility

A Windows-only Python tool for checking, backing up, changing, and restoring selected hardware/network identifiers from one simple menu.

This tool combines two main utilities:

1. HWID registry identifier checker/spoofer/restorer
2. Wi-Fi/Ethernet MAC address checker/randomizer/reverter

The updated version improves navigation by adding a cleaner main menu, grouped sections, and easier movement between HWID tools and MAC address tools.

---

## Features

### HWID Tools

- Check current hardware identifier values
- View:
  - MachineGuid
  - HwProfileGuid
  - ProductId
  - ComputerName
  - Active MAC addresses
  - Disk drive serial information
- Create a backup before changing registry-based identifiers
- Restore backed-up values from `hwid_backup.json`
- Automatically requests Administrator privileges when needed

### MAC Address Tools

- Check current Wi-Fi and Ethernet MAC addresses
- Show active MAC address and custom registry MAC value
- Randomize all detected supported Wi-Fi/Ethernet adapters
- Revert supported adapters back to default hardware MAC behavior
- Restart adapters automatically after changing/reverting MAC values
- Creates a log file for troubleshooting

### Navigation Improvements

- Cleaner main menu
- Separate HWID and MAC sections
- Back option from submenus
- Combined current status overview
- Command-line options still supported for MAC tools

---

## Requirements

- Windows 10 or Windows 11
- Python 3.10+
- Administrator permissions
- PowerShell available on the system

This script uses Windows-specific modules and commands, including:

- `winreg`
- `ctypes`
- `Get-NetAdapter`
- `Disable-NetAdapter`
- `Enable-NetAdapter`

It will not work on Linux or macOS.

---

## Installation

1. Install Python from the official Python website.
2. Download this repository.
3. Open Command Prompt or PowerShell as Administrator.
4. Run the script:

```bash
python Test_BetterNavigation.py
