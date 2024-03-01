<h1>Failed RDP to IP Geolocation Information</h1>




<h2>Description</h2>
<b>This repository had my heart racing! It houses a potent PowerShell script crafted to dissect Windows Event Log data, specifically targeting failed RDP attacks. Using a third-party API, the script uncovers the geographic origins of these malicious assaults.


</b>
<br />
<br />
In this thrilling Lab, I showcase the script's prowess by integrating it with Azure Sentinel (SIEM) and deploying it alongside a live virtual machine configured as a honeypot. Prepare to witness real-time RDP Brute Force attacks from across the globe. With this custom PowerShell script, I unveil the attackers' geolocation information and visualize their movements on an Azure Sentinel Map!
<br />
<br />
<p align="center">
 
<img src="https://imgur.com/VlzpCFD.png"/>
</p>
<h2>Languages Used</h2>

- <b>PowerShell:</b> Extract RDP failed logon logs from Windows Event Viewer 

<h2>Utilities Used</h2>

- <b>ipgeolocation.io:</b> IP Address to Geolocation API

<h2>Attacks from Argentina coming in; Custom logs being output with geodata</h2>

<p align="center">
<img src="https://imgur.com/oj7W78F.png"/>
</p>

<h2>World map of incoming attacks after 24 hours (built custom logs including geodata)</h2>

<p align="center">
<img src="https://imgur.com/8GMTPcw.png"/>
</p>
<br />
<br />
<h2>Key Features</h2>
- <b>Extract RDP failed logon logs from Windows Event Viewer</b><br />
- <b>Utilize ipgeolocation.io API to fetch geolocation data of attackers</b><br />
- <b>Integrate with Azure Sentinel to monitor and respond to attacks</b><br />
- <b>Visualize attacker geolocation information on an Azure Sentinel Map</b><br />
<br />
<br />
<h2>Lab Overview</h2>
- <b>Setup:</b> Configure Azure Sentinel and connect it to a live virtual machine acting as a honeypot.<br />
- <b>Observation:</b> Monitor live RDP Brute Force attacks from around the world.<br />
- <b>Analysis:</b> Execute the custom PowerShell script to extract and analyze failed RDP attack logs.<br />
- <b>Visualization:</b> Plot attacker geolocation data on an Azure Sentinel Map for real-time insights.<br />
<br />
<h2>Contributors</h2>
- <b>Jenna Frank</b><br />
<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
