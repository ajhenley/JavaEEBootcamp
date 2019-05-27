# Obtaining the Oracle Virtual Machine

## Obtaining the software for this course

Oracle makes a virtual appliance for VirtualBox that runs all the software needed for this course. Once you have VirtualBox installed you can run the appliance and then install Eclipse and git.

This software is provided by Oracle. There is no cost to download and use this software. However, you will need to register at Oracle's website to access the download page.

## Obtaining VirtualBox

Vist [https://www.virtualbox.org/wiki/Downloads](https://www.virtualbox.org/wiki/Downloads) and download the version for your computer. You will have a much better experience if you have at least 8 Gb RAM installed and sufficient space on your hard drive. The Virtual appliance we will download takes up a lot of disk space.... almost 80 Gb. You'll need to have that much free after you've collected all your Game of Thrones episodes and Adele songs and videos. You'll really want more space after that. The good news is that the virtual machine can be hosted on a USB drive \(newer is faster and therefore better\).

Are you trying to develop on a hand-me down laptop that you know should be replaced? You really need to question your dedication to the task. You can obtain all the software for becoming a super Java developer for free. Consider putting some money into good hardware. The limiting factors are mostly memory and hard disk size.

Still trying to become a Java developer using old hardware? It can be done. Install linux on that dusty old laptop and use MySQL or PostgreSQL as the database.

Ok, so you just don't have a laptop... there's still hope. Check out C9.io or [http://www.tutorialspoint.com/codingground.htm](http://www.tutorialspoint.com/codingground.htm).

## Back to Oracle

Follow the link below to download the Oracle Developer machine. It comes all set up with everything you need to get stated except git and Eclipse. Instructions for installing Eclipse are in the section of this book called "Developing with Eclipse".

The developer machine is almost 8 Gb large. Use a download manager to avoid downloading it multiple times.

## Link to download the Database App Developer Virtual Machine

[http://www.oracle.com/technetwork/database/enterprise-edition/databaseappdev-vm-161299.html](http://www.oracle.com/technetwork/database/enterprise-edition/databaseappdev-vm-161299.html)

Oracle wants you to know this virtual machine is appliance is for testing purposes only, as such it is unsupported and should not to be used in production environment. This virtual machine contains:

* Oracle Linux 7 \(based on Redhat\)
* Oracle Database 12c Release 1 Enterprise Edition \(12.1.0.2 with In-Memory Option\)
* Oracle SQL Developer 4.1.3
* Oracle Application Express 5.0

### After the download is complete and VirtualBox has been installed

Import your VM: File &gt; Import Appliance to launch Appliance Import Wizard. ClickChoose... to browse to the directory you re-assembled all the files in and select the OTN\_Developer\_Day\_VM.ova then click Next&gt; to begin importing the virtual machine. It will prompt you to agree to the appropriate developer licenses while importing. You will see 'Oracle Developer Days \(Powered Off\)' when it is finished importing.

Finally, Test your VM: Once the import has completed, double-click the OTN Developer Days VM. Click OK to close the Virtualbox Information dialogs. When you get to the Enterprise Linux 6 screen you can now login. \(Username and password is oracle.\) Allow the process to complete; it is ready when you see a terminal window, which you can close. Once you are finished working in the guest VM you can shut it down via System &gt; Shut Down; this will return the guest VM to the Powered Off state.

