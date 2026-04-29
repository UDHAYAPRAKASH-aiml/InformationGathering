# InformationGathering
Information Gathering Techiques

# To perform information gathering techniques

# AIM:

To perform information gathering techniques using kali linux 

## STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various categories of tools as follows:

### Step 3:
Open terminal/browser and try execute necessary commands/use url to perform information gathering

## Pen Test Tools Categories:  

Following Categories of pen test tools are identified for information gathering:

Footprinting is a part of the reconnaissance process which is used for gathering possible information about a target computer system or network.
http://www.whois.com/whois website to get detailed information about a domain name information including its owner, its registrar, date of registration, expiry, name server, owner's contact information, etc.

## OUTPUT:


## Finding IP address:
ping command is available on Windows as well as on Linux OS. Following is the example to find out the IP address of facebook.com.
##output

<img width="583" height="1007" alt="image" src="https://github.com/user-attachments/assets/4bdf3b09-4442-40cb-a0c9-21711e894570" />



## Finding Hosting Company
get further detail by using ip2location.com website.
## output
<img width="1127" height="1083" alt="image" src="https://github.com/user-attachments/assets/f54e7da3-e159-4d92-b4c4-0f8287a51dd5" />




## History of the website:
## output

<img width="1920" height="1077" alt="image" src="https://github.com/user-attachments/assets/20d1db98-e257-4545-87f8-4dfd2a3aee04" />



# Webserver Fingerprinting:

## Netcat:
sudo nc example.com 80
GET / HTTP/1.1
Host: example.com
<img width="649" height="549" alt="image" src="https://github.com/user-attachments/assets/509b0433-ef0c-4aed-a07c-6caf4f9fbe47" />



## nmap:
### output

<img width="649" height="238" alt="image" src="https://github.com/user-attachments/assets/0ec8acb7-6fac-484f-97e6-0b40fe06a55e" />



## Whatweb
### output
<img width="1718" height="177" alt="image" src="https://github.com/user-attachments/assets/a37b793f-4c94-4031-b6c0-95aa86438cc2" />


# Tracing the Location
TCP Traceroute:
sudo traceroute -T www.google.com
## output
<img width="680" height="100" alt="image" src="https://github.com/user-attachments/assets/9b8e1f7b-db76-43f5-9f6e-1148b1b55849" />


## UDP Traceroute:
sudo traceroute -U www.google.com
## output
<img width="680" height="534" alt="image" src="https://github.com/user-attachments/assets/6181c938-f1fd-4012-9bcc-b2969c2235ee" />




## ICMP Traceroute:
sudo traceroute  www.google.com
## output


<img width="617" height="548" alt="image" src="https://github.com/user-attachments/assets/3b78ccc5-b4e1-44ce-a8be-34b060855ded" />





## RESULT:
The information gathering techniques tools/procedure were  identified successfully
