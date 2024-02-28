<h1>Failed RDP to IP Geolocation Information</h1>




<h2>Description</h2>
<b>This repository had my heart racing! It houses a potent PowerShell script crafted to dissect Windows Event Log data, specifically targeting failed RDP attacks. Using a third-party API, the script uncovers the geographic origins of these malicious assaults.


</b>
<br />
<br />
In this thrilling demo, I showcase the script's prowess by integrating it with Azure Sentinel (SIEM) and deploying it alongside a live virtual machine configured as a honeypot. Prepare to witness real-time RDP Brute Force attacks from across the globe. With this custom PowerShell script, I unveil the attackers' geolocation information and visualize their movements on an Azure Sentinel Map!
<br />
<br />
<p align="center">
<img src="https://private-user-images.githubusercontent.com/151777956/308397332-01836cf5-794f-4747-80f2-ae0488e26997.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MDkxNDU3MTQsIm5iZiI6MTcwOTE0NTQxNCwicGF0aCI6Ii8xNTE3Nzc5NTYvMzA4Mzk3MzMyLTAxODM2Y2Y1LTc5NGYtNDc0Ny04MGYyLWFlMDQ4OGUyNjk5Ny5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwMjI4JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDIyOFQxODM2NTRaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT0wM2Q5ZTkzZTNmMTI1MDA5NDM1NTI5OTZkYmJjZGUwYTg3MDUyY2M0MDJkMTBhNTgyZjMxNGQ4ZDBlNThiYjZjJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.taREpg99TIZsqJpZL61CGgoQ-_KXnMR96ZzI1pRO-O4"/>
</p>
<h2>Languages Used</h2>

- <b>PowerShell:</b> Extract RDP failed logon logs from Windows Event Viewer 

<h2>Utilities Used</h2>

- <b>ipgeolocation.io:</b> IP Address to Geolocation API

<h2>Attacks from Argentina coming in; Custom logs being output with geodata</h2>

<p align="center">
<img src="https://private-user-images.githubusercontent.com/151777956/308397369-4a2b2b2c-48b7-4662-bed7-3fb9dc280c78.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MDkwODc4NzEsIm5iZiI6MTcwOTA4NzU3MSwicGF0aCI6Ii8xNTE3Nzc5NTYvMzA4Mzk3MzY5LTRhMmIyYjJjLTQ4YjctNDY2Mi1iZWQ3LTNmYjlkYzI4MGM3OC5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwMjI4JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDIyOFQwMjMyNTFaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1mZGFhYjIwZjFmNTJkYzgzMDhhYWYzZjQxMGFhYzM4ZTcwMGMwODZlZDFiYmY3YTFkOWIwYmU0NjBkZWY2ZjUxJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.hHjUxEKiXcPtFN2H6cEjoObAKj5koRYOZ2OfkcVCYKw" height="85%" width="85%" alt="Image Analysis Dataflow"/>
</p>

<h2>World map of incoming attacks after 24 hours (built custom logs including geodata)</h2>

<p align="center">
<img src="https://i.imgur.com/krRFrK5.png" height="85%" width="85%" alt="Image Analysis Dataflow"/>
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
<h2>Demo Overview</h2>
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
