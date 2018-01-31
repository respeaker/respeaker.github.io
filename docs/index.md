# The ReSpeaker Project

!!! Note
    The website is still under construction

The ReSpeaker project provides hardware components and software libraries to build voice enabled device.

![](assets/images/vui.png)

## Hardware

The hardware components include I2S 2 microphone array, I2S 4 microphone array, USB 6+1 microphone array, ReSpeaker Core 7688.

|  | USB 6+1 Mic Array | 4 Mic Array for Pi | 2 Mic Array for Pi | MT7688 Core | USB 4 Mic Array |
|:------------:|:-------------------------------------:|:------------------:|:------------------:|:----------------------------------------------------------------:|:---------------:|
| Microphones | 7 | 4 | 2 | 1 | 4 |
| Shape | circular | square | rectangle | circular | circular |
| Interface | USB | I2S | I2S | WiFi | USB |
| RGB LEDs | 12 | 12 | 3 | 12 | 12 |
| Audio Output | Mono | NA | Stereo | Stereo | Mono |
| Note | built-In audio processing algorithms  |  |  | on-baord ATmega32U4  for Arduino compatible usage,  touch sensor | coming soon |

## Sofware

Audio processing algorithms including VAD, DOA, Beamforming, NS, AEC and KWS are available and are evolving rapidly.

![](assets/images/mic_array.png)



