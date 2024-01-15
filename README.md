<h1>Active Directory Home Lab Guide</h1>


<h2>Description</h2>
In this guide we're going to walk throught how to create an Active Directory home lab enviroment using Virtual Box. Configuring and running throught this lab will definetly help develop your understanding of how Active Directory and Windows networking works, so I highly recommend running through it a couple of times, ask questions where stuff is unclear, and eventually try to build it on your own without needing this guide. Please let me know if you have any questions!
<br />


<h2>Environments Used</h2>

- <b>Windows Server 2022</b> 
- <b>Windows 10 Pro</b>

<h2>Project walk-through:</h2>

<p align="center">
First we are going to download a few things <a href="https://www.virtualbox.org/" target="_blank">Virtual Box</a>
, <a href="https://info.microsoft.com/ww-landing-windows-server-2022.html" target="_blank">Windows Server 2022 ISO</a>
, and  <a href="https://www.microsoft.com/en-us/software-download/windows10" target="_blank">Windows 10 Pro ISO</a>. On the Windows Server link just fill up the form and click download, and on the Windows 10 link make sure you select the "Create Windows 10 installation media" option. Once we have everything downloaded we can run the Virtual Box installer. Next, were going to run the "Media creation tool" that we downloaded from the windows 10 link. Hit accept on the EULA and on the next screen make sure you select "Create installation media": <br/>
<img src="https://imgur.com/XuAxpYS.png" height="50%" width="50%" alt="Installation Steps"/>
<br />
<br />
Click next a few times then select ISO file when you get to the "choose which media to use" section:  <br/>
<img src="https://i.imgur.com/tcTyMUE.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enter the number of passes: <br/>
<img src="https://i.imgur.com/nCIbXbg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Confirm your selection:  <br/>
<img src="https://i.imgur.com/cdFHBiU.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Wait for process to complete (may take some time):  <br/>
<img src="https://i.imgur.com/JL945Ga.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Sanitization complete:  <br/>
<img src="https://i.imgur.com/K71yaM2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Observe the wiped disk:  <br/>
<img src="https://i.imgur.com/AeZkvFQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
