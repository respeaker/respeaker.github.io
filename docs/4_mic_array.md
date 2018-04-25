# ReSpeaker 4 Mic Array for Raspberry Pi

![](assets/images/4_mic_array.jpg)

[![Get One](assets/images/get_one.png)](https://www.seeedstudio.com/ReSpeaker-4-Mic-Array-for-Raspberry-Pi-p-2941.html)

The ReSpeaker 4 Mic Array for Raspberry Pi is a Pi hat with a 12 RGB LEDs ring.
It is designed to build voice enabled applications such as Google Assistant and Alexa.

There are several algorithms such as DOA, VAD, NS and KWS we can use with the 4 mic array.

## Sound Source Localization & Tracking
[ODAS](https://github.com/introlab/odas) is a very cool project to perform sound source localization, tracking, separation and post-filtering. Let's have a try!

![](https://github.com/introlab/odas_web/raw/master/screenshots/live_data.png)

1. get ODAS and build it

        sudo apt-get install libfftw3-dev libconfig-dev libasound2-dev
        git clone https://github.com/introlab/odas.git
        mkdir odas/build
        cd odas/build
        cmake ..
        make

2. get ODAS Studio from https://github.com/introlab/odas_web/releases and open it. You can run ODAS Studio on a computer or the Raspberry Pi.

    The `odascore` will be at `odas/bin/odascore`, the config file is at `odas/config/respeaker_4_mic_array.cfg`. Change `odas.cfg` based on your sound card number.


        interface: {
            type = "soundcard";
            card = 1;
            device = 0;
        }


    If you run the ODAS Studio on a computer, you should also need to change IP address from `127.0.0.1` to the IP of the computer.

## Resources
+ [Linux driver for Raspberry Pi](https://github.com/respeaker/seeed-voicecard)
+ [Algorithms includes DOA, VAD, NS](https://github.com/respeaker/mic_array)
+ [Voice Engine project, provides building blocks to create voice enabled objects](https://github.com/voice-engine/ec)
+ [Acoustic Echo Cancellation (AEC) project](https://github.com/voice-engine/ec)

## Wiki
[http://wiki.seeedstudio.com/ReSpeaker_4_Mic_Array_for_Raspberry_Pi](http://wiki.seeedstudio.com/ReSpeaker_4_Mic_Array_for_Raspberry_Pi)


