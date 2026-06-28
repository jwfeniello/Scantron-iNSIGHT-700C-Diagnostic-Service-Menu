# Scantron iNSIGHT 700C - All Console Menu Options
    
  The Scantron iNSIGHT 700C has a hidden diagnostic shell (`Phoenix Setup`)
  built into the firmware. You can access it over the regular USB port
  without opening the machine.
    
    ## How to Connect
    
    1. Plug the scanner into your PC using a standard USB printer cable.
    2. Open **PuTTY** (Windows) or run `screen /dev/ttyACM0 115200` (Linux).
    3. Set serial settings to **115200 baud, 8-N-1**.
    4. Power on the scanner or hit Enter to bring up the menu.
    
    ## Menu Commands
## Main Menu (`Phoenix Setup`)
    - `F` — Open Flash Menu
    - `S` — Set / rewrite machine serial number
    - `0` — Set / reset sheet counter 0 (lifetime scan count)
    - `1` — Set / reset sheet counter 1 (batch scan count)
    
    ## Flash Menu (`F`)
    - `B` — Blank check device memory
    - `D` — Display memory block hex dumps (`First block` to `Last block`)
    - `Ctrl+E` — Erase device flash blocks
    - `I` — Read hardware SPI Flash chip ID (`%04X-%04X`)
    - `Ctrl+P` — Lock / Protect flash blocks
    - `R` — Read / verify pseudo-random test data
    - `S` — Dump full firmware to S-record file (for backup)
    - `Ctrl+U` — Unlock / Unprotect flash device
    - `Ctrl+W` — Write pseudo-random test data
    - `X` — Exit menu back to Main Menu
