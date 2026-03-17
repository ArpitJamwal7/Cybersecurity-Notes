# &#x09;				Linux











* ###### **Linux** is an **open-source OS kernel** created by **Linus Torvalds** in **17-sep-1991.**

###### 

* ###### It is free, secure, stable, and customizable.

###### 

* ###### **Example:-**   Ubuntu, Debian, Fedora Linux, Kali Linux.











#### **Features of Linux :-**



###### &#x09;	Open source, Multi-user system, Multitasking, Strong security, Highly customizable, Supports networking, Stable and reliable.





#### 

#### **Linux File System (hierarchy) :-**



###### &#x09;				Linux uses a hierarchical directory structure starting from the root /.





###### **Directory	Purpose**



###### /		Root directory (single root directory)

###### /home		User files

###### /bin		Basic user commands

###### /etc		Configuration files

###### /var		Log files and variable data

###### /tmp		Temporary files

###### /usr		User programs

###### /def		device files (hardware files like ubantu, usb, printer, etc drivers)

###### /s bin		System bin (system maintenance e.g reboot)

###### /mnt 		For you to mount things manually

###### /media		where the system mounts removable media

###### /opt		optional apk 3rd party















#### 

#### Basic Linux Commands :-









* #### Directory Commands :-



###### **Command		Description			Example**



###### pwd		Show current directory		pwd

###### ls		List files and folders		ls

###### ls -l		Detailed file list		ls -l

###### ls -a		Show hidden files		ls -a

###### cd		Change directory		cd Documents

###### cd ..		Go back one directory		cd ..

###### mkdir		Create directory		mkdir test

###### rmdir		Remove empty directory		rmdir test











##### 

* #### **File Commands :-**





###### **Command		Description					Example**



###### touch		Create empty file				touch file.txt

###### cp		Copy file					cp file.txt newfile.txt

###### mv		Move or rename file				mv file.txt new.txt

###### rm		Delete file					rm file.txt

###### rm -r		Delete directory				rm -r folder

###### rm -v		prints a message for every file removed		rm -v file.txt

###### rm -f		force delete without prompt			rm -f file.txt

###### rm -i 		ask before deleting				rm -i file.txt













* #### **File Viewing Commands :-**





###### **Command		Description**

###### 

###### cat file.txt	Show file content

###### less file.txt	View large file

###### more file.txt	View file page by page

###### head file.txt	Show first 10 lines

###### tail file.txt	Show last 10 lines















#### &#x09;**File Permission Commands :-**





* ##### **Types of Permissions:-**





###### **Permission	Symbol		Meaning**



###### Read		r		View file content

###### Write		w		Modify the file

###### Execute		x		Run the file as a program

###### 

###### 









* ##### **Permission Groups :-**

###### 

###### 

###### **User Type	Symbol		Description**

###### 

###### Owner		u		Person who created the file

###### Group		g		Users in the same group

###### Others		o		All other users













###### **Command		Description**

###### 

###### chmod		Change file permission		chmod permission filename (chmod 755 script.sh)

###### chown		Change file owner

###### 

###### 

###### 

###### 

* ##### **Symbolic Method :-**

###### 

###### 

###### 

###### **Symbol		Meaning**

###### 

###### \+		Add permission			chmod +x file.sh

###### \-		Remove permission		chmod -w file.txt

###### =		Set exact permission		chmod \[who]=\[permissions] filename

###### 

###### 

###### 

* ##### **Permission Numbers :-**

###### 

###### 

###### 

###### **Permission	Value**



###### r		4

###### w		2

###### x		1

###### 

##### 

##### 

##### &#x09;**Example:-**

###### 

###### &#x09;		**Permission	Calculation	Value**

###### 

###### &#x09;		rwx		4+2+1		  7

###### &#x09;		rw-		4+2		  6

###### &#x09;		r-x		4+1		  5

###### &#x09;		r--		4		  4

###### 

###### 

###### 

###### 







* ##### **User Management Commands :-**

###### 

###### 

###### **Command		Description**

###### 

###### adduser		Add user

###### useradd		Add user

###### passwd		Change password

###### userdel		Delete user

###### su		switch user

###### exit		logout

###### group add	add group

###### gshadow		Admin Properties

###### group add	add group

###### sudo reboot	done by admin

###### user mod	rename user

###### 

###### 

###### 





###### 

###### 

* #### **Process Management :-**

###### 

###### 

###### **Command		Description**

###### 

###### ps		Show running processes

###### top		Monitor system processes

###### kill		Stop process

###### 

###### 

###### 





###### 

###### 

* ##### **Package Management :-**

###### &#x09;			sudo apt update

###### &#x09;			sudo apt install <package\_name>

###### 

###### 

###### 

###### 

###### 

##### **Advantages of Linux :-**

###### 

* ###### Free to use

###### 

* ###### Secure from viruses

###### 

* ###### Good for servers and developers

###### 

* ###### Customizable.











* #### **Access Control List (ACL) :-**

###### &#x09;				list of rules used to allow or deny access to a resource (file, system, or network).







##### **Purpose :**



* ###### Control who can access what

###### 

* ###### Improve security

###### 

* ###### Restrict unauthorized users

###### 







##### **Types of ACL :-**





1. ##### **File System ACL**

###### 

###### a. Used in Linux/Windows

###### b. Controls access to files/directories







2. ##### **Network ACL**

###### 

###### a. Used in routers/firewalls

###### b. Controls traffic based on:

* ###### IP address
* ###### Port
* ###### Protocol











* ##### &#x20;**setfacl (to set ACL) :**

###### &#x09;				setfacl -m u:<user, group>:<permissions> file





* ##### **getfacl (to view ACL) :**

###### &#x09;				**getfacl file/directory**







###### **Command		Purpose**



###### getfacl file	View ACL

###### setfacl -m	Add/modify ACL

###### setfacl -x	Remove specific ACL

###### setfacl -b	Remove all ACL













##### **Regular Expressions :-**

###### &#x09;		pattern used to search, match, and manipulate text.

###### &#x09;		Used in tools like **grep, sed, awk**, programming languages, etc.

###### 

###### 

###### **grep :**

###### &#x09;grep "^root" /etc/passwd

###### 

###### **sed :**

###### &#x09;sed 's/old/new/' file.txt

###### 

###### **awk :**

###### &#x09;awk '/pattern/ {print}' file.txt











##### **Word Count \& Line Count :**



###### wc -l →  lines

###### 

###### wc -w →  words

###### 

###### wc -c →  bytes

###### 

###### wc    →  all counts





















##### **Job Automation :**

###### &#x09;		Job automation in Linux means scheduling tasks to run automatically at a specific time or interval without manual intervention.









##### **a. cron :** cron is a service used to schedule recurring tasks.



###### **Syntax (crontab) :**

###### &#x09;		\* \* \* \* \* command





###### **Format :**

###### &#x09;	minute hour day month day\_of\_week command

###### 

###### 

###### **Example :**

###### &#x09;	0 2 \* \* \* backup.sh

###### 

###### 

###### **Schedule	Meaning**

###### 

###### \* \* \* \* \*	Every minute

###### 0 \* \* \* \*	Every hour

###### 0 0 \* \* \*	Every day at midnight

###### 0 0 \* \* 0	Every Sunday





###### **commands :**	crontab -e   # edit cron jobs

###### &#x09;	crontab -l   # list cron jobs

###### &#x09;	crontab -r   # remove cron jobs











##### **b. at (One-time job) :** Used to schedule a one-time task.





###### **Syntax :**

###### &#x09;	at <time>

###### 

###### **Example :**

###### &#x09;	at 10:00

###### 

###### &#x09;			echo "Hello" > file.txt













