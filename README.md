# Lab Guide

---
### Access Pi device in Raspberry Pi Connect
Raspberry Pi Connect provides secure access to your Raspberry Pi from anywhere in the world.

1. Visit **https://connect.raspberrypi.com** on any computer
2. Sign in with your Raspberry Pi ID
   * Pi ID: **support@heswiki.com**
   * Password: ******
3. Select your device and connect it via screen sharing
4. Use your device as you use it locally with GUI interface
5. Open the Linux terminal and launch script for running your applications

---
### How to SSH into Raspberry Pi
Now that you have SSH enabled and you have the IP, you’re ready to SSH into your Raspberry Pi. The steps to do this will vary depending on whether you’re using Windows, Mac, or the Ubuntu Linux OS.

#### How to SSH into Raspberry Pi from Windows
There are many ways to SSH into a Raspberry Pi. In the following steps, we’ll show you how to do this using PuTTy (an open-source terminal emulator) or PowerShell. 


---
#### To SSH into your Raspberry Pi from PuTTy:
To SSH into your Raspberry Pi using PuTTy, follow these steps:

1. Download PuTTY (free SSH client for Windows): https://www.putty.org/
2. Open PuTTy in Windows
4. Under Host Name (or IP address), enter your Raspberry Pi’s IP address or hostname.
5. Make sure that Port is set to 22. If the Raspberry Pi SSH port is not set to 22, the connection will fail.
6. Under Connection type, select SSH.
7. Select Open, and enter your username and password.

---
#### To SSH into your Raspberry Pi from PowerShell
To SSH into your Raspberry Pi using PowerShell, follow these steps:

1. Open a terminal on the device you would like to SSH into your Raspberry Pi from.  
2. To open PowerShell, either press Ctrl + Shift + P, or hit the Windows key and manually search for PowerShell.
3. Enter the shell command in the terminal
```
$ ssh [username]@[IP address]
## Replacing [username] and [hostname] or [IP address] with the details of your Raspberry Pi as below
$ ssh demo@192.168.52.71 -X
```

---
#### To SSH into Raspberry Pi from Mac
To SSH into your Raspberry Pi from macOS:

1. Navigate to Applications > Utilities
2. Open the terminal and enter the shell command in the terminal
```
$ ssh [username]@[IP address]
## Replace[username] and [hostname] or [IP address] with the details of your Raspberry Pi as below
$ ssh demo@192.168.52.71 -X
```

---
#### To SSH into a Raspberry Pi from a Linux device:

1. Press Ctrl + Alt + T to open a terminal window
2. Enter the shell command in the terminal
```
$ ssh [username]@[IP address]
## replace [username] and [hostname] or [IP address] with the details of your Raspberry Pi as below
$ ssh demo@192.168.52.71 -X
```

---
#### To SSH into a Raspberry Pi device from Internet

1. SSH into the training server (111.251.210.138) with your training account (rx71)
2. SSH into the Pi device from training server with your user account (demo) on Pi device
```
$ sshpass -p rpi5demo ssh rx71@111.251.210.138 -X
$ sshpass -p rpi5demo demo@192.168.52.71 -X
```

---
### Available Pi devices in the cloud 

| Device | IP address | SSH to Pi Device | SSH to Server |
|:-|:-|:-|:-|
| rx71 | 192.168.52.71 | ssh demo@192.168.52.71 -X | ssh rx71@server -X |
| rx72 | 192.168.52.72 | ssh demo@192.168.52.72 -X | ssh rx72@server -X |
| rx73 | 192.168.52.73 | ssh demo@192.168.52.73 -X | ssh rx73@server -X |
| rx74 | 192.168.52.74 | ssh demo@192.168.52.74 -X | ssh rx74@server -X |
| rx75 | 192.168.52.75 | ssh demo@192.168.52.75 -X | ssh rx75@server -X |
| rx76 | 192.168.52.76 | ssh demo@192.168.52.76 -X | ssh rx76@server -X |


---
### Resource 
* Basic guide for Linux shell scripting: [[Github]](https://github.com/heslabs/rpi-llm-course/blob/main/00_Lab_Guide/Linux_Shell.md)
* Raspberry Pi Connect: [[Github]](https://github.com/heslabs/rpi-llm-course/blob/main/00_Lab_Guide/rpi-connect.md)
* Raspberry Pi Connect (Beta): https://www.raspberrypi.com/documentation/services/connect.html
* Download PuTTY - a free SSH and telnet client for Windows: https://www.putty.org/ 
