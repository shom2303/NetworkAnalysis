<h1>Network Analysis Lab</h1>

 ### [YouTube Demonstration](https://youtu.be/VmLbdTw0HX8)

<h2>Description</h2>
In this lab, called Tomcat Takeover and hosted by CyberDefenders, I investigated suspicious activity on a compromised Apache Tomcat web server. By analyzing the provided PCAP file using Wireshark, I identified potential scanning behavior, open ports, and clues that led to uncovering an attacker’s successful login credentials. CyberChef was also used to decode the hash value and reveal the plaintext username and password that the attacker successfullu used to login. The analysis further uncovered tools used for directory enumeration, malicious file uploads, and the persistence method employed by the attacker.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Wireshark</b> 
- <b>CyberChef</b>

<h2>Environments Used </h2>

- <b>Apple macOS</b>

<h2>Lab walk-through:</h2>

<p align="center">
Identified the source IP address initiating suspicious requests through packet analysis: <br/>
<img src="https://i.imgur.com/OPdpMkd.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Determined the country of origin for the attacker based on the identified IP address:  <br/>
<img src="https://i.imgur.com/eDo4Apm.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Found the open port that grants access to the web server’s admin panel:  <br/>
<img src="https://i.imgur.com/qmjl91W.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Analyzed the tools used by the attacker for directory and file enumeration:  <br/>
<img src="https://i.imgur.com/BHYkO1h.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
 <br />
Identified the specific admin panel directory uncovered by the attacker:  <br/>
<img src="https://i.imgur.com/5elWeJO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
 <br />
Located the hash value used for login credentials in the captured traffic:  <br/>
<img src="https://i.imgur.com/TLwd8T3.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
 <br />
Used CyberChef to decode the hash value into plaintext username and password:  <br/>
<img src="https://i.imgur.com/PxMTzjZ.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
 <br />
Detected the malicious file uploaded by the attacker to establish a reverse shell:  <br/>
<img src="https://i.imgur.com/fNco6RM.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
 <br />
Analyzed the command scheduled by the attacker to maintain persistence on the server:  <br/>
<img src="https://i.imgur.com/T1yvpSv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
