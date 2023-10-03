# SSH SETUP

## # RPI CUSTOM INSTALLATION

Certainly! Setting up a Raspberry Pi with a custom installation involves several steps. Here's a step-by-step guide to help you get started:

**`Step 1: Gather Your Hardware`**
Make sure you have the following items:
- Raspberry Pi board (any model)
- MicroSD card (8GB or larger)
- MicroSD card reader
- Power supply
- Monitor, keyboard, and mouse (for initial setup)
- An internet connection (via Ethernet or Wi-Fi)

**`Step 2: Download the Operating System`**
1. Visit the official Raspberry Pi website (https://www.raspberrypi.org).
2. Go to the "Downloads" section.
3. Download the latest version of Raspberry Pi OS lite for win64.



**`Step 3: RUN IMAGER`** (MENDATORY)

**set username password and device name**

 1. ENABLE ssh
 2. wifi configure
 


**`step 4: WRITE`**

select sd card and write it.

## # SET WIFI USING TERMINAL ON RPI

        sudo iwlist wlan0 scan

if error occured - wlan0     Interface doesn't support scanning : Network is down

1. sudo ifconfig wlan0 up 
error - operation not possible due to RF-kill 

        rfkill list

unblock the device 

        sudo rfkill unblock wifi


#### open configure file for set wifi ssid and password

    sudo nano /etc/wpa_supplicant/wpa_supplicant.conf

![Alt text](image.png)

save it.

> sudo reboot

> ifconfig wlan0

> ifconfig eth0
