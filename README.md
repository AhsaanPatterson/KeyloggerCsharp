<h1>Step-by-Step Guide to Create a Keylogger in C#</h1>


<h2>Description</h2>
This lab will cover dives into the technical aspects of a keylogger written in C# for windows and is intended for educational purposes only.

<h2>Languages and Utilities Used</h2>

- <b>Microsoft Visual Studio</b> 
- <b>Oracle Virtual Box</b>

<p align="center">
Create a Keylogger in C#

<p align="center"> 
Step 1: Install Visual Studio (Community edition is free).
</br>
Create a new Console Application project in C#.
<br />
<br />
<p align="center"> 
Step 2: Add Necessary Namespaces
</br>
At the top of your Program.cs, include the following namespaces to access necessary classes and functions:
 <br/>
<img src="https://imgur.com/XiPycxv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />

<p align="center"> 
Step 3: Define the Program Namespace and Class
</br>
Define your namespace and class in the project
<br/>
<img src="https://imgur.com/zsoyQ8q.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<p align="center"> 
Step 4: Define Constants and Hook Variables
</p>
</br>
Inside the Program class, declare necessary constants and variable that will be used for setting the keyboard hook:
 <br/>
<img src="https://imgur.com/cfxennm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<p align="center"> 
Step 5: Implement the Main Method
</p>
</br>
Create the Main method where you'll set the hook and run the application:
<img src="https://imgur.com/rjtUNV8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
Step 6: Setup Virtual Machine
Open VirtualBox.
Select create a Virtual Machine.
With this Virtual Machine you want to name it Client1 and the type Windows and version Windows 10 (64-bit).
Next you would want to set the hardware memory to 2096 MB if your computer allows that.
Click next on the following screens until you see the VM created.
Before starting right click on Client1 go to advanced settings and turn on these two options.
Go to the processor and if your computer allows it, change it to 4 CPU.
After finding your network tab and modify it to NAT  then press ok.

<br/>
<img src="https://imgur.com/rkAxWLu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/jZuJcs9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/eq0Z65Y.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/lfa06LN.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/5iPtnBC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/Xgz1K9K.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Step 6. Double tap on your Virtual Machine to start it.
You will receive this message at first prompting you to paste the path where Windows 2019 ISO is downloaded at.
Once you have added the ISO you can select the “Mount and Retry Boot” option.
Depending on your PC it may take some time for the installation to begin.
<br/>
<img src="https://imgur.com/PdchRYM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Step 7: Next you want to double click on Client1 and locate the Windows10 ISO file downloaded earlier.
Wait a little time for the installation to be completed and press next until you receive.
You want to select the option if you do not have a license key.
Select the option Windows 10 Pro.
Next you want to select the custom option for installation type and press next to install.
Installation may take some time to complete after a while you will receive the following screen.
Select your keyboard layout.
Next option you would select “I dont have internet”.
You want to choose “Continue with limited setup”.
Type user as your account name.
You can unselect each option to help speed up time.
You can select the not now option for Cortana.

<br/>
<img src="https://imgur.com/L6PvezF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/xIX95xB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/30J9dZt.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/n6FKGbO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/EvNIb7x.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/j5akPcB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/gHYiIOG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
Step 8: Configure your default admin password’
<br/>
<img src="https://imgur.com/SSg5IAj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>



Step 9: Press Control Alt Delete for the newly installed Windows
 <br/>
 <br/>
 <img src="https://imgur.com/DpbVKH5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

Step 10: Import CD Guest Additions
Next you want to open File Explorer inside of Virtual Machine.
After you want to click on the selected program to run amd64.
For the next few options up to the finalization of installation select next for default options.
 <br/>
 <br/>
 <img src="https://imgur.com/2t4sKvH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>[

Step 11: Click on the Reboot later option then manually shut down VM
 <br/>
 <br/>
 <img src="https://imgur.com/5J8BK2f.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>



Step 12: Log back into Virtual Machine and Prepare to configure IP address.
First, click on the network icon in the lower right hand corner.
Select the change adapter options.
Next select the first option right click on status then on details.
You want to point out the IP address.
If the IP address start with 10 then that is the correct 1st NAT option.
Now change the name of the 1st NAT to something like “Internet”.
Rename the 2nd NAT to something like “Internal”.

 <br/>
 <br/>
 
<img src="https://imgur.com/GEezSPK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


Step 13. We will rename the PC and restart the PC after this
 <br/>
 <br/>
 <img src="https://imgur.com/Xzam2Km.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>




Step 14. Configure IP address for NAT #2
Go to Network icon in bottom left hand corner.
Click on change adapter options.
Click on the Internal and press properties. 
Input the following address and select ok and ok after.
IP address 172.16.0.1
Subnet Masking 255.255.255.0
Preferred DNS Server 127.0.0.1
 <br/>
 <br/>
 <img src="https://imgur.com/fHNfoDI.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>



Step 15: Create an Domain
Search Server Manager
Click on “Add roles and manager”.
Click on next and next once you reach this screen pause.
Once you select your DC click next.
After you would select “Active Directory Domain Services”.
You will next, next, and then select Install.
Once the installation have completed close out this screen.
<br/>
<br/>
<img src="https://imgur.com/C6oWpGb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>




Step 16: Click on the notification at the upper right hand corner to begin “Post deployment Configuration”
Select “ Add a new forest” and input the name mydomain.com
Input a generic password on the next screen
Click on Next when you receive the Install option and select it
Once the installation is completed the VM will automatically restart
 <br/>
 <br/>
 <img src="https://imgur.com/jaTInQP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


Step 17: Once logging back in go to the windows home icon and find underneath Windows Admin Tools  for “Active Directory Users and Computers”.
Once inside of the Active Directory Users and Computers” you want to right click on mydomain.com -> New -> Organizational Unit.
Create _Admins organizational group and uncheck option.
Next you will right click on _Admins folder and select New -> User.
You want to choose your name and standard naming convention for username.
Select an generic password

  <br/>
  <br/>
  <img src="https://imgur.com/vZduLOW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>




Step 18: Right click on your user account and select properties.
Click on Members Of and select add.
You want to type in domain admins and press check names.
Then you want to apply and press ok.
  <br/>
<br/>

Step 19: Signout of the VM in order to login to newly created admin account
  <br/>
  <br/>
  <img src="https://imgur.com/Yqr6Uau.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>




Step 20: Create RAS/NAT
Search Server Manager and select “Add roles and features”.
Select next and then next, after that you want to add Remote Access.
Click next again two more times you should be able to select the feature Routing.
Click on next until you get the option to Install.
<br/>
<br/>
<img src="https://imgur.com/R2Ha3aG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


Step 21: Close out of the installation and select Tools -> Routing and Remote Access.
Right click on your DC and select Configure and Enable Routing and Remote Access.
Select next then you want to choose the option “NAT”.
You want to select the Internet option and finish the installation.
If no Network Interfaces appear you may want to close out and repeat step 21 a
After the installation is complete you should see this screen.
<br/>
<br/>
<img src="https://imgur.com/5UngmMf.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


Step 22: Setup DHCP server
Go back into Server Manager and select “Add roles and features”.
Click next, next and next until you receive the following screen and select DHCP.
Click next until you receive the install option.
ext you want to exit out of the installer and go to tools => DHCP.
Expand your DC and right click on one of the IPv4 or IPv6 -> New Scope.
Click next and input the following name 172.16.0.100.200
Input the following information for the next screen.
Start IP 172.16.0.100 End IP 172.16.0.200 and Subnet Mask 255.255.0.0
After you will hit next until you see the Configure DHCP options.
Next you want to enter the following IP address and make sure to select add before moving forward.
172.16.0.1
Next you want to proceed through until you see the installation.
You want to then right click on the DC and select Authorize.
After you want to right click on IPv4 and refresh.
<br/>
<br/>
<img src="https://imgur.com/tqnCJcM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


Step 23: Setup users via Powershell
Go back to Server Manager and select “Configure this local server”.
Click on Internet Explorer Ehanced Security Configuration and turn it off.
Open Internet Explorer and copy the following link https://github.com/joshmadakor1/AD_PS…
The link will automatically begin downloading the script files to create multiple users.
Save as the folder on your desktop and extract it. 
<br/>
<br/>
<img src="https://imgur.com/1JQ5WQP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/8yxTPci.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/e5I9D1Y.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

Open the folder and names file
After add your name to the top of the names file.
Open Windows Powershell ISE from the windows icon and run as admin.
Once inside of Powershell click on the folder icon to locate the folder downloaded with the create users script.
Once you see the script pulled up you want to type in the following command to allow scripts executable.
Set-ExecutionPolicy Unrestricted.
Select Yes to all after running script.
Next you want to enter the following command to change directories in order to run above script.
Cd C:\users\(AD name)\desktop\AD_PS-master.
At this point you can press the green play button and watch the users be created.
<br/>
<br/>

<img src="https://imgur.com/lBon7J5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/mjItyhP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/AbPKytc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/IgAsXRC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/BPKe4r7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/cV7lwBr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


Step 24: Confirm changes in Active Directory.
Next you want to go to the windows icon in the bottom left hand corner and select Windows Admin Tools -> Administrative Directory Users and Computers.
Next you want to refresh the DC (mydomain.com) and you should see the _USERS folder and all of the newly added users.
<br/>
<br/>

<img src="https://imgur.com/VMvoKXx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


Step 25: Create another new VM with Windows 10
Minimize your current VM and open VirtualBox.
Next you want to create a new Virtual Machine.
With this Virtual Machine you want to name it Client1 and the type Windows and version Windows 10 (64-bit).
Next you would want to set the hardware memory to 2096 MB if your computer allows that.
Click next on the following screens until you see the VM created.
Before starting right click on Client1 go to advanced settings and turn on these two options.
Go to the processor and if your computer allows it change it to 4 CPU.
After find your network tab and modify the NAT to internal then press ok.
<br/>
<br/>

<img src="https://imgur.com/rkAxWLu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/jZuJcs9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="(https://imgur.com/eq0Z65Y.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/lfa06LN.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/5iPtnBC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/hrgaQ7i.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>



Step 26: Next you want to double click on Client1 and locate the Windows10 ISO file downloaded earlier.
Wait a little time for the installation is completed and press next until you receive.
You want to select the option you do not have an license key.
Select the option Windows 10 Pro.
Next you want to select the custom option for installation type and press next to install.
Installation may take some time to complete after a while you will receive the following screen.
Select your keyboard layout.
Next option you would select “I dont have internet”.
You want to choose “Continue with limited setup”.
Type user as your account name.
You can unselect each option to help speed up time.
You can select not now option for Cortana.
<br/>
<br/>
<img src="https://imgur.com/L6PvezF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/xIX95xB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/30J9dZt.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/n6FKGbO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/EvNIb7x.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/j5akPcB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/gHYiIOG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


Step 27: Make sure Internet is connected
Open the command prompt by searching cmd.
Then enter the following command to pull up the ip addresses.
Ipconfig
If you do not see an Default Gateway be defined we must investigate from the Domain Controller.
Log back into your first VM.
Open DHCP
<br/>
<br/>
<img src="https://imgur.com/QLEHUpJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>


Expand out the domain controller.
Expand out IPv4 and double click on Server options.
After doing that you want to select more actions on the right hand plan.
The selection you want to choose is “Routing” and add the following IP address below 172.16.0.1
Next you want to right click on the domain controller -> All Task -> Restart<br/>
<img src="https://imgur.com/0PB7KMe.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://imgur.com/e9sripu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<br/>
Step 28: After going back to your second VM repeat the above step by typing in ipconfig
You should see the following 
<br/>
<br/>

<img src="https://imgur.com/H065XlV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>  






</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
