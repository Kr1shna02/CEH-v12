# Web server Concepts
## Web server Operations

![web](https://github.com/Kr1shna02/CEH-v12/assets/117007783/acd0ee6e-97d5-490a-8660-ac8b8c2651f5)
### Components of web server
+ Document Root -The document root is one of the root file directories of the web server that stores critical HTML files related to the web pages of a domain name, which will be sent in response to requests.

+ Server Root -It is the top-level root directory under the directory tree in which the server’s configuration and error, executable, and log files are stored. It consists of the code that implements the server.
  
+ Virtual Hosting -It is a technique of hosting multiple domains or websites on the same server
+ Web Proxy -A proxy server is located between the web client and web server. They are used to prevent IP blocking and maintain anonymity.

### open-source web server architecture 
![open](https://github.com/Kr1shna02/CEH-v12/assets/117007783/447d4ef1-b958-4253-be85-08a7c482ee66)
+ Linux - web server os
+ Apache - web server
+ Mysql -Database
+ php -backend connector
#### IIS Web Server Architecture
![iis](https://github.com/Kr1shna02/CEH-v12/assets/117007783/b239e9de-d899-41e2-87c0-8fe693cf804a)
The Internet Information Service (IIS) is a web server application developed by Microsoft for Windows. It supports HTTP, HTTPS,FTP, FTPS,SMTP and NNTP.t has several components, including a protocol listener such as HTTP.sys and services such as the World Wide Web Publishing Service (WWW Service) and Windows Process Activation Service (WAS).

## Web server Security Issues

![stack](https://github.com/Kr1shna02/CEH-v12/assets/117007783/1d5da0e0-3f9a-4269-b74c-45b78025e956)
### Impact of Web Server Attacks
+ Compromise of user accounts
+ Website defacement
+ Secondary attacks from the website
+ Root access to other applications or server
+ Data Tampering 
+ Data Theft
 
# Web Server attacks 
## DNS Server Hijacking

![dns hijack](https://github.com/Kr1shna02/CEH-v12/assets/117007783/e26b9c45-e713-452e-bcb8-d885112a6e00)

## DNS Amplification Attack

In this attack the attacker spoof dns request with victim IP and sends it to multiple DNS servers , which results in large amount dns replays to the victim causing DDOS.

![dns](https://github.com/Kr1shna02/CEH-v12/assets/117007783/1e1b480c-c150-4af1-8430-f779e51025fe)

![amp](https://github.com/Kr1shna02/CEH-v12/assets/117007783/4e7e56eb-c46c-4c70-8f8e-040ecf52bf6d)

## Directory Traversal Attacks

The design of web servers limits public access to some extent. Directory traversal is the exploitation of HTTP through which attackers can access restricted directories and execute commands outside the web server’s root directory by manipulating a Uniform Resource Locator (URL). In directory traversal attacks, attackers use the dot-dot-slash (../) sequence to access restricted directories outside the web server’s root directory. Attackers can use the trial-and-error method to navigate outside the root directory and access sensitive information in the system.

![dir](https://github.com/Kr1shna02/CEH-v12/assets/117007783/15a5bb02-275c-4d5e-b2cc-509fd5ed579a)

## Website Defacement
+ Website defacement refers to unauthorized changes made to the content of a single web page or an entire website, resulting in changes to the visual appearance of the web page or website.
+ Defaced pages expose visitors to propaganda or misleading information until the unauthorized changes are discovered and corrected. Attackers use a variety of methods, such as MySQL injection, to access a website to deface it. In addition to changing the visual appearance of the target website, attackers deface websites for infecting the computers of visitors by making the website vulnerable to virus attacks.

## Web Server Misconfiguration

 + Verbose debug/error messages
 + Anonymous or default users/passwords
 + Sample configuration and script files
 + Remote administration functions
 + Unnecessary services enabled
 + Misconfigured/default SSL certificates

## HTTP Response-Splitting Attack

+ In this attack, the attacker controls the input parameter and cleverly constructs a request header that elicits two responses from the server. The attacker alters a single request to appear as two requests by adding header response data into the input field.
+ Cross-site scripting (XSS), cross-site request forgery (CSRF), and Structured Query Language (SQL) injection are examples of this type of attack.

![ser](https://github.com/Kr1shna02/CEH-v12/assets/117007783/15e984a8-4281-432b-bfde-f4a944633670)

## Web Cache Poisoning Attack 

![ca](https://github.com/Kr1shna02/CEH-v12/assets/117007783/be0f44e8-f2da-4f50-866a-f1f54433ca2d)

## SSH Brute Force Attack

![ssh](https://github.com/Kr1shna02/CEH-v12/assets/117007783/94bef2df-778e-4bb6-876f-db3a7c52fdb6)

## DoS/DDoS Attacks

![d](https://github.com/Kr1shna02/CEH-v12/assets/117007783/33a7ac60-9224-432b-87f2-811f75e9a95e)

## Man -in Middle Attacks

![m](https://github.com/Kr1shna02/CEH-v12/assets/117007783/dc09d8a8-563c-44eb-924d-e1541c9a3724)

## Web application Attacks

+  Server-Side Request Forgery (SSRF) Attack
+  Parameter/Form Tampering
+  Cookie Tampering - Cookie-tampering attacks occur when a cookie is sent from the client side to the server.
+  Unvalidated Input and File Injection Attacks
+  Session Hijacking
+  SQL Injection Attacks
+  Directory Traversal
+  Cross-Site Scripting (XSS) Attacks
+  Command Injection Attacks

# Web Server Attack Methodology
+ Information Gathering
+ Web Server Footprinting
+ Website Mirroring
+ Vulnerability Scanning
+ Session Hijacking
+ Web Server Passwords Hacking

## Information Gathering
Information gathering tools
+ [who.is](https://who.is)
+ [Domain Dossier](https://centralops.net)
+ [Find Subdomains](https://pentest-tools.com)
  
## Information Gathering from Robots.txt File
A website owner creates a robots.txt file to list the files or directories a web crawler should index for providing search results. Poorly written robots.txt files can cause the complete indexing of website files and directories.

![p](https://github.com/kr1shna02/CEH-v12/assets/117007783/884d32fb-9577-406f-9c25-1ee52ee7cf26)

## Web Server Footprinting/Banner Grabbing
Tools
+ Netcat -netcat is a networking utility that reads and writes data across network connections by using the TCP/IP protocol.

![ser](https://github.com/kr1shna02/CEH-v12/assets/117007783/f4b24e81-f7d7-4bd5-88c0-562a3d780a76)

+ httprecon -httprecon is a tool for advanced web server fingerprinting. This tool performs banner-grabbing attacks, status code enumeration, and header ordering analysis on the target web server and provides accurate web server fingerprinting information.

![m](https://github.com/kr1shna02/CEH-v12/assets/117007783/0bf7e244-46d2-45b6-a600-f4f9e028cf40)

+ ID Serve -ID Serve is a simple Internet server identification utility.
  
  ![id](https://github.com/kr1shna02/CEH-v12/assets/117007783/219794ec-4e0f-451b-8993-d26e71246390)

## Enumerating Web Server Information Using Nmap
+ Discover virtual domains with hostmap:
  ```
  nmap --script hostmap <host>
  ```
+ Detect a vulnerable server that uses the TRACE method:
  ```
  nmap --script http-trace -p80 localhost
  ```
+ Harvest email accounts with http-google-email:
  ```
  nmap --script http-google-email <host>
  ```
+ Enumerate users with http-userdir-enum:
```
  nmap -p80 --script http-userdir -enum localhost
```
+ Detect HTTP TRACE:
```
  nmap -p80 --script http-trace <host>
```
+ Check if the web server is protected by a web application firewall (WAF) or IPS:
```
  nmap -p80 --script http-waf-detect --script-args=”http-waf-detect.uri=/testphp.vulnweb.com/artists.php,http-waf-detect.detectBodyChanges” www.modsecurity.org
```
+ Enumerate common web applications
```
  nmap --script http-enum -p80 <host>
```
+ Obtain robots.txt
```
  nmap -p80 --script http-robots.txt <host>
```
## Finding Default Credentials of Web Server 

![q](https://github.com/kr1shna02/CEH-v12/assets/117007783/ede898a8-979d-4f39-a53a-abc3b022f679)

## Finding Default contents of Web Server
+ Administrators debug and test functionality
+ Sample functionality to demonstrate common tasks
+ Publicly accessible powerful functions
+ Server installation manuals

Tools

Nikto -  is a vulnerability scanner used extensively to identify potential vulnerabilities in web applications and web servers.

![w](https://github.com/kr1shna02/CEH-v12/assets/117007783/25a18254-8d05-439a-b3b5-9ad90bd1cee3)

## Finding Directory Listings of Web Server

When a web server receives a request for a directory, rather than a file, the web server responds to the request in the following ways. 
+ Return Default Resource within the directory
+ Return Error
+ Return listing of directory content
Tool:

Dirhunt - is a web crawler optimized for searching and analyzing directories.

![d](https://github.com/kr1shna02/CEH-v12/assets/117007783/1d28eb94-4d6f-443b-af12-5312822922ec)



