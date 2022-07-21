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
| BIOS | C2ZE0200 X64 (20200812) |

</details>

## Issues
* Thunderbolt: "No drivers are loaded."
* USB-C output has no sound.
* HDMI output doesn't work.
* Power button is not functional.
* Power chime is not working when using internal speaker.
* system reboots very rarely instead of shutdown.

<details>
<summary>ERROR: "Timeout powering ON the panel" (a few seconds delay when internal display turned on)</summary>

2022-03-20 13:06:24.032687+0900 0x5fe      Default     0x0                  0      0    kernel: (AppleIntelICLLPGraphicsFramebuffer) [IGFB][ERROR][AUX       ] WR address = 0x004e0, data size = 2, cmd = 0x8004e001, ddi = 0 AUX received a NACK. Reply: 0x10

2022-03-20 13:06:24.032924+0900 0x5fe      Default     0x0                  0      0    kernel: (AppleIntelICLLPGraphicsFramebuffer) [IGFB][ERROR][AUX       ] WR address = 0x004e0, data size = 2, cmd = 0x8004e001, ddi = 0 AUX received a NACK. Reply: 0x10

2022-03-20 13:06:24.033157+0900 0x5fe      Default     0x0                  0      0    kernel: (AppleIntelICLLPGraphicsFramebuffer) [IGFB][ERROR][AUX       ] WR address = 0x004e0, data size = 2, cmd = 0x8004e001, ddi = 0 AUX received a NACK. Reply: 0x10

2022-03-20 13:06:24.033391+0900 0x5fe      Default     0x0                  0      0    kernel: (AppleIntelICLLPGraphicsFramebuffer) [IGFB][ERROR][AUX       ] WR address = 0x004e0, data size = 2, cmd = 0x8004e001, ddi = 0 AUX received a NACK. Reply: 0x10

2022-03-20 13:06:24.033627+0900 0x5fe      Default     0x0                  0      0    kernel: (AppleIntelICLLPGraphicsFramebuffer) [IGFB][ERROR][AUX       ] WR address = 0x004e0, data size = 2, cmd = 0x8004e001, ddi = 0 AUX received a NACK. Reply: 0x10

2022-03-20 13:06:24.033863+0900 0x5fe      Default     0x0                  0      0    kernel: (AppleIntelICLLPGraphicsFramebuffer) [IGFB][ERROR][AUX       ] WR address = 0x004e0, data size = 2, cmd = 0x8004e001, ddi = 0 AUX received a NACK. Reply: 0x10

2022-03-20 13:06:24.034097+0900 0x5fe      Default     0x0                  0      0    kernel: (AppleIntelICLLPGraphicsFramebuffer) [IGFB][ERROR][AUX       ] WR address = 0x004e0, data size = 2, cmd = 0x8004e001, ddi = 0 AUX received a NACK. Reply: 0x10

2022-03-20 13:06:24.034099+0900 0x5fe      Default     0x0                  0      0    kernel: (AppleIntelICLLPGraphicsFramebuffer) [IGFB][ERROR][AUX       ] writeAUX for address 0x4e0 failed with error 0xe00002f0

... (repeated many times)

2022-03-20 13:06:26.126927+0900 0x5fe      Default     0x0                  0      0    kernel: (AppleIntelICLLPGraphicsFramebuffer) [IGFB][ERROR][PANEL     ] Timeout powering ON the panel

2022-03-20 13:06:26.127173+0900 0x5fe      Default     0x0                  0      0    kernel: (AppleIntelICLLPGraphicsFramebuffer) [IGFB][ERROR][TRANSACTION] Path is not active in prepareAndSetPipePostCSCGamma

2022-03-20 13:06:26.391679+0900 0x762      Default     0x0                  0      0    kernel: (AppleIntelICLLPGraphicsFramebuffer) [IGFB][ERROR][DISPLAY   ] TxnHang1: FB0: IsTransactionComplete called following fakeVBL notification

2022-03-20 13:06:26.469292+0900 0x762      Default     0x0                  0      0    kernel: (AppleIntelICLLPGraphicsFramebuffer) [IGFB][ERROR][DISPLAY   ] TxnHang1: FB0: IsTransactionComplete called following fakeVBL notification

</details>
