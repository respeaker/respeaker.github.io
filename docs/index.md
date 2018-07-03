# The ReSpeaker Project

!!! Note
    The website is still under construction

The ReSpeaker project provides hardware components and software libraries to build voice enabled device.

![](assets/images/vui.png)

## Hardware

The hardware components include I2S microphone array for Raspberry Pi, USB microphone array for Linux/Windows/macOS, standalone ReSpeaker Core v1.0 & v2.0.

### Microphone Array

|              | USB 4 Mic Array     | 2 Mic Array for Pi | 4 Mic Array for Pi | 4 Linear Mic Array for Pi | 6 Mic Array for Pi |
|:------------:|---------------------|:------------------:|:------------------:|:-------------------------:|:------------------:|
|  Microphones | 4                   |          2         |          4         |             4             |          6         |
|     Shape    | circular            |       linear       |       square       |           linear          |       hexagon      |
|   Interface  | USB                 |         I2S        |         I2S        |            I2S            |         I2S        |
|   RGB LEDs   | 12                  |          3         |         12         |             NA            |         12         |
| Audio Output | Mono                |       Stereo       |         NA         |           Stereo          |       Stereo       |
|     Note     | built-in algorithms |                    |                    |                           |                    |

If you are looking for a custom shape mic array, you may want to try [Seeed's Fusion service](https://www.seeedstudio.com/fusion.html) to design a new one based on our design. It should be easy.

### Standalone ReSpeaker Core

|             | ReSpeaker Core v1 (MT7688)  | ReSpeaker Core v2 (RK3229)                    |
|-------------|-----------------------------|-----------------------------------------------|
| CPU         | MT7688 (MIPS24KEc, 580 MHz) | RK3229 (4 ARM Cortex A7 cores, 1.5GHz)        |
| RAM         | 256 MB                      | 1 GB                                          |
| Microphones | 1                           | 6                                             |
| Shape       | circular                    | hexagon                                       |
| Interfaces  | WiFi, USB device            | WiFi, Bluetooth, Ethernet, HDMI, USB otg/host |
| loopback    | NA                          | 2 channels                                    |

## Software

Audio processing algorithms includes VAD, DOA, Beamforming, NS, AEC and KWS.

![](assets/images/mic_array.png)

