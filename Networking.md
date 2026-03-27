# &#x09;				Networking







* ### VNet (Virtual Network) :

##### &#x09;			A virtual network is a software-defined network that allows devices, servers, or systems to communicate securely 				without being physically connected. It is widely used in cloud computing and enterprise security.







##### **Virtual networks are critical in cyber security because they:**



* ###### Isolate sensitive data from public access

###### 

* ###### Control traffic flow using firewalls and routing rules

###### 

* ###### Prevent unauthorized access

###### 

* ###### Enable secure remote connections







#### **Key Components :**





##### **1. Virtual Private Network (VPN)**



###### &#x09;					A VPN encrypts internet traffic and hides user identity

###### 

###### &#x09;					Example : Secure remote work connections





##### **2. Subnets**



###### &#x09;	a. Divides a virtual network into smaller segments

###### 

###### &#x09;	b. Helps in limiting access and containing threats









##### **3. Firewalls**



###### &#x09;	a. Monitor and filter incoming/outgoing traffic

###### 

###### &#x09;	b. Block malicious activity









##### **4. Network Security Groups (NSGs)**



###### &#x09;					Define rules for traffic control at a granular level.









##### **5. IP Address Range**



###### &#x09;		Defines how many devices can exist in your network

###### 

###### &#x09;		Example: 10.0.0.0/16

###### 





##### **6. Route Tables**



###### &#x09;		Define how traffic moves inside the network









##### **7. Gateways**



###### &#x09;	Connect VNet to:

###### 

###### &#x09;			a. Internet

###### 

###### &#x09;			b. On-premise networks (VPN)











##### &#x09;**Types of Virtual Networks :**









1. ##### **Private Virtual Network**



* ###### Used within organizations

###### 

* ###### Not accessible from the public internet









##### **2. Public Virtual Network**





* ###### Connected to external networks

###### 

* ###### Used for web servers, applications

###### 







##### 3\. Hybrid Virtual Network





* ###### Combines private and public networks

###### 

* ###### Common in cloud environments













* #### NAT Gateway :

##### &#x09;	**Network Address Translation Gateway** is a cloud networking service that allows private resources inside a 					network (like a VNet) to access the internet without exposing them directly.

##### 

##### &#x09;	 used in platforms like Microsoft Azure and Amazon Web Services.











* ##### **Internet Gateway:**

###### &#x09;		**IGW is a cloud networking component that allows resources inside a virtual network to communicate with the internet** 

###### &#x09;		**(both inbound and outbound).**

###### 

###### &#x09;		**It’s mainly used in Amazon Web Services within a VPC (Virtual Private Cloud).**





* ##### **Reverse Proxy :**

###### &#x09;		**A reverse proxy is a server that sits between clients (users) and multiple backend servers, handling requests on behalf of those servers.**

###### &#x09;		**It’s widely used in web infrastructure for security, load balancing, and performance optimization.**





##### **How It Works ?**



&#x09;		1. Client sends request to reverse proxy

---

&#x09;		2. Proxy decides which backend server should handle it

---

&#x09;		3. Backend server processes request and returns response to proxy

---

###### &#x09;		4. Proxy sends response to client



* ##### **Key Features :**



&#x09;		1. **Load Balancing** **–** distributes requests across servers

---

&#x09;		2. **SSL/TLS Termination** **–** offloads encryption work from backend

---

&#x09;		3. **Caching –** speeds up responses

---

&#x09;		4. **Compression –** reduces bandwidth usage

---

###### &#x09;		5. **Security –** hides backend IPs from clients









* ##### **Reverse Proxy in Cybersecurity :**



* ###### Hides backend servers → reduces attack surface

###### 

* ###### Blocks malicious requests → can filter bad traffic

###### 

* ###### Rate-limiting → prevents DDoS

###### 

* ###### Can integrate with WAF (Web Application Firewall)









* ##### **SSL Certificate :**

###### &#x09;		It is a digital certificate **that encrypts communication between** a **client** (browser) and a **server**. 



###### &#x09;		It ensures that **sensitive data** like passwords, credit card numbers, and personal info are **secure in transit**.

###### 

###### &#x09;		It used in HTTPS websites.





* ##### **Key Features :**



###### &#x09;		**Encryption 	–** 	protects data in transit

###### 

###### &#x09;		**Authentication  –** 	verifies the server is who it claims to be

###### 

###### &#x09;		**Integrity 	–** 	ensures data isn’t tampered with

###### 



* ##### **Types of SSL Certificates :**



###### &#x09;	**Type					Description**



###### &#x09;Domain Validated (DV)			Verifies domain ownership



###### &#x09;Organization Validated (OV)		Verifies domain + organization info



###### &#x09;Extended Validation (EV)		Highest validation; shows company name in browser



###### &#x09;Wildcard SSL				Secures a domain and all its subdomains



###### &#x09;Multi-Domain (SAN)			Secures multiple domains with one certificate

###### 



* ##### **Why SSL Matters in Cybersecurity ?**



###### &#x09;					Prevents Man-in-the-Middle (MITM) attacks

###### 

###### &#x09;					Protects sensitive info from eavesdroppers

###### 

###### &#x09;					Boosts user trust (padlock icon)



* ##### **Tools \& Checks :**



###### &#x09;		**OpenSSL 		→** 	Create/inspect certificates

###### 

###### &#x09;		**Browser DevTools 	→** 	heck certificate validity

###### 

###### &#x09;		**SSL Labs Test 		→** 	Analyze server SSL configuration







* ##### **SSL vs TLS**



###### &#x09;		**SSL 	=** 	older protocol, mostly deprecated

###### 

###### &#x09;		**TLS 	=** 	modern, secure version of SSL

###### 

###### &#x09;		Most “SSL certificates” today actually use TLS protocols

###### 

