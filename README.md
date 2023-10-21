<h2>Description</h2>
<b>
The PowerShell script within this repository is designed to extract Windows Event Log data related to unsuccessful RDP intrusion attempts and employs a third-party API to retrieve geographical details about the attackers' location.
</b>
<br />
<br />
In this project, I've configured Azure Sentinel (SIEM) and linked it to a live virtual machine posing as a honey pot. Through this setup, I'm able to witness real-time attacks, specifically RDP Brute Force attempts, originating from various global locations. For this analysis, I've used a specialized PowerShell script to retrieve the attackers' geolocation data, which I then visualize on an Azure Sentinel Map for a comprehensive view of the attacks' origins.
<br />
<br />

<p align="center">
<img src="https://imgur.com/ABSjI51.png" height="85%" width="85%" alt="RDP event fail logs to iP Geographic information"/>
</p>
<h2>Languages Used</h2>

- <b>PowerShell:</b> [Extract RDP failed logon logs from Windows Event Viewer](https://github.com/Mrudul-Waechter/Sentinel-Lab/blob/main/WindowsSecurityLogExporter.ps1)

<h2>Utilities Used</h2>

- <b>ipgeolocation.io:</b> [IP Address to Geolocation API](https://ipgeolocation.io/)

<h2>Project Details</h2>
<br />
<br />

<ins><B>Created honeypot VM using Azure</ins></B>
<p align="center">
<img src="https://imgur.com/45F8m7e.png" height="65%" width="65%" alt="Azur Honeypot VM"/>
</p>
<br />
<br />

<ins><B>Added an inbound rule to expose the VM to the internet</ins></B>

 
<p align="center">
<img src="https://imgur.com/rprByJj.png" height="65%" width="65%" alt="Inbound Rule"/>
</p>


<p align="center">
<img src="https://imgur.com/EBDfdZy.png" height="65%" width="65%" alt="Inbound Rule"/>
</p>
<br />
<br />


<ins><B>Connected to the Azure Log Analytics Workspace </ins></B>
 
<p align="center">
<img src="https://imgur.com/8EM3IGb.png" height="65%" width="65%" alt="Azure log analytics workspace"/>
</p>
<br />
<br />

<ins><B>Collecting windows security event through Microsoft Defender</ins></B>

<p align="center">
<img src="https://imgur.com/N7BmbhF.png" height="65%" width="65%" alt="Microsoft Defender"/>
</p>
<br />
<br />

<ins><B>Connecting to Microsoft Sentinel-SIEM to log analytic workspace </ins></B>

<p align="center">
<img src="https://imgur.com/eQV2DiS.png" height="65%" width="65%" alt="SIEM"/>
</p>
<br />
<br />

<ins><B>Powershell script showing live attack data</ins></B>
<p align="center">
<img src="https://imgur.com/0sM0sDH.png" height="65%" width="65%" alt="Powershell script"/>
</p>
<br />
<br />

<ins><B>KQL query to extract log data</ins></B>

<p align="center">
<img src="https://imgur.com/zC0OwUN.png" height="65%" width="65%" alt="KQL query"/>
</p>
<br />
<br />

<h2>Live Brute Force attacks coming from all around the world</h2>

2 Hours after creating the honeypot VM
<p align="center">
<img src="https://imgur.com/J0J5mgS.png" height="65%" width="65%" alt="KQL query"/>
</p>
<br />
<br />
3 Hours after creating the honeypot VM
<p align="center">
<img src="https://imgur.com/qp0AnPD.png" height="65%" width="65%" alt="KQL query"/>
</p>
<br />
<br />
4 Hours after creating the honeypot VM
<p align="center">
<img src="https://imgur.com/ox1IsRg.png" height="65%" width="65%" alt="KQL query"/>
</p>
<br />
<br />

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
