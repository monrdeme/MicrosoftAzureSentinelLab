<h1>Microsoft Azure Sentinel (SIEM) Lab</h1>

 <h2>Description</h2>
Project consisted of configuring Azure Sentinel (Microsoft's cloud SIEM) workbook to display global attack data (RDP brute force) on a world map according to physical location and magnitude of attacks. A custom PowerShell script was used to extract metadata from Windows Event Viewer to be forwarded to a third party API in order to derive geolocation data
<br />


<h2>Languages and Utilities Used</h2>

- <b>PowerShell</b> 
- <b>Microsoft Azure</b> 
- <b>ipgeolocation.io: IP Address to Geolocation API</b>

<h2>Environments Used </h2>

- <b>Windows 10</b> (21H2)

<h2>Project Walk-Through:</h2>

<p align="center">
Create Azure Subscription: <br/>
<img src="https://i.imgur.com/j5SMGY5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Create Virtual Machine:  <br/>
<img src="https://i.imgur.com/ejal6GD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Allow All In Firewall: <br/>
<img src="https://i.imgur.com/Lv1hk5A.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/66gWNYQ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Create Log Analytics Workspace:  <br/>
<img src="https://i.imgur.com/AkgYTWo.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Connect Log Analytics To VM:  <br/>
<img src="https://i.imgur.com/lcxkVJz.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/h7DNClJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/BvETOl4.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Enable Gathering VM Logs In Microsoft Defender For Cloud:  <br/>
<img src="https://i.imgur.com/ehvpHbR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/rs0iReR.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Setup Azure Sentinel:  <br/>
<img src="https://i.imgur.com/IffNUjG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Log Into VM With Remote Desktop:  <br/>
<img src="https://i.imgur.com/tAqRJaq.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/vcJ9Eal.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Observe Event Viewer Logs In VM:  <br/>
<img src="https://i.imgur.com/pVlHXZ5.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Turn Off Windows Firewall On VM:  <br/>
<img src="https://i.imgur.com/yzN2OdV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/SifBFCV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/SuJS0KA.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/if5IBSx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Download PowerShell Script:  <br/>
<img src="https://i.imgur.com/HlxTQfV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Get Geolocation.io API Key:  <br/>
<img src="https://i.imgur.com/v5dlpNp.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/XKzQFd6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Run Script To Get Geo Data From Attackers:  <br/>
<img src="https://i.imgur.com/JMctSIN.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Create Custom Log In Log Analytics Workspace To Bring In The Custom Log:  <br/>
<img src="https://i.imgur.com/CjYMwes.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/BxQNEMa.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/bDu0Ib1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/a451vHT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/1D8Xq0I.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/eQkAy1n.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/1Fo7lJK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Create Custom Fields/Extract Fields From Raw Custom Log Data:  <br/>
<img src="https://i.imgur.com/s7UWvDZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/HzXJv5g.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/jMzIjF9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/HvBn5oX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/JkuEjfs.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/iUpDeT8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/rUFw2C8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/KEFaUHO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/Q1kqHv6.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/1tXI6ot.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/ZvQP3f0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/CyUSKKO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/ummW9L7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/pztvfXB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/ZIrJnMJ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/HtO5bEa.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/Bp6maXC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/FQByvsM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/hqZIf0h.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Setup Map In Sentinel With Latitude and Longitude:  <br/>
<img src="https://i.imgur.com/ISIYPjT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/AU62wEZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/3ycJ1HH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/rfVPBtw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/04jKmyv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
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
