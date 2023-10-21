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

- <b>PowerShell:</b> Extract RDP failed logon logs from Windows Event Viewer 

<h2>Utilities Used</h2>

- <b>ipgeolocation.io:</b> [IP Address to Geolocation API](https://github.com/Mrudul-Waechter/Sentinel-Lab/blob/main/WindowsSecurityLogExporter.ps1)
