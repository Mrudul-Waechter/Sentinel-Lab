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
- 
- <h2>Created honeypot VM using Azur</h2>
<p align="center">
<img src="https://imgur.com/45F8m7e.png" height="65%" width="65%" alt="Azur Honeypot VM"/>
</p>
<br />
<br />

 <h2>Added an inbound rule to expose the VM to the internet</h2>

 
<p align="center">
<img src="https://imgur.com/rprByJj.png" height="65%" width="65%" alt="Inbound Rule"/>
</p>


<p align="center">
<img src="https://imgur.com/EBDfdZy.png" height="65%" width="65%" alt="Inbound Rule"/>
</p>
<br />
<br />


 <h2>Connected to Log Analytics Workspace </h2>
 
<p align="center">
<img src="https://imgur.com/8EM3IGb.png" height="65%" width="65%" alt="Inbound Rule"/>
</p>
<br />
<br />

<h2>Turned on data collection for all event through Microsoft Defender</h2>

<p align="center">
<img src="https://imgur.com/N7BmbhF.png" height="65%" width="65%" alt="Inbound Rule"/>
</p>
<br />
<br />
