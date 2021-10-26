# LG Gram 14 (14Z90N) hackintosh

<details>
<summary><strong>Specs</strong></summary>
</br>

| Model | 14Z90N-V.AR5DK |
| - | - |
| CPU | Intel Core i5-1035G4 |
| GPU | Intel Iris Plus Graphics |
| RAM | M471A1G44AB0-CWE (on-board) |
| SSD | ~~HFS256GD9TNG-L2A0A~~ Intel 7600p |
| LCD | LP140WFA-SPY1 |
| WLAN | Intel Wi-Fi 6 AX201 160MHz |
| Audio | Conexant CX8200 |
| BIOS | 20200812 |

</details>

## Issues
* HDMI output doesn't work.
* Thunderbolt: "No drivers are loaded."

## To-do
* Remap USB (left type-C and SD card reader)

## Touchpad
* VoodooI2C works as force polling mode. If you want to use Interrupt mode, set `Force unlock on all GPIO pads` to "Enabled", and remove `force-polling` in DeviceProperties.

## Weird mouse cursor
1. When LG logo is appeared, press F2 to enter Setup
2. Press "Ctrl + Alt + F7" to unlock advanced menu
3. Go to Advanced - Intel Advanced Menu - System Agent (SA) Configuration - Graphics Configuration
4. Set DVMT Pre-Allocated to 64M (default is 60M)
