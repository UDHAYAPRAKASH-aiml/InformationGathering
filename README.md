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

### Description of the Output:
Pinging facebook.com [157.240.22.35] → Shows the domain name and its resolved IP address.

bytes=32 → Size of the data packet sent.

time=25ms → Time taken for the packet to travel to the server and back (latency).

TTL=56 → Time To Live value, indicating how many hops the packet can take before being discarded.

Multiple replies indicate a successful connection with the server.

## Finding Hosting Company
get further detail by using ip2location.com website.
## output
<img width="1127" height="1083" alt="image" src="https://github.com/user-attachments/assets/f54e7da3-e159-4d92-b4c4-0f8287a51dd5" />
## Description of the Output

- **IP Address**: Shows the unique numerical address of the server associated with the domain.  
- **Country / Region / City**: Indicates the physical location of the hosting server.  
- **ISP (Internet Service Provider)**: Displays the organization providing internet or hosting services.  
- **Domain Name**: The queried website name linked to the IP address.  
- **Latitude & Longitude**: Represents the geographical coordinates of the server location.  
- **ZIP Code / Time Zone**: Provides additional regional and time-related information.  
- **Hosting Provider**: Identifies the company responsible for hosting and maintaining the website.  



## History of the website:
## output

<img width="1920" height="1077" alt="image" src="https://github.com/user-attachments/assets/20d1db98-e257-4545-87f8-4dfd2a3aee04" />



## Description of the Output

- **Timeline / Calendar View**: Displays different years and dates when snapshots of the website were recorded.  
- **Snapshots (Captures)**: Shows how the website looked at specific points in time.  
- **Frequency of Captures**: Indicates how often the website was archived or updated.  
- **Changes Over Time**: Helps in identifying design, content, or structural changes in the website across different periods.  
- **Availability of Data**: Highlights which dates have stored versions and which do not.

# Webserver Fingerprinting:

## Netcat:
sudo nc example.com 80
GET / HTTP/1.1
Host: example.com
<img width="649" height="549" alt="image" src="https://github.com/user-attachments/assets/509b0433-ef0c-4aed-a07c-6caf4f9fbe47" />


## Description of the Output
- **HTTP Response Headers**: Shows server response including status code (e.g., 200 OK).  
- **Server Information**: May reveal web server type (e.g., Apache, Nginx).  
- **Content Response**: Displays raw HTML or webpage content returned by the server.  
- **Connection Status**: Confirms successful communication with the target server.


## nmap:
### output

<img width="649" height="238" alt="image" src="https://github.com/user-attachments/assets/0ec8acb7-6fac-484f-97e6-0b40fe06a55e" />


## Description of the Output
- **Open Ports**: Lists active ports (e.g., 80, 443).  
- **Service Detection**: Identifies services running on those ports.  
- **Version Information**: Provides details about service versions if detected.  
- **Host Status**: Confirms whether the target host is up or reachable. 


## Whatweb
### output
<img width="1718" height="177" alt="image" src="https://github.com/user-attachments/assets/a37b793f-4c94-4031-b6c0-95aa86438cc2" />


## Description of the Output
- **Web Technologies**: Identifies technologies used (e.g., CMS, frameworks).  
- **Server Details**: Shows web server type and configuration.  
- **IP Address**: Displays the resolved IP of the target website.  
- **Security Headers / Plugins**: Detects additional components and configurations.  


# Tracing the Location
TCP Traceroute:
sudo traceroute -T www.google.com
## output
<img width="680" height="100" alt="image" src="https://github.com/user-attachments/assets/9b8e1f7b-db76-43f5-9f6e-1148b1b55849" />


## Description of the Output
- **Hop-by-Hop Path**: Displays each router between source and destination.  
- **Latency (ms)**: Shows time taken for each hop.  
- **TCP Method**: Uses TCP packets, useful when ICMP is blocked.  


## UDP Traceroute:
sudo traceroute -U www.google.com
## output
<img width="680" height="534" alt="image" src="https://github.com/user-attachments/assets/6181c938-f1fd-4012-9bcc-b2969c2235ee" />

## Description of the Output
- **Network Path**: Lists intermediate routers using UDP packets.  
- **Response Time**: Indicates delay for each hop.  
- **Packet Filtering Insight**: Helps detect firewalls blocking certain traffic. 



## ICMP Traceroute:
sudo traceroute  www.google.com
## output


<img width="617" height="548" alt="image" src="https://github.com/user-attachments/assets/3b78ccc5-b4e1-44ce-a8be-34b060855ded" />

## Description of the Output
- **Default Method**: Uses ICMP echo requests to trace route.  
- **Hop Count**: Shows number of routers to destination.  
- **Timeouts (*)**: Indicates no response from a hop (possible filtering).  
- **Latency Measurement**: Displays round-trip time for each hop.  



## RESULT:
The information gathering techniques tools/procedure were  identified successfully
