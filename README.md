<h1>🖥️ Cybersecurity Lab Workstation Build</h1>
Custom AM5 High-Performance Lab Machine

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
  
<h2>System Architecture</h2>

- CPU: Ryzen 7 7800X3D
- Motherboard ASUS B650E-E TUF Gaming WiFi
- GPU: NVIDIA GeForce RTX 5070
- Storage: Samsung 990 Pro NVMe 1TB
- RAM: 32GB DDR5-6000 (EXPO Enabled)
- Power Supply: Corsair RM850e
- CPU Cooler: Phantom Spirit 120 SE
- Case: Meshify 2 case
- OS: Windows 11 Pro



<h2>⚙️ Deployment Process:</h2>

<h3>1️⃣ Hardware Assembly</h3> 


Installed CPU and both RAM sticks in correct dual-channel configuration according to Motherboard manual: <br/>
 
 ![image2](https://github.com/user-attachments/assets/eb6f3711-f349-4a3f-b0d4-2f75ed0b5107)

<br />
<br />

Placed CPU cooler ontop of CPU with the correct amount of thermal paste and placed CPU fans in proper positions for air flow: <br/>
 
![image3](https://github.com/user-attachments/assets/59dade0e-92e7-45dc-b4fe-d0a1432d620d)


<br />
<br />
Mounted NVMe SSD with heatsink and installed GPU, verifying PCIe seating: <br/>

![image4](https://github.com/user-attachments/assets/335b7ccb-c682-40a4-81cf-ea402d0b6310)


<br />
<br />
Installed the proper PSU cables and ready for initial test before placing in case:  <br/>

![image5](https://github.com/user-attachments/assets/122c042b-8153-44f7-aa16-d52d8cc7d2c1)

<h2>2️⃣ Initial POST & Troubleshooting:</h2>
Issue Encountered:

- Yellow motherboard diagnostic LED (No boot up)
- White motherboard diagnostic LED (No display output)

Troubleshooting Actions:
- Reseated RAM (tested one stick at a time)
- Cleared CMOS (RTC reset)
- Reseated GPU
- Switched from DisplayPort to HDMI
- Verified power connections

Root Cause:
Improper GPU seating + initial memory training delay


Issue Encountered: Yellow motherboard diagnostic LED, fixed then followed by a white motherboard diagnostic LED

![image7](https://github.com/user-attachments/assets/2cf1bdeb-92c1-446a-80ed-5f379220f929)
![image8](https://github.com/user-attachments/assets/98086fcc-4c36-4fea-a5a6-9e76fe2b1cd7)


<br />
<br />
According to the motherboard manual, a yellow light indicates a DRAM error, so I reinstalled the RAM, verified the correct position, and securely placed it, then tried again. Was met with the White light, which meant a VGA issue, so I reinstalled the GPU and used an HDMI cord instead of DisplayPort for initial boot: 

![image11](https://github.com/user-attachments/assets/2c61a0c1-f398-4d64-a38f-42a1bd43ac0d)
<br />
<br />

Successful! I installed the motherboard, PSU, and fans appropriately into the case, then cleaned up the cables with proper cabling and ziptines:

![image13](https://github.com/user-attachments/assets/6bab119b-4d75-4bc4-ad0e-6c1e3b055478)
![image15](https://github.com/user-attachments/assets/ac8d0153-6e7f-4568-82bd-361d09842b2d)

<br />
<br />

<h2>3️⃣ BIOS Configuration</h2>

- Updated BIOS from version 0215 → 3602
- Enabled EXPO profile (DDR5-6000)
- Verified CPU voltage and thermals
- Confirmed storage detection
- Loaded optimized defaults post-update
  
![image20](https://github.com/user-attachments/assets/4c766156-4f9f-49ad-bfc5-7f7fcdbed239)

<br />
<br />


<br />
<br />
<h2>4️⃣ Driver Installation</h2>

After flashing windows and confirming proper boot into Windows 11 Pro, I installed all the neccessary drivers manually via USB:
- AMD Chipset Drivers
- Realtek LAN Drivers
- MediaTek WiFi Drivers
- NVIDIA Game Ready Drivers
<br />
Validated in:
Device Manager → No unknown devices

![image17](https://github.com/user-attachments/assets/06080ca7-220e-4db6-8e18-2c448f87ad27)



<h2> 5️⃣ Validation & Stability Checks </h2>

- Confirmed proper boot into Windows 11 Pro
- Verified GPU detection in NVIDIA Control Panel
- Confirmed 2560x1440 output
- Monitored CPU temps in BIOS & Windows
- Verified memory frequency (6000 MHz EXPO)
- Verified that all necessary drivers and updates were installed   <br/>
<br />
<br />

<h2> 🔐 Security Relevance </h2>

This build supports:

- Hyper-V multi-VM lab environments
- Malware analysis sandboxes
- Log aggregation simulations
- SOC alert triage labs
- Red/Blue team exercises


<br />


<h2>🛠 Lessons Learned</h2>

- Memory training on DDR5 can delay the initial POST
- USB 3.0 interference can impact wireless peripherals (while setting up mouse and keyboard) 
- BIOS updates require BitLocker awareness
- Always test hardware outside the case first
- GPU reseating resolves many “no display” issues

<br />
<h2>Outcome</h2>

- Final system is stable, updated, optimized, and ready for:
- Cybersecurity lab development
- Portfolio documentation
- Virtualization-heavy workflows
- Long-term professional use
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
