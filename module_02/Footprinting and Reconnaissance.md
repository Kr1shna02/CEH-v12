# Footprinting Concepts
Footprinting is used to gather maximum information of the computer system or the servers or persons we are going to attack.

## Types :
+ Active Footprinting
+ Passive Footprinting

## Information Obtained in Footprinting:
+ Organization Information - employee details, contact nos, about organisation etc.
+ Network Information - Domain and sub-domains, Network blocks, Network topology, trusted routers, and firewalls, Whois records o DNS records and related information
+ System Information - OS, webservers, technology's and applications used.

## Footprinting Methodology
![alter txt](https://github.com/Kr1shna02/CEH-v12/blob/main/images/footprinting.png)

# Footprinting through Search Engines
operator:serach_term
Any Keyword can be specified before the operator.It is used to search for particular keyword in the particular searh query.
+ site -This operator restricts search results to the specified site or domain.
    - games site: www.certified.com
    
+ allinurl -This operator restricts results to only the pages containing all the query terms specified in the URL.
    - allinurl: google career   
+ inurl -This operator restricts the results to only the pages containing the specified word in the URL.
    - inurl: copy site:www.google.com

+ allintitle -All Query in Page title
    - allintitle: detect malware
+ intitle - This operator restricts results to only the pages containing the specified term in the title
    - intitle: help
+ inanchor - Search page contain specified word in the anchor link.
    - antivirus inachor: norton
+ allinanchor- Search page contain all the specified terms in anchor link.
    - allinanchor: best cloud service provider
+ cache: Display google cached version of the webpage.
    - cache:www.ef.org
+ link
+ related
+ info
+ location
+ filetype
