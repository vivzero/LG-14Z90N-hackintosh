# LG Gram 14 (14Z90N) hackintosh

<details>
<summary><strong>Specs</strong></summary>
</br>

| Model | 14Z90N-V.AR5DK |
| - | - |
| CPU | Intel Core i5-1035G4 |
| GPU | Intel Iris Plus Graphics |
| RAM | M471A1G44AB0-CWE * 2 |
| SSD | ~~HFS256GD9TNG-L2A0A~~ *(Disabled)* <br> MTFDHBA512TDV-1AZ1AABYY |
| LCD | LP140WFA-SPY1 |
| WLAN | AX201D2W |
| Audio | Conexant CX8200 |
| BIOS | C2ZE0200 X64 (20200812) |

</details>

## Reported Issues
* Power management is poor than Windows.
* System reboots very rarely instead of shutdown.
* USB-C (DP Alt) has no sound.
* Thunderbolt: "No drivers are loaded."
* HDMI output is unsupported.
* Power button does not work.
* power chime internal speaker.

<details>
<summary>"Timeout powering ON the panel" (a few seconds delay when internal display turned on)</summary>

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

</details>
