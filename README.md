# Enumeration
Enumeration Techniques

# Explore Google hacking and enumeration :

# AIM :

To use Google for gathering information and perform enumeration of targets.

## PROCEDURE :

### STEP 1 :

Install kali linux either in partition or virtual box or in live mode.

### STEP 2 :

Investigate on the various Google hacking keywords and enumeration tools as follows:

### STEP 3 :

Open terminal and try execute some kali linux commands.

## Pen Test Tools Categories :  

Following Categories of pen test tools are identified:

 Information Gathering.

### Google Hacking :

  Google hacking, also known as Google dorking, is a technique that involves using advanced operators to perform targeted searches on Google. These operators can be used to search for specific types of information, such as sensitive data that may have been inadvertently exposed on the web. Here are some advanced operators that can be used for Google hacking :

#### site : 

  This operator allows you to search for pages that are within a specific website or domain. For example, "site:example.com" would search for pages that are on the example.com domain.
Following searches for all the sites that is in the domain youtube.com

![image](https://github.com/Bharath745/Enumeration/assets/94508354/928c3bcd-89fe-443c-8ef2-67ef396e7570)


##### filetype : 

  This operator allows you to search for files of a specific type. For example, "filetype:pdf" would search for all PDF files.
Following searches for pdf file in the domain youtube.com

![image](https://github.com/Bharath745/Enumeration/assets/94508354/0721e4b6-4967-4786-b9d5-d479241aaf75)


#### intext : 

  This operator allows you to search for pages that contain specific text within the body of the page. For example, "intext:password" would search for pages that contain the word "password" within the body of the page.

![image](https://github.com/Bharath745/Enumeration/assets/94508354/5d808aab-b7b8-487c-baf9-634027c20d11)


#### inurl : 

  This operator allows you to search for pages that contain specific text within the URL. For example, "inurl:admin" would search for pages that contain the word "admin" within the URL.
  
![image](https://github.com/Bharath745/Enumeration/assets/94508354/e38ccec4-b404-4f2c-abe0-a7848fe87a30)


#### intitle :

  This operator allows you to search for pages that contain specific text within the title tag. For example, "intitle:index of" would search for pages that contain "index of" within the title tag.

![image](https://github.com/Bharath745/Enumeration/assets/94508354/7205092d-a7a8-489d-bd75-e1970d84cdc4)


#### link :

  This operator allows you to search for pages that link to a specific URL. For example, "link:example.com" would search for pages that link to the example.com domain.

![image](https://github.com/Bharath745/Enumeration/assets/94508354/57a7ff5d-c553-42b4-a176-0f99ebf96a56)


#### cache : 

  This operator allows you to view the cached version of a page. For example, "cache:example.com" would show the cached version of the example.com website.

![image](https://github.com/Bharath745/Enumeration/assets/94508354/1d871ebc-f303-4799-8a0c-573463a2d46c)


# DNS Enumeration :

## DNS Recon :

Provides the ability to perform:

Check all NS records for zone transfers

Enumerate general DNS records for a given domain (MX, SOA, NS, A, AAAA, SPF , TXT)

Perform common SRV Record Enumeration

Top level domain expansion

## OUTPUT :

![image](https://github.com/Bharath745/Enumeration/assets/94508354/a172151f-05e7-4892-8530-932c0d2c5c73)


![image](https://github.com/Bharath745/Enumeration/assets/94508354/6cd1b7bf-7eab-4c53-bb94-076983827933)


## dnsenum :

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

![image](https://github.com/Bharath745/Enumeration/assets/94508354/ec024f4c-0d9e-4ae3-a103-ce38fa1e289b)


## smtp-user-enum :

  Username guessing tool primarily for use against the default Solaris SMTP service. Can use either EXPN, VRFY or RCPT TO.
  
![image](https://github.com/Bharath745/Enumeration/assets/94508354/b7eec0c3-0289-40a8-b78d-37777b4c10bc)


  In metasploit list all the usernames using head /etc/passwd or cat /etc/passwd:

![image](https://github.com/Bharath745/Enumeration/assets/94508354/55d270b3-dc46-4d36-970b-64f83fbae381)


  Select any username in the first column of the above file and check the same
  
![image](https://github.com/Bharath745/Enumeration/assets/94508354/3d81c49d-e633-47ad-a23c-1dc4d58fb2a2)


# Telnet for smtp enumeration :

Telnet allows to connect to remote host based on the port no. For smtp port no is 25

telnet <host address> 25 to connect

and issue appropriate commands.
  
## Output :

![image](https://github.com/Bharath745/Enumeration/assets/94508354/8bcd108c-5901-4cc6-bd5d-c57144ad9e31)


## nmap –script smtp-enum-users.nse <hostname> :

  The smtp-enum-users.nse script attempts to enumerate the users on a SMTP server by issuing the VRFY, EXPN or RCPT TO commands. The goal of this script is to discover all the user accounts in the remote system.

## OUTPUT :

![image](https://github.com/Bharath745/Enumeration/assets/94508354/2c7b24c0-d52a-43fa-9b2e-dacc6c655b59)


## RESULT :

The Google hacking keywords and enumeration tools were identified and executed successfully.

