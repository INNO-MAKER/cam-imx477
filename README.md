## Quick Start For Raspberry PI Series

### Step1, Modify config.txt
- sudo nano /boot/config.txt
  For the latest version raspberry Pi OS, it should be
- sudo nano /boot/firmware/config.txt

### Step2, Add below content to the last line
  dtoverlay=imx477

### Step3, Reboot and use below command to preview
- libcamera-hello -t 0

## More information please see [https://www.raspberrypi.com/documentation/computers/camera_softwarehtml](https://www.raspberrypi.com/documentation/computers/camera_softwarehtml)mark