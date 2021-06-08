# ADB, RASPI, AND OTHER COOL STUFF I tried to do

Step 1: installing raspbian headless on RASPI 4
  Basically flashed and sd card
  
  added a file called ssh (no extension) into the boot [activates ssh]
  
  added a file called wpa_supplicant.conf [connects to wifi]
  
  Boot the pi and wait for the pi to load
  
  On another computer open ssh and connect to pi@raspberry.local
  
  Done
 
Step 2: ADB on raspbian
  
  sudo apt-get install android-tools-adb android-tools-fastboot
  
  test the installation using command using "adb" and "adb start-server"

Step 3: Android Phone
  
  Go to system info, tap on the IMEI serial until it activates developer mode
  
  Go to developer menu and activate adb through usb debugging

Step 2 Part 2: 
  
  For python library, I used pure-python-adb
  
  pip install pure-python-adb
  
  Start server using "adb start-server" first, python will not work without this 
  
Step 4: OPENCV

  I followed this site: https://www.pyimagesearch.com/2019/09/16/install-opencv-4-on-raspberry-pi-4-and-raspbian-buster/
  


Other Notes: I have been trying to remote desktop into the PI4 using XRDP. After the initial setup, the PI4 fails to work on both ssh and remote desktop. The best solution I could think of is to avoid remote desktop and the initial installation boot menu altogether. All development will be done remotely via ssh and vscode's ssh capabilities.
  
  
