# OptiDarwin (Windows Optimizer)

**OptiDarwin** is a PowerShell-based optimizer for Windows that auto-elevates to Administrator and provides a
menu-driven interface to apply performance tweaks, disable optional services, and adjust system settings.

> ⚠️ Intended for advanced users. Read the safety notes before applying system-wide changes.

---

## 💡 What it does

- Auto-elevates to **Administrator** (UAC prompt)
- Offers a **Main Menu** of performance tweaks
- Includes a **Services Submenu** (Option 9) to disable optional services via registry (`Start = 4`)
- Creates a **restore point** (when possible) before applying bulk tweaks
- Cleans temp and prefetch folders, disables telemetry, Game DVR, hibernation, transparency, etc.

---

## 📋 Requirements

- Windows 10/11
- PowerShell (Windows PowerShell 5.1 or PowerShell 7+)
- **Administrator** privileges (auto-elevation is built in)
- Internet access (only for the download shortcuts you trigger from the menu)

---

## ▶️ How to run

1. Download `main.ps1` (this script).
2. Right-click **PowerShell** → **Run as Administrator**.
3. (If needed) Temporarily allow local script execution:
   ```powershell
   Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass
