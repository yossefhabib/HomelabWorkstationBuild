<h1>Homelab-Infrastructure</h1>

 ### [YouTube Demonstration](https://youtu.be/7eJexJVCqJo)

<h2>Overview</h2> 
This project documents the design, assembly, configuration, and validation of a high-performance workstation built to support Security Operations Center (SOC)–focused lab activities. The system is intended to serve as a stable, multi-VM environment for defensive security testing, log analysis, threat simulation, and detection engineering practice, with room for more advanced labs as my skills develop.


<h2>Objective</h2>

- Build a reliable bare-metal platform capable of running multiple virtual machines simultaneously
- Enable SOC-relevant lab scenarios (Active Directory, SIEM, endpoint monitoring)
- Validate hardware performance and thermal stability under load
- Document configuration and deployment steps for reproducibility

<h2>Capabilities Enabled</h2>

- Multi-VM virtualization (Windows, Linux)
- Active Directory lab simulation
- Log forwarding and SIEM ingestion
- Network traffic capture (Wireshark, Zeek)
 -Vulnerability scanning (OpenVAS, Nmap)
  
<h2>Hardware and Tools</h2>

- CPU: Ryzen 7 7800X3D
- Motherboard ASUS B650E-E TUF Gaming WiFi
- GPU: RTX 5070 Shadow 2X
- Storage: Samsung 990 Pro NVMe 1TB
- Memory: 32GB DDR5-6000
- Power Supply: RM850e PSU
- CPU Cooler: Phantom Spirit 120 SE
- Case: Meshify 2 case


<h2>Environments Used </h2>

- <b>Windows 10</b> (21H2)

<h2>Program walk-through:</h2>

<p align="center">
Launch the utility: <br/>
<img src="https://i.imgur.com/62TgaWL.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Select the disk:  <br/>
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
