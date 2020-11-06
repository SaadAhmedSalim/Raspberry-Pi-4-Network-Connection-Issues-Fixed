# Raspberry-Pi-4-Network-Connection-Issues-Fixed

Hello Everyone!

Today I will discuss about the common problem that we faced when we want to connect raspberry to a network (Wireless or Wired).

<b>That means You can connect your pi without a monitor or cable thing!</b>

There will be lots of videos and documentation about these problems but not with proper solutions!

<b>Before looking my solutions, I want to make a clear statement that you have to enable your pi ssh and vnc. 
After that anywhere you go, just with your pi and laptop, you can control your pi through laptop without a monitor or cable.
</b>

Here is my advice for you guys but you need some tools for that !

<h3>REQUIREMENTS:</h3>

    1. Windows operating system based Laptop or PC
    
    2. Wireless router
    
    3. Ethernet cable 
    
    4. Putty + VNC (Download these software)
    
    5. Raspberry PI with power cable.
  
  
<b>For these solution I have used Raspberry Pi 4 (1GB).</b>

<h3>Steps:</h3>

1. Connect Ethernet cable's one head in Raspberry pi port and other head in the router.

2. Power up the pi source and Check your router main page. (Example: my router is tp-link so my address is 192.168.0.1)

3. Log in your router.

4. There will be a option called DHCP.

5. Here, you will find your host name: raspberry pi with an ip address.

6. Turn on Putty and put that ip address in the gap, port is same 22.

7. It will connect automatically, (If there is an security alert message shown, just click YES)

<h4>Notes: Some cases it wants user name and password. </h4>
  
<b>So, username is pi and password is raspberry</b>

If you want to change password manually ,

<div><p>
So the first thing to do is change the password. This can be done via the raspi-config application, or from the command line.

    sudo raspi-config

Select option 2, and follow the instructions to change the password.

In fact, all raspi-config does is start up the command line passwd application, which you can do from the command line. Simply type in your new password and confirm it.

    passwd
</p>
</div>
  
8. Then open VNC, put the address in that (e.x: mine was 192.168.0.106)

9. It will show your pi environment.

<b>Note:</b>

Using putty you can do terminal code in pi. It's easy and smooth way to learn pi.

<h3>How to make a WIRELESS Connection</h3>

I have seen many were trying terminal and maximum cases, they failed, as there are lots of dependencies. Mine is simple and easy. I hope it will work for all!

<b>Launch PI terminal (ctrl + alt+ T) </b>

    sudo raspi-config
    
    select network option
    
    add your wifi name
    
    add your password
    
<b>ENJOY WIRELESS MODE</b>

<h4>Note: Remember! All these things must have to do under wired connections!</h4>

<h3>IN MY CASE THERE WAS A RESOLUTION ISSUE</h3>

I fixed that too.

For that 

<b></b>There are many solutions:

Launch pi terminal. If you use putty you can do there too.
  
    sudo raspi-config
    
There will be so many option. For PI-4, click on ADVANCED SETTINGS
  
    select resolution
  
There will be your desire size, just pick one.

Reboot the PI. <b>Problem Solved!</b>


Further details will be uploaded soon.
