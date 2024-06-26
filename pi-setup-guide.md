# Pi Setup Guide

## Milestone C4

### C1.10 WiFi Setting Up

While you are writing the image into the SD card, please make sure your WiFi configurations are correct. Your rapsberry Pi should be able to connect to the WiFi when you first power it.

### C2.2 Looking for the IP address of Raspberry Pi

If you are using Windows 10/11 or MacOS hotsport to provide WiFi, you can easily see the IP address of your Raspberry Pi (2.4GHz).

<figure><img src=".gitbook/assets/1719391966287.png" alt=""><figcaption><p>Win10 Hotspot Config Page</p></figcaption></figure>

Although Raspberry Pi 4 is able to connect with 5.0GHz WiFi, the 2.4GHz has a higher compatibility to Rapsberry Pi.

If you are using iPhone Hotspot, you may unable to get the IP address of your Raspberry Pi. Now please  use NetSetMan to enumerate the machines that connect with your iPhone and get the Ip address of the Raspberry Pi. (Your PC should connect to the iPhone's Hotspot!)

<figure><img src=".gitbook/assets/1719392777299.png" alt=""><figcaption><p>NetSetMan's Screenshot</p></figcaption></figure>

### C3 Using SSH to skip the Setting Up using GUI

In case you cannot using GUI mode of the Raspberry Pi or you do not have keyboard or mouse as peripheros, we use SSH to finish configuring of the Raspberry Pi.

Make sure in C1.10, you have enabled SSH in OS Customisation section of Raspberry Pi Imager.

To SSH, you need to connect your PC, your Raspberry Pi in the same network, and you know the IP address or the name of your Raspberry Pi.

```shell-session
ssh <username>@<RPi's name/RPi's IP Address>
```

for me, the command is `ssh pi@sws3009` or `ssh pi@192.168.137.43`.

You should enable the figerprint check and insert correct password to your Raspberry Pi (for securety reason, you will not see what you type in password session)

<figure><img src=".gitbook/assets/1719394141153.png" alt=""><figcaption><p>SSH Connection to Raspberry Pi</p></figcaption></figure>

Insert: `sudo raspi-config`, and click Enter, you should see a blue screen with options in a grey box:

<figure><img src=".gitbook/assets/1719395809785.png" alt=""><figcaption><p>Raspberry Pi 4 Configuration Tool</p></figcaption></figure>

Use the **Up** and **Down** arrow keys to move the highlighted selection between the options available.

Press the **Right** arrow key or press **Tab** to access the `<Select>` and `<Finish>` buttons. Press **Left** or press **Tab** to return to the options.

Select the "Interfaces" tab and enable:&#x20;

* Camera\*
* SSH (you should have enabled)
* VNC

If you did not see the camera at this stage, it is OK! We will guide you in next stage.

You should reboot your Raspberry Pi after changing the above configuration, type `sudo reboot` to restart your Raspberry Pi.

### C4.6 VNC Setting Up

Please download VNC from: [https://www.realvnc.com/en/connect/download/](https://www.realvnc.com/en/connect/download/)

&#x20;If you encounter the “**Cannot currently show the desktop**” error while using VNC, you can resolve this issue by editing the `boot/config.txt` file on your Raspberry Pi. Please read the section 2 at: [https://www.comp.nus.edu.sg/\~guoyi/tutorial/cg2111a/ros-setup/](https://www.comp.nus.edu.sg/\~guoyi/tutorial/cg2111a/ros-setup/).

## Milestone C6

### C6.1 Running `rpicam-hello`

You should see if your RPi Camera can work correctly:

<figure><img src=".gitbook/assets/image (48).png" alt=""><figcaption><p>Bitvise Terminal</p></figcaption></figure>

### C6.1 Running `rpicam-jpeg --output test.jpg`



<figure><img src=".gitbook/assets/image (49).png" alt=""><figcaption><p>Bitvise Terminal</p></figcaption></figure>

You may see the test picture from `/home/pi/test.jpg`.

