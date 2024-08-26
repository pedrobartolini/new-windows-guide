# Windows cheatsheet

## Activating
- Open powershell
- Execute the code bellow then follow on screen instructions
```powershell
irm https://massgrave.dev/get | iex
```

## Disabling web search suggestions (the ones from BING that show up when you want to search for an program/file)
- Navigate to regedit path **HKEY_CURRENT_USER\Software\Policies\Microsoft\Windows**
- Create key in path **Explorer**
- It should look like this -> **HKEY_CURRENT_USER\Software\Policies\Microsoft\Windows\Explorer**
- Create DWORD 32 bit called **DisableSearchBoxSuggestions**
- Edit DWORD value to **hexadecimal** and **1**
- Reboot

## Disable write cache policy (IMPORTANT IF YOU HAVE AN WD NVME)
- Open device manager
- Right-click your NVME
- Properties
- Policies
<img src="https://raw.githubusercontent.com/pedrobartolini/new-windows-guide/main/write-cache.png" width="400">

## Activate native hardware accel
- Right click desktop
- Display settings
- Graphical settings
- Activate **Hardware-accelerated GPU Scheduling**
<img src="https://raw.githubusercontent.com/pedrobartolini/new-windows-guide/main/hardware-accel.png" width="800">

## Disable energy saving
- Search for **Power settings**
- Drag **Performance and Energy** to *Best performance*
<img src="https://raw.githubusercontent.com/pedrobartolini/new-windows-guide/main/power-settings.png" width="800">

## Uninstalling Cortana
- Open powershell as admin
- Execute code bellow
```powershell
Get-AppxPackage -allusers Microsoft.549981C3F5F10 | Remove-AppxPackage
```

## VCREDIST All-in-one package (if needed)
**VCREDIST AIO** https://github.com/abbodi1406/vcredist/releases
