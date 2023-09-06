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

## Output

![image](https://github.com/Vasanthpushpa/Enumeration/assets/119291100/72ad5e2b-641f-4fc7-8540-fef3b84de636)


filetype: This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain yahoo.com

## Output

![image](https://github.com/Vasanthpushpa/Enumeration/assets/119291100/61fac389-5cd5-49d3-8b73-f9c611f91d58)


intext: This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

## Output

![image](https://github.com/Vasanthpushpa/Enumeration/assets/119291100/98a8b9a1-aff8-415f-8036-9b4dc75e6178)



inurl: This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.

## Output

![image](https://github.com/Vasanthpushpa/Enumeration/assets/119291100/dd72de28-c958-4d67-abed-710aa69462a7)


intitle: This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

## Output

![image](https://github.com/Vasanthpushpa/Enumeration/assets/119291100/c82c63d6-913a-4ee3-828d-ded6b6a4866f)


link: This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

## Output

![image](https://github.com/Vasanthpushpa/Enumeration/assets/119291100/ef0fc5b0-31c0-497a-b61c-6c2c81f36bbf)


cache: This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

## Output

![image](https://github.com/Vasanthpushpa/Enumeration/assets/119291100/eb7c5635-dce4-47f3-815d-89600cac8ccf)


 
#DNS Enumeration


##DNS Recon
provides the ability to perform:
Check all NS records for zone transfers
Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)
Perform common SRV Record Enumeration
Top level domain expansion
## OUTPUT:

![image](https://github.com/Vasanthpushpa/Enumeration/assets/119291100/514e6938-627b-456e-9629-fc6b714dbc0b)

![image](https://github.com/Vasanthpushpa/Enumeration/assets/119291100/4a85fc7d-674c-48d7-b79c-5676f5df2631)

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

## Output

![image](https://github.com/Vasanthpushpa/Enumeration/assets/119291100/f5e7b77a-408e-408b-9fae-d5da4f52ddbe)



##smtp-user-enum
Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.

![image](https://github.com/Vasanthpushpa/Enumeration/assets/119291100/3c4748cd-469a-448f-b586-0f17b013418a)


In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

![image](https://github.com/Vasanthpushpa/Enumeration/assets/119291100/2a09e248-65b7-4036-9842-803d15571679)


select any username in the first column of the above file and check the same

![image](https://github.com/Vasanthpushpa/Enumeration/assets/119291100/30d7ec60-5d58-41be-88f3-46a14d5fe2a7)


#Telnet for smtp enumeration
Telnet allows to connect to remote host based on the port no. For smtp port no is 25
telnet <host address> 25 to connect
and issue appropriate commands

## Output

![image](https://github.com/Vasanthpushpa/Enumeration/assets/119291100/46cdd6f6-fdf5-4439-a99e-15ca3bf46db8)

  
## nmap –script smtp-enum-users.nse <hostname>

The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.

## Output

![image](https://github.com/Vasanthpushpa/Enumeration/assets/119291100/17d9daaf-54c6-4da6-873d-43a296de085f)


## RESULT:
The Google hacking keywords and enumeration tools were identified and executed successfully

