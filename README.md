<!--
If you want to use the free SVG icons referenced below,
copy the contents of `autopilotv2-icons/` into your repo at `assets/icons/`.
-->
Rafal Zimonczyk
# AutopilotV2

[![MEM Community — Official Community Tool](https://img.shields.io/badge/MEM%20Community-Official%20Community%20Tool-ffd700?labelColor=0b1220)](https://www.memcommunity.com/official-community-tool-oct)
![Platform](https://img.shields.io/badge/Windows-10%2F11-0078D6?logo=windows)
![Intune](https://img.shields.io/badge/Microsoft-Intune-5E5E5E?logo=microsoft)
![PowerShell](https://img.shields.io/badge/PowerShell-Graph-2B64B7?logo=powershell)
![Size](https://img.shields.io/badge/Size-~3%20MB-lightgrey)
[![Issues](https://img.shields.io/github/issues/rafallz10100/AutopilotV2)](https://github.com/rafallz10100/AutopilotV2/issues)
[![Stars](https://img.shields.io/github/stars/rafallz10100/AutopilotV2)](https://github.com/rafallz10100/AutopilotV2/stargazers)
[![Release](https://img.shields.io/github/v/release/rafallz10100/AutopilotV2?display_name=tag)](https://github.com/rafallz10100/AutopilotV2/releases)

**AutopilotV2** is a lightweight Windows application that **generates or imports `.csv` files into Microsoft Intune** for the **Windows Autopilot Device Preparation** process.

> This project is **officially recognized by the Modern Endpoint Management (MEM) Community as an “Official Community Tool.”**  
> Learn more: https://www.memcommunity.com/official-community-tool-oct

---

## Table of Contents
- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
  - [Import a `.csv` into Intune](#a-import-a-csv-into-intune)
  - [Generate a `.csv` (no import)](#b-generate-a-csv-no-import)
  - [If your system version isn’t compatible](#c-if-your-system-version-isnt-compatible)
- [Screenshots](#screenshots)
- [Troubleshooting & Permissions](#troubleshooting--permissions)
- [Recognition](#recognition)
- [Reporting Issues](#reporting-issues)
- [Project Status](#project-status)

---

## Features
- <img src="assets/icons/csv.svg" width="18" alt=""> Import device serial numbers from a `.csv` directly into Intune  
- <img src="assets/icons/export.svg" width="18" alt=""> Generate a valid `.csv` locally (without importing)  
- <img src="assets/icons/key-auth.svg" width="18" alt=""> Automatic detection/installation of **Microsoft.Graph.Authentication** and sign-in flow  
- <img src="assets/icons/duplicate-check.svg" width="18" alt=""> Duplicate protection (checks if a serial number was previously imported)  
- <img src="assets/icons/update.svg" width="18" alt=""> Version compatibility check for **Autopilot Device Preparation** with a shortcut to Windows Update  

---

## Requirements
- Windows 10 or Windows 11  
- ~3 MB free disk space  
- Internet access (required for sign-in and import)  
- Appropriate permissions in Entra ID / Intune (e.g., permission to import devices for Autopilot)

---

## Installation
- Download the repository (ZIP) or use the **Releases** section (if available).  
- Run the application on Windows 10/11.  

> **Note:** On first launch, the app checks for the **Microsoft.Graph.Authentication** PowerShell module and installs it if needed.

---

## Usage

### A) Import a `.csv` into Intune
1. Launch **AutopilotV2**.  
2. Click **Import Serial Number**.  
3. The app verifies **Microsoft.Graph.Authentication** (installs it if missing).  
4. Sign in with your Microsoft credentials.  
5. If you lack permissions, request them in **Entra ID** or ask an admin to consent on behalf of your organization (depending on your setup).  
6. The app checks whether the serial number(s) were already imported.  
7. The `.csv` is imported into Intune.

---

### B) Generate a `.csv` (no import)
1. Launch **AutopilotV2**.  
2. Click **Export to CSV file**.  
3. Notepad opens with the generated data.  
4. Save the file or copy the contents.

---

### C) If your system version isn’t compatible
1. If your Windows build does not meet **Autopilot Device Preparation** requirements, the app will show a visible notice.  
2. Click **Windows Update**.  
3. The Windows Update settings window will open.  
4. Install the required updates and retry.

---

## Screenshots

**Import flow**  
![AutopilotV2](https://github.com/user-attachments/assets/4feb9ed5-1338-4b2d-ac11-8caec93a2b6b)

**Generate `.csv`**  
![AutopilotV22](https://github.com/user-attachments/assets/1f6d2c4f-07c0-4ffc-b907-b7228800cef6)

**Incompatible system notice**  
![Device Preparation incompatibility](https://github.com/user-attachments/assets/892b7b49-d5ee-4128-8631-8a452c4ce023)

**Windows Update prompt**  
![Windows Update](https://github.com/user-attachments/assets/c4506c50-bef0-4100-aed4-a2b7b226d2ec)

---

## Troubleshooting & Permissions
- Ensure your account has sufficient **Intune/Entra ID** permissions to import Autopilot devices.  
- If module installation fails, verify your PowerShell execution policy and network access to the PowerShell Gallery.  
- Re-run the app after applying updates or permission changes.

---

## Recognition
This project is **officially recognized by the Modern Endpoint Management (MEM) Community as an “Official Community Tool.”**  
Learn more: https://www.memcommunity.com/official-community-tool-oct

---

## Reporting Issues
Found a bug or have an idea for improvement? Open an issue:  
**https://github.com/rafallz10100/AutopilotV2/issues**

---

## Project Status
Actively maintained and updated.
