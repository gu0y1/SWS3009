---
description: Debugging Material for Day 4 (Released on 5 July 2024)
---

# Day 4: Everything Together

## Install Arduino IDE on RPi

Install the Arduino IDE on a Raspberry Pi 4 running Raspbian 12 Bookworm:

#### 1. Update Your System

First, make sure your system is up to date. Open the terminal and run the following commands:

```sh
sudo apt update
sudo apt upgrade
```

#### 2. Install Dependencies

Before installing the Arduino IDE, ensure that some necessary dependencies are installed:

```sh
sudo apt install -y curl wget tar
```

#### 3. Download the Arduino IDE

Download the latest version of the Arduino IDE from the official Arduino website. You can use the following command:

```sh
wget https://www.comp.nus.edu.sg/~guoyi/tutorial/cg2111a/wget/arduino-1.8.19-linuxaarch64.tar.xz
```

#### 4. Extract the Files

Once the download is complete, extract the downloaded file:

```sh
tar -xf arduino-1.8.19-linuxaarch64.tar.xz
```

#### 5. Install the Arduino IDE

Navigate to the extracted directory and run the installation script:

```sh
cd arduino-1.8.19
sudo ./install.sh
```

#### 6. Launch the Arduino IDE

After the installation is complete, you can launch the Arduino IDE with the following command:

```sh
arduino
```

Alternatively, you can find the Arduino IDE in the application menu of your desktop environment and launch it from there.

#### 7. Add User to dialout Group

To allow the Arduino IDE to access serial ports, you need to add the current user to the `dialout` group:

```sh
sudo usermod -aG dialout $USER
```

Then, log out and log back in, or run the following command to apply the changes:

```sh
newgrp dialout
```

You should now be able to successfully run the Arduino IDE on your Raspberry Pi 4!
