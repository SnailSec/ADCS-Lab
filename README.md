# ADCS-Lab
This repository contains all the necessary files/links to set up ADCS in a lab environment. While the basic setup instructions and configuration files are provided here, detailed explainations, tutorials, and demonstrations are going to be made available on the SnailSec youtube channel.

The lab currently contains following ESC (Escalation) vectors:
  * ESC1
  * ESC2
  * ESC3
  * ESC4
  * ESC7
  * ESC8

**IPs**
|VM|IP|
|---|---|
|DC-01|10.10.10.100|
|DC-02|10.10.10.101|
|Kali|Dynamic-IP|

## Steps to install
* Download the zip containing VM's from releases
* Extract the zip
* Edit vmnet2 in the network settings of VMware Workstation. Goto Edit -> Virtual Network Editor
  ![Edit](https://github.com/SnailSec/ADCS-Lab/assets/168891917/245a98db-bfe5-4636-8720-66c1e567010a)
* Select VMnet2 and click on "Change Settings". Ensure that the Subnet IP is : 10.10.10.0
  ![Change VMnet2 Subnet](https://github.com/SnailSec/ADCS-Lab/assets/168891917/18b83100-d984-40de-8281-0ab468269075)
* Open the "SnailSec ADCS" Folder which has been extracted from the zip
* Import each machine by going into the machine's folder and double clicking on the .vmx file
  ![Import VM](https://github.com/SnailSec/ADCS-Lab/assets/168891917/25b0a000-aa0a-4e45-abd9-fae92e16cbfe)
* After importing each VM. Select the vm and goto "Edit virtual machine settings" -> Add -> Network Adapter -> Custom -> VMnet2 (Host-Only)
  ![Add Custom Network Adapter](https://github.com/SnailSec/ADCS-Lab/assets/168891917/50ac5b3b-4300-406e-9c82-59d18a361106)
* Start all 3 VM's and enjoy!
