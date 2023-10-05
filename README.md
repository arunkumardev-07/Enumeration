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
![image](https://github.com/LOKESHKUMARPANCHATCHARAM/Enumeration/assets/119644432/84407220-c45f-4688-b102-4ec363381d14)


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com
## output:
![image](https://github.com/LOKESHKUMARPANCHATCHARAM/Enumeration/assets/119644432/88e8678b-c7a5-4653-b2c8-3b51677321ca)





intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.
## output:
![image](https://github.com/LOKESHKUMARPANCHATCHARAM/Enumeration/assets/119644432/a8a581ff-24ac-467f-a702-0231b9651f32)




inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
## output:
![image](https://github.com/LOKESHKUMARPANCHATCHARAM/Enumeration/assets/119644432/051be651-4bff-4c62-a848-60332aae5f32)



intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.
## output:
![image](https://github.com/LOKESHKUMARPANCHATCHARAM/Enumeration/assets/119644432/c0ce3ec0-9487-4ff6-9139-bb8284506dd6)



link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.
## output:
![image](https://github.com/LOKESHKUMARPANCHATCHARAM/Enumeration/assets/119644432/1560196c-b109-45d7-a9d5-2862cf6aceac)


cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.
## output:
![image](https://github.com/LOKESHKUMARPANCHATCHARAM/Enumeration/assets/119644432/7fb5164d-debd-48a3-a354-c47db752c2bd)



 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:
![image](https://github.com/LOKESHKUMARPANCHATCHARAM/Enumeration/assets/119644432/128e514a-ef6e-4152-ac53-0851e0348b14)
![image](https://github.com/LOKESHKUMARPANCHATCHARAM/Enumeration/assets/119644432/6eb179ae-ea25-4629-a48a-411a305ef176)







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
![image](https://github.com/LOKESHKUMARPANCHATCHARAM/Enumeration/assets/119644432/30cfc394-1508-47fc-9928-79590a7d0a0b)



##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
## output:
![image](https://github.com/LOKESHKUMARPANCHATCHARAM/Enumeration/assets/119644432/797cf17c-c01d-4fa1-acbe-741e7ff46712)



In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:
![image](https://github.com/LOKESHKUMARPANCHATCHARAM/Enumeration/assets/119644432/f7195cc1-9efa-49a1-8f35-c5e1b374513d)


select any username in the first column of the above file and check the same
![image](https://github.com/LOKESHKUMARPANCHATCHARAM/Enumeration/assets/119644432/a3bbfbb3-3f20-4383-9364-a4a13cad8214)



#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands
  
 ## Output
![image](https://github.com/LOKESHKUMARPANCHATCHARAM/Enumeration/assets/119644432/c2d3a90c-ceaf-41a2-a3e3-88ca32fe8782)

  
  

## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.


## OUTPUT:
![image](https://github.com/LOKESHKUMARPANCHATCHARAM/Enumeration/assets/119644432/aba0a481-25f4-4f61-aee0-acb8d9aea488)


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully
