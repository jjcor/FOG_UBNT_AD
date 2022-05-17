# Install FOG on UBUNTU 20.04, Windows DHCP, one network card.
## Installation
### Install Ubuntu
Install as usuall, create a user,configure fixed ip network, timezone...
Update packages
``` {.bash}
sudo apt get update && sudo apt dist-upgrade -y
```
Install some packages
``` {.bash}
sudo apt install unzip
```
### Install FOG
``` {.bash}
wget https://github.com/FOGProject/fogproject/archive/master.zip; unzip master.zip
```
``` {.bash}
cd fogproject-master/bin/
```
``` {.bash}
./installfog.sh
```
Select Choice 2.
Installation mode normal, select N
All N, Exceo the last thas ask you to accept all.

``` {.bash}
* Here are the settings FOG will use:
 * Base Linux: Debian
 * Detected Linux Distribution: Ubuntu
 * Interface: ens192
 * Server IP Address: 172.16.204.18
 * Server Subnet Mask: 255.255.252.0
 * Server Hostname: servername
 * Installation Type: Normal Server
 * Internationalization: 0
 * Image Storage Location: /images
 * Using FOG DHCP: No
 * DHCP will NOT be setup but you must setup your
 | current DHCP server to use FOG for PXE services
  * On a Linux DHCP server you must set: next-server and filename

 * On a Windows DHCP server you must set options 066 and 067

 * Option 066/next-server is the IP of the FOG Server: (e.g. 172.16.204.18)
 * Option 067/filename is the bootfile: (e.g. undionly.kpxe)
```
A the middel of the install ask you to go your webbrowser to this address and update/create database.
``` {.bash}
 http://172.16.204.18/fog/management
```
Push the button.
Back to the installation process and press Enter
Whait until install is done.
``` {.bash}
* Setup complete

   You can now login to the FOG Management Portal using
   the information listed below.  The login information
   is only if this is the first install.

   This can be done by opening a web browser and going to:

   http://172.16.204.18/fog/management

   Default User Information
   Username: fog
   Password: password
```

## Configuration
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec orci turpis, egestas ac ante in, scelerisque condimentum turpis. Quisque elementum enim ut urna sodales fringilla. Quisque ipsum nulla, rhoncus in diam ac, dignissim finibus nunc. Maecenas scelerisque laoreet dui, eget ultrices arcu sagittis at. Vestibulum lacus est, consectetur vitae mi scelerisque, aliquam varius purus. Praesent scelerisque, lacus vel
convallis varius, tortor diam efficitur elit, non tempor magna erat sit amet erat. Curabitur accumsan rhoncus euismod. Fusce a augue quam. Nullam malesuada tellus ac dolor sagittis tempus. Curabitur eleifend sodales lorem, vitae convallis ligula imperdiet id. Mauris malesuada sapien elit, ut fermentum lectus posuere in. Phasellus in semper odio. Donec convallis aliquet nisl, in elementum mauris scelerisque at. Mauris gravida tortor in magna sollicitudin, in euismod metus varius. Proin rhoncus convallis faucibus. Praesent egestas efficitur eros in aliquam.
