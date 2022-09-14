# Awesome Fedora Server

Fedora Linux Server Guide  
  
    Fedora Server is a short-lifecycle, community-supported server operating system 
    that enables seasoned system administrators, experienced with any OS, 
    to make use of the very latest technologies available in the open source community.  

### Overview  

[Fedora Server](https://getfedora.org/en/server/)

### Download  

[Download Fedora Server](https://getfedora.org/en/server/download/)

### Docs  

    Fedora Server provides a stable, flexible and universally adaptable basis 
    for the everyday provision of digital services and information, 
    suitable for use by all kinds of organizations and individuals. 
    
    It is based on the latest technology and as such, 
    brings the most modern environment to users as early as possible.  
      

[Fedora Server Docs](https://docs.fedoraproject.org/en-US/fedora-server/)  
    
### DNF Package Manager

DNF is the default package manager for RPM-based Linux distributions such as Fedora.

[Fedora Quick Docs - DNF](https://docs.fedoraproject.org/en-US/quick-docs/dnf/)  
[DNF Docs](https://dnf.readthedocs.io/en/latest/command_ref.html)  
[DNF - Fedora Magazine](https://fedoramagazine.org/tag/dnf/)  
[Using DNF (Mageia)](https://wiki.mageia.org/en/Using_DNF)  
    
Example : Installing Vim with DNF    

    sudo dnf install vim-enhanced
    
### Modularity

[Modularity Overview](https://docs.pagure.org/modularity/)  
[Modularity Docs](https://docs.fedoraproject.org/en-US/modularity/)  

Get a list of available modules to install :  

    dnf module list
    
List a specific module :  
 
    dnf module list mysql  

Install a module :  
    
    sudo dnf module enable mysql:8.0 -y
    sudo dnf module install mysql:8.0/{server,client} -y


### SELinux

Fedora Server ships with SELinux enabled.  

[Getting started with SELinux](https://docs.fedoraproject.org/en-US/quick-docs/getting-started-with-selinux/)

Get current mode ( enforcing, permissive, disabled ):  

    getenforce

### Firewall

Firewalld is the default network firewall.  
This may be fine for your home server when protected by a router.  

[Firewalld](http://firewalld.org)

For a production server, Config Server Firewall (CSF) provides a much higher level of security by default.  

    CSF is a Stateful Packet Inspection (SPI) firewall, 
    Login/Intrusion Detection and Security application for Linux servers.

[Config Server Firewall](https://www.configserver.com/cp/csf.html)

There is no official rpm for installing CSF. 
Follow the instructions to download the install script to get started.


### Control Panel

Cockpit is a web-based graphical interface for servers :  
[Cockpit](https://cockpit-project.org/)  

Webmin is a web-based interface for system administration :  
[Webmin](https://www.webmin.com/)  

Webmin provides a gui for managing CSF.  



