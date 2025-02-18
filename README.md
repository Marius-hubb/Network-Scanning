<h1>Network Recon: Uncovering Hosts and Monitoring Traffic</h1>

 ## [Video Demonstration (12:31)](https://drive.google.com/file/d/1bmvQORkCRQJLOKtMBQEgJbIlThoKNk2l/view?usp=sharing)

<h2>Description</h2>

This lab explores network scanning and traffic analysis using tools in both Linux and Windows. We start by inspecting network interfaces and gateway settings with commands like ip a, ifconfig/ipconfig, and ip route/route. We'll then discover live hosts on the local network through ARP-based scanning with tools such as arp-scan and netdiscover — demonstrating both active and passive modes.

Next, we explore network path analysis with traceroute (and its variants like mtr, pathping, or tracert), and then transition into in-depth host and port scanning using Nmap. We will cover various scanning techniques, including ARP scans (nmap -sn), TCP scans (both full connect and stealth SYN scans), UDP scans, and methods to save and enhance scan outputs with verbose and XMAS scans.

Finally, we capture and analyze network traffic in real time using Wireshark, applying filters to gain deeper insights into the data.<br />
<br />

<h2>Lab walk-through:</h2>

<p align="center">Adding the webserver 10.10.1.16 machine as Wazuh agent
<br/>
<img src="https://i.imgur.com/55MK1xc.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<p align="center">Extract the Agent key
<br/>
<img src="https://i.imgur.com/NvH0Kal.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
<p align="center">creating key.txt file that will contain the Agent key. 
<br/>
<img src="https://i.imgur.com/GMSAjNg.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
<p align="center">Copying the key.txt file into the shared folder on 10.10.1.16
<br/>
<img src="https://i.imgur.com/bsYP7lI.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
<p align="center">Configuring the firewall to communicate with the agent
<br/>
<img src="https://i.imgur.com/TSrTMic.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />

<p align="center">Installing Wazuh agent on WebServer machine
<br/>
<img src="https://i.imgur.com/iRfQUMu.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
<p align="center">Restarting Wazuh
<br/>
<img src="https://i.imgur.com/Oo8DdvY.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
<p align="center">Verifying that the agent is active
<br/>
<img src="https://i.imgur.com/yMh3Hyy.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
<p align="center">Performing brute-forece attack via RDP on WebServer 10.10.1.16 using hydra
<br/>
<img src="https://i.imgur.com/jO3iBMC.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
<p align="center">We can observe the alert for Dst IP 10.10.1.16.
<br/>
<img src="https://i.imgur.com/f0e8aHo.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<br />
<br />
