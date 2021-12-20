# LG Gram 14 (14Z90N) hackintosh
![11](https://img.shields.io/badge/macOS-11-Green)

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
* USB-C connection is lost repeatedly after wake from sleep.
* 3.5mm combo jack: audio input (microphone) doesn't work.
* Thunderbolt: "No drivers are loaded."
* Brightness is lower than Windows. (S3 Sleep can fix it)
* HDMI output doesn't work at all.

</details>

## Weird mouse cursor
1. When LG logo is appeared, press F2 to enter Setup
2. Press "Ctrl + Alt + F7" to unlock advanced menu
3. Go to Advanced - Intel Advanced Menu - System Agent (SA) Configuration - Graphics Configuration
4. Set DVMT Pre-Allocated to 64M (default is 60M)

## Click works as Force Click
1. Go to "System Preferences" - "Trackpad"
2. Disable "Force Click and haptic feedback"
