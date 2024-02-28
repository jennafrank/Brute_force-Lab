<h1>Failed RDP to IP Geolocation Information</h1>




<h2>Description</h2>
<b>This repository contains a PowerShell script designed to parse Windows Event Log information for failed RDP attacks. It utilizes a third-party API to gather geographic information about the attackers' location.
</b>
<br />
<br />
The script is utilized in a demo scenario where Azure Sentinel (SIEM) is set up and connected to a live virtual machine acting as a honeypot. Live attacks, specifically RDP brute force attempts, are observed from various locations worldwide! A custom PowerShell script is employed to retrieve the attackers' geolocation information and plot it on an Azure Sentinel Map.

<br />
<br />
<p align="center">
<img src="https://private-user-images.githubusercontent.com/151777956/308397332-01836cf5-794f-4747-80f2-ae0488e26997.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MDkwODc4NzEsIm5iZiI6MTcwOTA4NzU3MSwicGF0aCI6Ii8xNTE3Nzc5NTYvMzA4Mzk3MzMyLTAxODM2Y2Y1LTc5NGYtNDc0Ny04MGYyLWFlMDQ4OGUyNjk5Ny5wbmc_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjQwMjI4JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI0MDIyOFQwMjMyNTFaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT1hMjUxNzIxZDU1MDFhZWNhYTgzNzkzMmY0N2E2MjU4MjY1NzhiYzczMDIwNTJlYjI2OTFhZjY2Y2RlMzZlNzZhJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZhY3Rvcl9pZD0wJmtleV9pZD0wJnJlcG9faWQ9MCJ9.FjZ76NN6WbRJLwWW5LyjHlOZXYFSChb-5QGEwDC3CdA" height="85%" width="85%" alt="RDP event fail logs to iP Geographic information"/>
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


<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
