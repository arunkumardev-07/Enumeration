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
## output:
![Screenshot 2024-09-24 234019](https://github.com/user-attachments/assets/7922a691-840a-4ebc-a759-9e757ebb7e66)


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com
## output:
![img-2](https://github.com/user-attachments/assets/3ba7da04-c9fa-4c05-8b90-216242392641)






intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
## output:
![Screenshot 2024-09-24 234248](https://github.com/user-attachments/assets/2517f77c-cb36-419d-b58f-c4153ba0292c)



inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
## output:
![Screenshot 2024-09-24 234420](https://github.com/user-attachments/assets/753bd552-40c0-437e-ba0d-15a4f517c6b9)


intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
## output:
![Screenshot 2024-09-24 234545](https://github.com/user-attachments/assets/366566d4-5060-457a-ae65-26c64c224cbc)





link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
## output:
![Screenshot 2024-09-24 234545](https://github.com/user-attachments/assets/e3c1bd55-ffed-4224-8ee8-3b3c602c6cc2)



cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
## output:
![img-7](https://github.com/user-attachments/assets/fb7e7de7-40dc-4a6b-b85f-2e9737daffe0)


 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:
![img1](https://github.com/user-attachments/assets/7a78ffcb-380e-4bfb-a6d3-0a4c59295128)








##dnsenum
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
## output:
![img2](https://github.com/user-attachments/assets/0ac40e34-f74a-48dd-8733-13c5a7241992)


##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
## output:
![img-11](https://github.com/user-attachments/assets/1cd915fd-be1a-4297-8c7d-6cf9c0be1bb8)


select any username in the first column of the above file and check the same
![smtp userenum](https://github.com/user-attachments/assets/bbf86954-7774-4e64-aafb-f79d3fe0e63b)
![www data](https://github.com/user-attachments/assets/8f010d3f-a21d-4c65-88e8-17a0d922fbe9)




#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ## Output
![telnet](https://github.com/user-attachments/assets/263252fc-0b37-4401-8f8d-24f96d4bff11)

  
  

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:
![nmap](https://github.com/user-attachments/assets/69e263ef-69d1-4b1a-813a-3763eb010172)


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully
