# INFORMATION ASSURANCE - FINAL PROJECT

By:
* Portanova, Mel Christopher B.
* Neri, Rodelyn O.
* Panizal, Baby Jean R.
* Reblando, Rio joy J.  
BSCS - 3B


## STEP-BY-STEP PROCEDURE

### 1. Installing Headless Raspbian OS into Raspberry Pi  

* First download the imager in this link -> [Raspberry Pi Imager](https://www.raspberrypi.com/software/) <img src="img\1.png" alt="1.png">

* After downloading the imager run the <img src="2.png" alt="2.png"> as administrator.

* After running the Rasberry Pi installer this will show up then click Install and wait for it to finish.<img src="img\3.png" alt="3.png"> 

* Once the installation is finished just click finish and the Raspberry Pi Imager will run
  <img src="img\4.png" alt="4.png">

* This is the Rasberry Pi imager this is where the installation of raspbian os starts by setting up the Pi device, OS, and your selected storage device (SD card).  
 <img src="img\5.png" alt="5.png">

 * On Raspberry Pi device we will be using Raspberry Pi 3  
   <img src="img\6.png" alt="6.png">

 * On Operating System we will be using Raspberry Pi OS (Legacy) 
   <img src="img\7.png" alt="7.png">

 * On selecting storage use the SD card you plugged and after you choose a storage device click next.
   <img src="img\8.png" alt="8.png">

 * Clear the settings to set it to default
   <img src="img\9.png" alt="9.png">

 * After clearing the settings click Edit Settings. you set the hostname to your own wish but I left into default raspberry pi, set a user name and password, wireless LAN that you want to connect, and locale settings Manila's timezone. And now we're finished in General settings.  
   <img src="img\10.png" alt="10.png">

 * Moving to Serices enable or chekc the SSH and click on Use password authentication then click save.
   <img src="img\11.png" alt="11.png">

* Now we're finished setting up the custom settings then you may now click yes to proceed to the installation.  
   <img src="img\12.png" alt="12.png">

 * A warning will pop up after clicking yes saying all data on your sd card will be wiped out. click yes to proceed to installations of OS.  
   <img src="img\13.png" alt="13.png">

 * Wait for the installation.  
   <img src="img\14.png" alt="14.png">

 * After the Verification is finished this wil pop up and you may now remove the sd card from your computer and insert it into Rasberry Pi 3.   
   <img src="img\15.png" alt="15.png">


### 2. Connect to Raspberry Pi via SSH then update the OS


* To connect the Raspberry PI via SSH first we open command prompt as a administrator then enter the command ssh YourUsername@TheIPaddress ->
**ssh admin@192.168.1.9** then enter the password that you created from customization settings.

* After entering the password successfully enter these commands to update.
  * sudo apt update
  * sudo apt upgrade


### 3. Install LAMP Stack


* To install the LAMP stack properly refer to this tutorial [Link 1](https://ostechnix.com/install-apache-mysql-php-lamp-stack-on-ubuntu-18-04-lts/) and [link 2](https://linuxhint.com/install-phpmyadmin-raspberry-pi/) to install without errors 

* These are the commands to be entered on by one by one after one installation is finished.
  * sudo apt install apache2
  *  sudo apt install mariadb-server
  * sudo mysql_secure_installation
  * sudo apt install php libapache2-mod-php php-mysql
  * sudo apt-get install php*
  * sudo apt install phpmyadmin


### 4. Connect to Raspberry Pi via VNC

  
* First download RealVNC Viewer from this link [RealVNC](https://www.realvnc.com/en/connect/download/viewer/) and install.

* To be able to connect to the Raspberry Pi via VNC you have to enable the graphical remote access on Raspberry Pi Software Configuration Tool by entering this command **sudo raspi-config** on the raspberry pi's command line.

  * To enable the graphical remote access select **System Options**.  <img src="img\17.png" alt="17.png">
  
  * Then select **I3 VNC** then from there you can now enable the graphical remote access.  <img src="img\18.png" alt="18.png">

* also before you can use RealVNC viewer you need to create an account. To create an account run the RealVNC viewer and there will be a login pop up click the **"Don't have an account?"** then you may create your account there.  <img src="img\16.png" alt="16.png"> 

* After successful login enter the IP address on the search bar to connect to Raspberry Pi and be able to control the raspberry pi from your pc.  
<img src="img\19.png" alt="19.png">
