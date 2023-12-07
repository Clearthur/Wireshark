<h1>Analyze packets with Wrieshark</h1>


<h2>Description</h2>
Utilizing Wireshark to inspect packet data and apply filters to sort through packet information.
<br />


<h2>Utilities Used</h2>

- <b>Wireshark</b> 

<h2>Environments Used </h2>

- <b>Windows 10</b>
- <b>Wireshark</b>

<h2>Walk-through:</h2>

<p align="center">
Start by opening Wireshark and performing a scan of the network to capture traffic: <br/>
<img src="first.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Selected Virtual machines and followed the steps to create  virtual machines including creating usernames and passwords for all VM's:  <br/>
<img src="Select VM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Created a Log Analytic Workstation to recive all logs from the virtual machines: <br/>
<img src="Law.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Connected all virtual machines to the Log analytics Workstation. This process can take several minutes:  <br/>
<img src="Vms connected to law.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
After the log analytics workstation has connected to all virtual machines it is time to create a SIEM tool using Microsoft Sentinel to scan the logs coming from our virtual machines. Select Microsoft Sentinel form the home page of the Azure Portal and follow the steps to activate Microsoft Sentinel:  <br/>
<img src="select sentinel.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Once Microsoft Sentinel has been installed you have to download and activate connectors for Sentinel. Once the Connectors are online you ready to scan for security logs with Microsoft Sentinel :  <br/>
<img src="data connectors connected.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Finally, we can test the integrity of the security of our network. We secured one virtual machine by closing all unnecessary ports and setting up windows defender. The other machines were not secure and were exposed to the raw internet. Using Microsoft Sentinel, we can see that in just a short time we have several attempts to remotely access our virtual machines by unauthorized individuals. The results below show VM 2 and VM 3 have several failed logins attempts indicating these systems are vulnerable to attack and VM 1 has none proving that it is secure. This shows the importance of proper security on endpoint systems.:  <br/>
<img src="results.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
