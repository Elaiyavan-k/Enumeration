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

site: This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain yahoo.com
<img width="942" height="1052" alt="Screenshot 2026-02-06 081824" src="https://github.com/user-attachments/assets/2e88e987-2453-4815-8298-729ba45f5b12" />

filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com
<img width="942" height="1045" alt="Screenshot 2026-02-06 082303" src="https://github.com/user-attachments/assets/510e15e6-f0c4-4dfd-9eac-18276de7d4e2" />



intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
<img width="938" height="351" alt="Screenshot 2026-02-06 082402" src="https://github.com/user-attachments/assets/7389b08b-9bf9-46ea-8bad-db59c6273fdb" />


inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
<img width="904" height="1041" alt="Screenshot 2026-02-06 082535" src="https://github.com/user-attachments/assets/d4348f8f-83f8-47ac-a9e8-6988dac38eeb" />
<img width="924" height="1033" alt="Screenshot 2026-02-06 082424" src="https://github.com/user-attachments/assets/dd75516d-e933-43bd-9ec6-a2c90ca732f3" />

intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

<img width="923" height="1041" alt="image" src="https://github.com/user-attachments/assets/7c53d8cb-757f-416a-865b-232149d3761f" />


link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
<img width="932" height="1049" alt="Screenshot 2026-02-06 082615" src="https://github.com/user-attachments/assets/bde64b42-0df0-4654-897d-c41dadd0e443" />

cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

# DNS Enumeration


## DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:


<img width="942" height="266" alt="Screenshot 2026-02-06 083006" src="https://github.com/user-attachments/assets/b34875f6-1b97-4150-b338-e18a0c56a07a" />





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

<img width="930" height="636" alt="Screenshot 2026-02-06 083226" src="https://github.com/user-attachments/assets/4dd3d281-6653-4b99-8036-b777f3ca8f83" />


## smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

select any username in the first column of the above file and check the same

<img width="658" height="298" alt="Screenshot 2026-02-06 084302" src="https://github.com/user-attachments/assets/5ea5c1b3-3dba-415e-8b11-b56db6a9fd40" />


# Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ## Output
 <img width="518" height="86" alt="Screenshot 2026-02-06 084356" src="https://github.com/user-attachments/assets/7fc00197-aafc-4911-ad6e-f3f1a7a23842" />

  

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:
<img width="615" height="178" alt="Screenshot 2026-02-06 084451" src="https://github.com/user-attachments/assets/83e2ccf2-bf6d-4cc4-a123-89ff38168d58" />


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

