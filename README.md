<h1>Active Directory Home Lab Guide</h1>


<h2>Description</h2>
In this guide we're going to walk through how to create an Active Directory home lab enviroment using Virtual Box. Configuring and running through this lab will definitely help develop your understanding of how Active Directory and Windows networking works, so I highly recommend running through it a couple of times, ask questions where stuff is unclear, and eventually try to build it on your own without needing this guide. Please let me know if you have any questions!
<br />


<h2>Environments Used</h2>

- <b>Windows Server 2022</b> 
- <b>Windows 10 Pro</b>

<h2>Project walk-through:</h2>

<p align="center">
First we are going to download a few things <a href="https://www.virtualbox.org/" target="_blank">Virtual Box</a>
, <a href="https://info.microsoft.com/ww-landing-windows-server-2022.html" target="_blank">Windows Server 2022 ISO</a>
, and  <a href="https://www.microsoft.com/en-us/software-download/windows10" target="_blank">Windows 10 Pro ISO</a>. On the Windows Server link just fill up the form and click download, and on the Windows 10 link make sure you select the "Create Windows 10 installation media" option. Once we have everything downloaded we can run the Virtual Box installerand install it on our computer. Next, were going to run the "Media creation tool" that we downloaded from the windows 10 link. Hit accept on the EULA and on the next screen make sure you select "Create installation media": <br/>
<img src="https://imgur.com/XuAxpYS.png" height="50%" width="50%" alt="Installation Steps"/>
<br />
<br />
Click next a few times then select ISO file when you get to the "choose which media to use" section. Once we have created the Windows 10 ISO were ready to start setting up our virtual machines. Open up Virtual Box if you don't have it running already and select "new" under the blue star icon in the top middle of the screen. Name the virtual machine "Windows Server 2022", select the ISO for the server from your downloads folder, and click the "Skip Unattended Installation" box. It should look like this:  <br/>
<img src="https://imgur.com/fO4eMUl.png" height="80%" width="80%" alt="Installation Steps"/>
<br />
<br />
Next we need to allocate the resources for the virtual machine. I recommend 4GB of RAM, 4 cores, and 50GB of storage if your system can handle it. Adjust the sliders to match the spec or google Windows Server 2022 system requirements to find the minimums if your system doesnt have the resources to spare. Note we can use these same settings for all the virtual machines for this lab: <br/>
<img src="https://imgur.com/WRtNewT.png" height="80%" width="80%" alt="Installation Steps"/>
<br />
<br />
Click next a few times and finish, and we're ready to boot up our first virtual machine! Select "Windows Server 2022" from the left, and click "start" under the green arrow in the top center of the screen. Now we can run through the Windows Server install just like installing any other OS. If you have never done it before don't worry we're going to do it together:  <br/>
<img src="https://imgur.com/eMJqtu4.png" height="80%" width="80%" alt="Installation Steps"/>
<br />
<br />
 Click next, and install and the installer will start running. The next step is important we need to select the second option from the list called "Windows Server Standard Evaluation (Desktop Experience)" otherwise the server won't include a graphical user interface and we will have to interact with it only through the command line.:  <br/>
<img src="https://imgur.com/clX0RD3.png" height="80%" width="80%" alt="Installation Steps"/>
<br />
<br />
Click next, agree to the EULA and select Custom install, then select next again and let it do its thing. This will take a couple of minutes so be patient. The server will start up on its own when the installation is complete and prompt you to enter a password for the administrator account. Once you do you'll be at the login screen from the server. To login you will need to select "input" from the top of the screen, and "keyboard", then insert "Ctrl-alt-del". Now we'll be able to imput the password we just set for the server and login. Server Manager will load automaticly and you will see a prompt on the left of the screen asking if we want to allow the PC to be descoverable on the network, select "yes":  <br/>
<img src="https://imgur.com/wizaw0U.png" height="80%" width="80%" alt="Installation Steps"/>
<br />
<br />
:  <br/>
<img src=".png" height="80%" width="80%" alt="Installation Steps"/>
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
