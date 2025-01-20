.. _trouble:


Troubleshooting 
================

General Problems
----------------

**DDS_DIRECT does not not appear**

* Cut the power and reconnect
* Turn on/off your device's wifi a couple of times
* Connect HDMI to a monitor and see if OS is running. If OS is running and the wifi icon on the top-right corner is showing 'Could not communicate with wpa_supplicant', your WiFi setup is broken. This is currently an issue with V1.0.0. 

    You have two options.
    
    1. If you don't have the HDMI cable and can't see if it is your case, simply running the system recovery will solve the problem.
    
    2. If you already confirmed the problem, open the commandline window and type the following two commands.
    
    Wifi reactivation commands:
    ::

        sudo systemctl enable dhcpcd
        sudo service dhcpcd restart

* Reassemble the housing - wifi signal related problem might disappear


**Video is too slow or there are severe lags**

* Try to get closer to the device. 
* Try other USB cable
* Try other power source

**Not able to connect**

* Cut the power and reconnect
* Turn off and on the device's WiFi a couple of times
* Try the system recovery

**DDS_DIRECT is connected but astroid.local is not found**

This occationally happens especailly when you run the system for long time (at least a couple of hours). It is simply the host name astroid is not visible. 

* Most of the time, rebooting the system solve this problem. 
* If you are connected through DDS_DIRECT, try 10.10.10.10 instead of astroid.local. If Astroid is connected to a router, go to router setting page and find the list of the connected devices. Find the IP address of your Astroid and use that IP to access the Astroid web interface. 
* Try the system recovery
* This might be a camera problem especially if you drop the device while the lens is fitted. Contact us for more information. 

**RPi is dead. No monitor signal. No power light. No reading light**



You have two options. If you are good at DIY, you can get a new RPi4 2GB model and fit that in. You just need to get a new license codes from us. Just get us your serial number, your name and we will issue a new license for you.

The second otpion is sending your Astroid to us. But you need to pay the shipping if the warrenty has over. 



eFinder Problems
----------------

**Sky recognition is too slow or not working**

* Normally the sky recognition takes 0.1~2 seconds
* Adjust the Gain a bit higher or lower
.. figure:: /images/gain_adjust.png
   :alt: Finder align 
   :align: center

* Point the camera to a direction where no cloud, moon, building exists
* Check your lens focus
* Try other USB cable
* Try other power source
* Check if your license is properly appear on the system info window. If not register it again. Let us know if don't know your eFinder License code.
* Run the lens calibration 
* Check the thermal grease is properly spread (DIY kit only)

**Color balance looks incorrect**
The color balance of Astroid is fixed to natural light condition. If you have some light source it might show an unbalanced color.

EAA Stacker Problems
--------------------

**Tone curve adjust is not working on a mobile device**
This is a bug. It will be fixed in the next update.



Dr. Pole Problems
--------------------


