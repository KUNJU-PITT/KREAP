# [](#header-1)Download the KREAP VM

Download the [KREAP](https://bioinf-galaxian.erasmusmc.nl/owncloud/index.php/s/BWlikRC5dXNHdK0/download) VM.

## [](#header-2)Extract the zip

The downloaded file is a zip archive, which has to be unpacked.  

### [](#header-2)Windows

Unpack the zip with an archiving tool, 7-zip is used here, but use what ever is available:  
![virtualbox setup 1](img/setup_kreap_unpack_windows.png)  

### [](#header-3)Mac

Unpack the zip \<---------------the mac way-------------------\>:  
![virtualbox setup 1](img/setup_kreap_unpack_mac.png)  

### [](#header-3)Linux

With the many flavours of Linux, it's difficult to cover every one of them, but most come with support for many different types of archives.  
Here is an example of what it would look like in Kubuntu:  
![virtualbox setup 1](img/setup_kreap_unpack_linux.png)  

## [](#header-2)Import KREAP into VirtualBox  

Open VirtualBox and click on "New" (top left), fill in a name for the VM, select Linux as a "Type" and "Ubuntu (64-bit)" as Version and click "Next":
![virtualbox setup 1](img/setup_kreap1.png)  
  
Select the ammount of memory that should be available to KREAP, at least 4096MB is recommended, but KREAP should still run with less.  
It is recommended to stay within the suggested (green) area, this is dependent on the computer that VirtualBox is installed on:  
![virtualbox setup 1](img/setup_kreap2.png)  
  
Select "Use an existing virtual hard disk file" and click on the "Choose a virtual hard disk file..." button:
![virtualbox setup 1](img/setup_kreap3.png)  
  
Navigate to the unpacked KREAP VM and open it:  
![virtualbox setup 1](img/setup_kreap4.png)  

Click on create:  
![virtualbox setup 1](img/setup_kreap5.png)  
  
You will be back at the main VirtualBox screen, but now with the KREAP VM ready to go:  
![virtualbox setup 1](img/setup_kreap6.png)  
  
Right click on the newly created KREAP VM and select "Settings":  
![virtualbox setup 1](img/setup_kreap7.png)  
  
In the settings of the KREAP VM, select "Network", click "advanced" and then "Port Forwarding":  
![virtualbox setup 1](img/setup_kreap8.png)  
  
Click on the green "+" icon on the right side of the window, fill in a name for the new rule and "8080" for the "Host Port" and "8080" for the "Guest Port":  
![virtualbox setup 1](img/setup_kreap9.png)  
  
Now it's finally time to start the KREAP VM, Click "OK" to accept the new Port forwarding rule and "OK" again to accept the new settings.  
Select the newly created KREAP entry and click on "Start" (green arrow) at the top, after a while you will see the following screen:  
![virtualbox setup 1](img/setup_kreap10.png)  

Open up your favourite webbrowser and go to [127.0.0.1:8080](http://127.0.0.1:8080), you should see the KREAP Galaxy main page:  
![virtualbox setup 1](img/setup_kreap11.png) 

# [](#header-1)Create a Plate zip and index  
  
Learn more about the Plate zip and index file that are used as inputs for KREAP [here](file_formats)