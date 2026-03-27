# &#x09;				    Ports





* ##### A port is a numbered channel (0–65535) tied to an IP address. It helps identify which service or application should receive incoming data.

##### 

##### &#x20; **Think of it like:**

##### 

* ##### IP address = building address

##### 

* ##### Port = specific room or office inside that building











#### **Types of Ports :**



##### **1. Well-Known Ports (0–1023)**



###### &#x09;			**a. Reserved for common \& specifically used services.**

###### &#x09;			**b. Used by some widely adopted protocols and services.**

###### &#x09;			**c. Used by common services:**



###### &#x09;							Port 80 → HTTP (web traffic)

###### 

###### &#x09;							Port 443 → HTTPS (secure web traffic)

###### 

###### &#x09;							Port 21 → FTP (file transfer)

###### 

###### &#x09;							Port 22 → SSH (secure remote login)

###### 

###### &#x09;							Port 25 → SMTP (email sending)









##### **2. Registered Ports (1024–49151)**



###### &#x09;					**a. Used by applications or services that are not as common.**

###### &#x09;					**b. but used by those applications or services which require its specific port.**

###### &#x09;					**c. Organizations can ask IANA(Internet Assigned Number Authority) for any specific port number within the range.**

###### &#x09;					**d. Assigned to specific applications:**



###### &#x09;										Port 3306 → MySQL database

###### 

###### &#x09;										Port 3389 → Remote Desktop Protocol (RDP)









##### **3. Dynamic / Private Ports (49152–65535)**



###### &#x09;						a. Also known as Ephemeral or **Private Port**.

###### &#x09;						b. Used for those connections that are temporary or short-lived.

###### &#x09;						c. Not registered or assigned and can be used by any process.	

###### &#x09;						d. Used temporarily by client systems for outgoing connections.







##### \*\*\*\*\*\*   In Industry a firewall can block port 3389 by default(used for remote desktop connections).















##### **Why Ports Matter in Cybersecurity ?**







##### **1. Attack Surface**



###### &#x09;		Open ports can be entry points for attackers.

###### &#x09;	**Example:**

###### 

###### &#x09;		Open port 22 → target for brute-force SSH attacks







##### **2. Port Scanning**



###### &#x09;		**Attackers use tools like :** Nmap

###### 

###### &#x09;		**To :** Discover open ports

###### 

###### &#x09;		Identify running services

###### 

###### &#x09;		Find vulnerabilities







##### **3. Common Threats**



###### &#x09;		Port 445 (SMB) → exploited in ransomware attacks (e.g., WannaCry)

###### 

###### &#x09;		Port 3389 (RDP) → frequently targeted for unauthorized access







##### **4. Firewall Protection**



###### &#x09;		**Firewalls control which ports are open or closed:**

###### 

###### &#x09;								Block unused ports ❌

###### 

###### &#x09;								Allow only necessary ones ✅







##### 

##### &#x20;     **Port		Service		Protocol			Why It Matters**

###### 

###### &#x09;21			FTP			TCP				Weak authentication, anonymous login possible

###### &#x09;22			SSH			TCP				Remote access, brute-force attacks

###### &#x09;23			Telnet			TCP				Unencrypted login (highly insecure)

###### &#x09;25			SMTP			TCP				Email spoofing, open relay issues

###### &#x09;53			DNS			TCP/UDP				DNS poisoning, zone transfer

###### &#x09;67/68			DHCP			UDP				Rogue DHCP attacks

###### &#x09;69			TFTP			UDP				No authentication, easy exploitation

###### &#x09;80			HTTP			TCP				Web vulnerabilities (XSS, SQLi)

###### &#x09;110			POP3			TCP				Plaintext credentials

###### &#x09;111			RPC			TCP/UDP				Information gathering

###### &#x09;123			NTP			UDP				Amplification (DDoS) attacks

###### &#x09;135			MS RPC			TCP				Windows enumeration

###### &#x09;139			NetBIOS			TCP				Legacy Windows vulnerabilities

###### &#x09;143			IMAP			TCP				Email credential attacks

###### &#x09;443			HTTPS			TCP				SSL/TLS misconfigurations

###### &#x09;445			SMB			TCP				Used in ransomware like WannaCry ransomware

###### &#x09;1433			MSSQL			TCP				Database attacks

###### &#x09;1521			Oracle DB		TCP				Sensitive data exposure

###### &#x09;3306			MySQL			TCP				Database exploitation

###### &#x09;3389			RDP			TCP				Remote access brute-force

###### &#x09;8080			HTTP Alt		TCP				Proxy/web apps







