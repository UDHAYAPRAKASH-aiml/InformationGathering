# Enumeration
Enumeration Techniques

# Explore Google hacking and enumeration 

# AIM:

To use Google for gathering information and perform enumeration of targets

## STEPS:

### Step 1:

Install kali linux either in partition or virtual box or in live mode

### Step 2:

Investigate on the various Google hacking keywords and enumeration tools as follows:


### Step 3:
Open terminal and try execute some kali linux commands

## Pen Test Tools Categories:  

Following Categories of pen test tools are identified:
Information Gathering.

Google Hacking:

Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking:

## site: 
This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com
![WhatsApp Image 2025-03-10 at 11 37 57_d1c06e0a](https://github.com/user-attachments/assets/0e1d33c0-7a87-4ead-b4b3-303c1e867c26)


## filetype: 
This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com
![WhatsApp Image 2025-03-10 at 11 37 57_d73b9dcf](https://github.com/user-attachments/assets/5c1026cf-9b6a-423c-9935-0b38ae9afee0)



## intext: 
This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
![WhatsApp Image 2025-03-10 at 11 37 57_c9b66fb9](https://github.com/user-attachments/assets/2a3f06c0-1625-486e-a63e-93bf7601fcf2)



## inurl: 
This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
![WhatsApp Image 2025-03-10 at 11 37 57_e29dfd77](https://github.com/user-attachments/assets/93c34e18-f871-4413-92fd-7a50bd67de02)

## intitle: 
This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
![WhatsApp Image 2025-03-10 at 11 37 56_79425ee7](https://github.com/user-attachments/assets/440a074e-76c8-44bd-aba0-27de6f43ade7)

## cache: 
This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
![image](https://github.com/user-attachments/assets/2963d70f-51fb-4237-a072-aebaa615f5c1)

## link: 
This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
![image](https://github.com/user-attachments/assets/ee290eec-b405-4dd6-a940-8838bef3f49d)

 
### DNS Enumeration

## DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:
![Screenshot 2025-03-14 135719](https://github.com/user-attachments/assets/c2504f21-7b1c-4dfd-a092-78aa56602c8f)








## dnsenum
Dnsenum is a multithreaded perl script to enumerate DNS information of a domain and to discover non-contiguous ip blocks. The main purpose of Dnsenum is to gather as much information as possible about a domain. The program currently performs the following operations:

Get the host’s addresses (A record).
Get the namservers (threaded).
Get the MX record (threaded).
Perform axfr queries on nameservers and get BIND versions(threaded).
Get extra names and subdomains via google scraping (google query = “allinurl: -www site:domain”).
Brute force subdomains from file, can also perform recursion on subdomain that have NS records (all threaded).
Calculate C class domain network ranges and perform whois queries on them (threaded).
Perform reverse lookups on netranges (C class or/and whois netranges) (threaded).
Write to domain_ips.txt file ip-blocks.
This program is useful for pentesters, ethical hackers and forensics experts. It also can be used for security tests.
## OUTPUT 
![image](https://github.com/user-attachments/assets/23e199a9-cd1a-41c9-b58b-434b399e738b)
![image](https://github.com/user-attachments/assets/1f40320a-6c88-49ea-a0d0-0238bd8c186c)


## smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same
## OUTPUT:
![image](https://github.com/user-attachments/assets/4de173a5-1635-49aa-a4ad-18f4e14d4414)


## Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
## Output
![Screenshot 2025-03-14 145928](https://github.com/user-attachments/assets/11958490-af0c-4a2d-b567-abbd6d5b5e05)


  

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:

![image](https://github.com/user-attachments/assets/a2b10581-7b1a-4daf-9dd1-4119ca2caa30)

## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

