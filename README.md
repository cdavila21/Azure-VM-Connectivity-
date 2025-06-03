# Vitual Private Network (VPN)
![image alt](https://github.com/cdavila21/Vitual-Private-Network/blob/main/How-vpn-works-01-1024x512-138588629.jpg?raw=true)
<p align="center">

</p>

<h1>Installation & Requirements </h1>
This section covers Virtual Private Networks (VPNs) and how they help protect remote connections within a network environment.<br />

<h2>Environments and Technologies Used</h2>

- A VPN (Proton VPN)
- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>STEPS INCLUDED</h2>

- STEP 1 - Locate Local IP
- STEP 2 - Setting Up VM Using Azure
- STEP 3 - Locating IP Through VM (Canada)
- STEP 4 - Connecting to VPN Through VM
- STEP 5 - Locating IP Through VPN (Netherlands)

<h2>Installation Steps</h2>

STEP 1 - Locate your own personal IP address by going to "www.whatismyipaddress.com" which will be able to show you your local IP address. We will use this later as well. See EXAMPLE 1A below.

EXAMPLE 1A
![image alt](https://github.com/user-attachments/assets/20b6840a-c1f5-4d47-bd7a-5eb97b3c292c)

</p>
<p>

Next we will set up our virtual machines on Azure. 
  
</p>
<br />

STEP 2 - Go to www.portal.azure.com, create an account, open a subscription, create a resource group and find Virtual Machines. See Example 2A for the Virtual Machine set up page. 

EXAMPLE 2A
<p>
<img src="https://i.imgur.com/K9oaS2z.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Creating the Virtual Machine on Example 2B the VM name set to “Vpn-Test1-VM” with central Canada as the REGION. Ensure the other items are selected as shown in EXAMPLE 2B & 2C.

EXAMPLE 2B

![image alt](https://github.com/cdavila21/Vitual-Private-Network/blob/main/canada.png?raw=true)
</p>
<p>

For the Username and Password you can create your credentials.
  
</p>
<br />

EXAMPLE 2C

![image alt](https://github.com/cdavila21/Vitual-Private-Network/blob/main/username%201.png?raw=true)
</p>
<p>

Select the “Networking” tab towards the top of the page and view EXAMPLE 2D inputs to match. 
  
</p>
<br />

EXAMPLE 2D

![image alt](https://github.com/cdavila21/Vitual-Private-Network/blob/main/network.png?raw=true)
</p>
<p>

Then select “Review and Create”, once it passes validation select “Create” at the bottom. 
  
</p>
<br />

NEXT: At the Virtual Machine we see that the IP to the Virtual Machine is “40.82.163.67”. See EXAMPLE 2E

EXAMPLE 2E


![image alt](https://github.com/cdavila21/Vitual-Private-Network/blob/main/ip%20address.png?raw=true)
</p>
<p>


STEP 3 – Log Into the VM and Find IP Address
<p>
Now that we have set up the Virtual Machine we will connecting to it using the application “Remote Desktop Connection” (EXAMPLE 3A) and input the IP address for the VM that we located in EXAMPLE 2E and then input the set credentials we set when creating the VM (see EXAMPLE 3B). Once logged in, we will open the web browser and again look up www.whatismyipaddress.com (EXAMPLE 3C).

  
</p>
<br />
EXAMPLE 3A

![image alt](https://github.com/cdavila21/Vitual-Private-Network/blob/main/remote.png?raw=true) 
</p>
<p>

  
</p>
<br />

EXAMPLE 3B
<p>

</p>
<p>

When we look up the IP address for the new VM inside the remote desktop at www.whatismyipaddress.com we see that this VM is showing the location for Canada. (EXAMPLE 3C).

</p>
<br />

EXAMPLE 3C

![image alt](https://github.com/cdavila21/Vitual-Private-Network/blob/main/sscan%201.png?raw=true)
</p>
<p>

STEP 4 – CONNECTING TO VPN (Free Version)

Using the local computer go to protonvpn.com and create a free account (if you use the VM then Canada will display on your browser). Once you are logged into your account, copy the URL from the Proton VPN website (EXAMPLE 4A) and then paste the URL to the VM web browser. 

  
</p>
<br />

EXAMPLE 4A
<p>
<img src="https://i.imgur.com/orO2O5y.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

Once you have logged into your Proton VPN account on the VM, you will select “Downloads” and choose to download the “Windows” version. Once the application Proton VPN is installed we will log in using the credentials we used when setting up a free account on Proton VPN. Then connect to the VPN through the installed app. See EXAMPLE 4B when this steps are completed.  
  
</p>
<br />


EXAMPLE 4B
<p>
<img src="https://i.imgur.com/oqPHozb.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>

On the left hand side of the VPN you can select a country where you want your VPN to be, the image below shows the VPN being connected to an IP in the Netherlands. See EXAMPLE 4C
  
</p>
<br />

EXAMPLE 4C

![image alt](https://github.com/cdavila21/Vitual-Private-Network/blob/main/ss%204.png?raw=true)
</p>
<p>

Next we will look at the IP again using the VM browser now that we have connected the VPN to the Netherlands. The website www.whatismyipaddress.com shows yet another IP address using the VPN from the Netherlands. 
  
</p>
<br />

EXAMPLE 4D

![image alt](https://github.com/cdavila21/Vitual-Private-Network/blob/main/ssam%202.png?raw=true)
</p>
<p>

Looking at this exercise we see that we have utilized 3 different IP addresses just from your local computer to connect to the internet.
Home IP (USA): 23.28.19.2 
Virtual Machin IP (Canada): 40.82.163.67
Virtual Machin IP VPN (Netherlands) 185.107.80.68 

  
</p>
<br />
