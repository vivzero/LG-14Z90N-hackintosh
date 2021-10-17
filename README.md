# LG Gram 14 (14Z90N) hackintosh

# WIP

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
| Audio | ? |
| BIOS | 20200812 |

* No need to change BIOS settings. (without Secure Boot)

</details>

## To-do
* Fix sleep
* Fix USB

## Touchpad
* VoodooI2C works as force polling mode. If you want to use Interrupt mode, set `Force unlock on all GPIO pads` to "Enabled", and remove `force-polling` in DeviceProperties.