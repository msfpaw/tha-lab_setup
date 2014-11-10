Hacker Academy
==============
http://hackeracademy.com

### THA LAB SETUP

#### Purpose
This lab will walk you through the steps required to set up the local testing environment required to complete the labs found at hackeracademy.com

#### Requirements
This lab requires the following applications to be installed
* virtualbox or vmware 
* vagrant

#### Setup
The THA lab environment supports Virtualbox and VMware has been tested with Windows, OS X, and Linux hosts.

##### NOTE
*Using VMware with Vagrant requires the purchase of a plugin from the developers of Vagrant so if you plan on using VMware to complete your THA labs you must first purchase the [plugin](https://www.vagrantup.com/vmware).
The following steps assume that you are either using Virtualbox or have purchased and installed the VMware plugin from hashicorp.*

1. Download and install Vagrant from [here](https://www.vagrantup.com/downloads.html).

2. Download and install Virtualbox if you haven't already done so. [Virtualbox.org](https://www.virtualbox.org/wiki/Downloads)
  * If you are using VMware then you do NOT need to install Virtualbox and can skip this step.

3. Download the THA [Vagrantfile](https://github.com/madsec/tha-lab_setup/raw/master/assets/Vagrantfile).

4. Move the Vagrantfile to a directory you will use to store your lab VMs.

5. Open a terminal and make sure you're in the same directory as the Vagrantfile, then launch your Kali VM by entering the following command:

  ```
  vagrant up kali
  ```

* The above command will download the Kali VM and launch it via Virtualbox.

6. Clone this repo on your Kali VM by opening a terminal and issuing the following command from the Kali VM:

    ```bash
    git clone git://github.com/madsec/tha-lab_setup /root/THA/setup
    ```

##### Note
* If the Kali VM network connection continually disconnects please reboot the VM.

#### Start the lab
* Follow the instructions for lab 1 found on your Kali machine at 
  ```
  /root/THA/setup/lab1.md
  ```
