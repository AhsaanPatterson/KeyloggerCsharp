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
<p align="center"> 
Step 6: Create Delegate for Keyboard Callbacks
</p>
</br>
Define a delegate for the keyboard hook procedure
<br/>
<img src="https://imgur.com/L0JMZGd.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<p align="center"> 
Step 7. Implement the Hook Callback Method
</p>
</br>
Create the HookCallback method to handle the key events:
<br/>
<img src="https://imgur.com/9UrKzC6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
<p align="center"> 
Step 8: Write Logic to Handle Different Keys
</p>
</br>
Inside the HookCallback, implement the logic to log specific keys (like OemPeriod, Oemcomma, Space, etc.) to a text file:
<br/>
<img src="https://imgur.com/nkYFdLX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br/>
<p align="center"> 
Step 9: Set the Low-Level Keyboard Hook
</p>
</br>
Implement the SetHook method to set up the keyboard hook
<br/>
<img src="https://imgur.com/R0iJVMQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<p align="center"> 
Step 10: Import Windows API Functions
</p>
</br>
Below your class definition, use [DllImport] to import required functions from the Windows API
<br/>
 <img src="https://imgur.com/gVoveGi.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

<p align="center"> 
Step 11: Compile and Run the Program
</p>
</br>
Save your code and compile the project.
Run the program, and it should start logging keystrokes to C:\ProgramData\mylog.txt.
Do not run the program on your home pc, please use a virtual lab when running
</br>

Important Notes:
 <br/>
 Ethical Considerations: Keyloggers can be misused for unethical purposes. Ensure you have permission to log keystrokes and comply with applicable laws.
Administrative Privileges: You may need to run the application with administrative privileges, depending on the system settings.
 <br/>

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
