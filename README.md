
![IMX477 Camera Module](https://www.inno-maker.com/wp-content/uploads/2023/12/InnoMaker_12.3MP_HQ_Camera_Module_IMX477_CMOS_Sensor_Raspberry_Pi_Jetson_Nano_CS_C_Lens_Compatible_with_Raspberry_Pi_HQ_Camera_02.jpg "IMX477")


## Quick Start For Raspberry PI Series
#### Step1, Modify config.txt
- sudo nano /boot/config.txt
  - For the latest version raspberry Pi OS, it should be
- sudo nano /boot/firmware/config.txt

#### Step2, Add below content to the last line
- dtoverlay=imx477

#### Step3, Reboot and use below command to preview
- libcamera-hello -t 0

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