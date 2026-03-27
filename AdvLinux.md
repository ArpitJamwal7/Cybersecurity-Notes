# &#x09;				Advance Linux





* #### **Services \& Daemons :**

##### &#x09;		Services or daemons are background processes that run continuously to provide system functionality like networking, web 			hosting, or logging









* ##### **Service Control (systemctl) :**

###### &#x09;				systemctl \[action] <service-name>



##### &#x09;	**Example :**



###### &#x09;			Start a Service 			: 	systemctl start nginx

###### &#x09;			Stop a Service				: 	systemctl stop nginx

###### &#x09;			Restart a Service 			: 	systemctl restart nginx

###### &#x09;			Check Status 				: 	systemctl status nginx

###### &#x09;			Enable Service (auto start at boot) 	:	systemctl enable nginx

###### &#x09;			Disable Service 			: 	systemctl disable nginx

###### &#x09;			Check All Services 			: 	systemctl list-units --type=service

###### &#x09;			Check Running Services 			: 	systemctl list-units --type=service --state=running



###### &#x09;			SSH service 				: 	systemctl restart ssh

###### &#x09;			Apache web server 			: 	systemctl status apache2









* #### &#x20;**Secure Shell Daemon (sshd) :**

##### &#x09;			sshd is the daemon that enables secure remote access to a Linux system using the SSH protocol.







##### **Works :**



* ###### Runs in the background

###### 

* ###### Listens on port 22 (default)

###### 

* ###### Authenticates users (password / key)

###### 

* ###### Starts a secure session



###### Start SSH service : systemctl start ssh

###### Stop SSH service  : systemctl stop ssh

###### Restart SSH	  : systemctl restart ssh

###### Check status	  : systemctl status ssh

###### Enable at boot	  : systemctl enable ssh





###### **Command		Purpose**



###### ssh		Client (connect to server)

###### sshd		Server (accept connections)





##### **Package Management :**

###### &#x09;		Package management is used to install, update, and manage software in Linux using package managers like apt, yum, or dnf.







###### **Feature		APT			YUM/DNF**



###### OS		Ubuntu/Debian		RedHat/CentOS

###### Format		.deb			.rpm







* ##### **Package Management :** is about installing and maintaining software.

##### 



###### &#x09;	**Examples :**

###### 

###### &#x09;		APT (Ubuntu/Debian)

###### 

###### &#x09;		YUM (CentOS/RHEL)

###### 

###### &#x09;		npm (JavaScript)

###### 

###### &#x09;		pip (Python)





###### **What they do:**

###### 

###### &#x09;	1. Install/remove software

###### 

###### &#x09;	2. Manage dependencies

###### 

###### &#x09;	3. Update packages automatically













# &#x09;			**Architecture of the Linux OS**











* ###### describes how different components interact to make the system work. It’s typically shown as a layered structure.





##### **Linux Architecture (Layered View) :**



###### &#x09;							**+---------------------------+**

###### &#x09;							**|     User Applications     |**

###### &#x09;							**+---------------------------+**

###### &#x09;							**|         Shell             |**

###### &#x09;							**+---------------------------+**

###### &#x09;							**|       System Calls        |**

###### &#x09;							**+---------------------------+**

###### &#x09;							**|          Kernel           |**

###### &#x09;							**+---------------------------+**

###### &#x09;							**|         Hardware          |**

###### &#x09;							**+---------------------------+**







##### **1. Hardware Layer :** This is the physical part of the system :

###### 

###### &#x09;									CPU, RAM, disk, I/O devices

###### 

###### &#x09;									Linux directly interacts with hardware through the kernel











##### **2. Kernel (Core of Linux) :** The kernel is the heart of the OS. Linux kernel manages everything.





###### **Main functions:**



###### &#x09;	**a. Process management (creating, scheduling processes)**

###### 

###### &#x09;	**b. Memory management (RAM allocation)**

###### 

###### &#x09;	**c. Device drivers (control hardware)**

###### 

###### &#x09;	**d. File system management**

###### 

###### &#x09;	**e. Security \& permissions**

###### 

###### &#x20;**Example:** When you open a file, the kernel handles the request and fetches data from disk.

###### 







##### **3. System Calls : These act as an interface between user programs and the kernel.**



* ###### Applications can’t directly access hardware

###### 

* ###### They use system calls to request services

###### 

* ###### **Example :** open(), read(), write(), fork()







##### **4. Shell :** The shell is the command interpreter that allows users to interact with the OS.



###### **Popular shells :** Bash, Zsh



###### **Functions:**

###### 

* ###### Executes commands

###### 

* ###### Runs scripts



###### &#x09;	**Acts as a bridge between user and kernel**



###### &#x20;**Example :** ls -l







##### **5. User Applications : These are programs users interact with:**

##### 

* ###### Browsers, editors, games, compilers

###### 

* ###### Examples: Firefox, Vim













### &#x09;		**SCP vs RSYNC (Difference)**









###### **Feature			SCP			RSYNC**



###### Speed		Slower for large files		Faster (only changes copied)

###### Transfer type	Full copy every time		Incremental sync

###### Compression	Limited				Yes (-z)

###### Resume support	No				Yes

###### Efficiency	Low				High







##### 1\. **SCP (Secure Copy Protocol) :** scp is a simple tool used to copy files securely over SSH using the SSH.



###### Basic Syntax:

###### &#x09;	scp source destination



###### **Examples:** Copy file from local → remote

###### &#x09;				scp file.txt user@remote:/home/user/

###### &#x09;Copy file from remote → local

###### &#x09;				scp user@remote:/home/user/file.txt .

###### &#x09;Copy directory

###### &#x09;				scp -r folder user@remote:/home/user/



##### **Features:**



* ###### Simple and quick

###### 

* ###### Uses SSH for encryption

###### 

* ###### Copies entire file every time

###### 







##### **2. RSYNC (Remote Sync) :** rsync is a more advanced tool for syncing files and directories efficiently.



##### **Basic Syntax:**

###### &#x09;		rsync \[options] source destination

###### **Examples:**

###### &#x09;	Copy files locally

###### &#x09;				rsync -av file.txt /backup/

###### 

###### &#x09;	Copy local → remote

###### &#x09;				rsync -av file.txt user@remote:/home/user/

###### 

###### &#x09;	Sync directories

###### &#x09;				rsync -av folder/ user@remote:/home/user/folder/

###### 

###### **Important Options:**

###### 

###### &#x09;	-a → archive mode (preserves permissions)

###### 

###### &#x09;	-v → verbose

###### 

###### &#x09;	-z → compress during transfer

###### 

###### &#x09;	--delete → remove extra files in destination







* ##### **Shell Scripting :** A shell script is a text file containing commands that the shell executes line by line.



##### 



##### **Common shells :**

##### &#x09;	Bash (most popular), sh (Bourne shell), zsh, ksh.





* ###### **Create file:**

###### &#x09;		nano script.sh





* ###### **Make it executable:**

###### &#x09;		chmod +x script.sh





* ###### **Run:**

###### &#x09;		./script.sh









