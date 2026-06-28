# RCJ2026-Korea_CAD-design-files

This repository contains the CAD design files for RoboCup Junior 2026.

## 📱 Download Repository

If you are viewing this document on paper or another device, scan the QR code below to open this repository directly.

<p align="center">
  <img src="qr.png" alt="Repository QR Code" width="220">
</p>

---

## Why are the files split?

GitHub has a maximum file size limit of **100 MB**.

Because the original Fusion 360 archive files (`.f3z`) exceed this limit, they have been split into multiple **80 MB** parts (such as `Part_aa`, `Part_ab`, etc.).

Before opening the CAD files in Fusion 360, you must combine the parts back into a single `.f3z` file.

---

# macOS

1. Open **Terminal**.
2. Move to the downloaded repository.

```bash
cd /path/to/RCJ2026-Korea_CAD-design-files
```

3. Run the following commands.

```bash
cat AIR_2026_Robot_Part_* > AIR_2026_Robot_ATK.f3z
cat AIR_2026_Robot_DEF_Part_* > AIR_2026_Robot_DEF.f3z
```

---

# Windows (Command Prompt)

1. Open **Command Prompt**.
2. Move to the downloaded repository.

```cmd
cd C:\path\to\RCJ2026-Korea_CAD-design-files
```

3. Run the following commands.

```cmd
copy /b AIR_2026_Robot_Part_aa + AIR_2026_Robot_Part_ab + AIR_2026_Robot_Part_ac + AIR_2026_Robot_Part_ad + AIR_2026_Robot_Part_ae AIR_2026_Robot_ATK.f3z

copy /b AIR_2026_Robot_DEF_Part_aa + AIR_2026_Robot_DEF_Part_ab + AIR_2026_Robot_DEF_Part_ac + AIR_2026_Robot_DEF_Part_ad + AIR_2026_Robot_DEF_Part_ae AIR_2026_Robot_DEF.f3z
```

---

# Windows (PowerShell)

1. Open **PowerShell**.
2. Move to the downloaded repository.

```powershell
cd C:\path\to\RCJ2026-Korea_CAD-design-files
```

3. Run the following commands.

```powershell
Get-Content AIR_2026_Robot_Part_* -Encoding Byte | Set-Content AIR_2026_Robot_ATK.f3z

Get-Content AIR_2026_Robot_DEF_Part_* -Encoding Byte | Set-Content AIR_2026_Robot_DEF.f3z
```

---

## Done!

After the commands finish, the following Fusion 360 files will be created:

* `AIR_2026_Robot_ATK.f3z`
* `AIR_2026_Robot_DEF.f3z`

You can now open these files directly in Fusion 360.
