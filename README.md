
![alt text](https://github.com/INNO-MAKER/cam-imx477/blob/main/images/477.jpg)


## Quick Start For Raspberry PI Series

#### Step1, Modify config.txt
- sudo nano /boot/config.txt
  - For the latest version raspberry Pi OS, it should be
- sudo nano /boot/firmware/config.txt

#### Step2, Add below content to the last line
- dtoverlay=imx477

#### Step3, Change camera_auto_detect=1 to
- camera_auto_detect=0

#### Step4, reboot and preview
- libcamera-hello-t 0
- 
#### More information
- [https://www.raspberrypi.com/documentation/computers/camera_softwarehtml](https://www.raspberrypi.com/documentation/computers/camera_softwarehtml)



## Quick Start for Nvidia Series
#### Step 1: Open the terminal and execute the following

- sudo /opt/nvidia/jetson-io/jetson-io.py
#### Step 2: Select Configure Jetson Nano CSI Connector
#### Step 3: Select Configure for compatible hardware
#### Step 4: Select the camera that you want to use
- Camera IMX477 DUAL
#### Step 5: Select Save pin changes
#### Step 6: Select Save and reboot to reconfigure pins
#### Step 7: Press any key on the keyboard and the device will reboot with the applied camera configuration

## For CAM0 port
- nvgstcapture-1.0 sensor-id=0

## For CAM1 port
- nvgstcapture-1.0 sensor-id=1