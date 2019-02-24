# Information Gathering
- [ ] Harvesting public information
- [ ] Automated discovery
- [ ] Automated application discovery

### Harvesting public information

Command | Description
--------|------------
Go to [Shodan](https://www.shodan.io/) -> Insert company name or domain -> Search -> Results | Use Shodan to find public ip 
Go to [Arin.net](https://whois.arin.net/ui/query.do) -> Insert company name or domain -> Under the tab Network -> Net Range | Use American Registry for internet numbers
Go to [Hurricane Electric](https://bgp.he.net/) Insert company name or domain -> Search -> Results | Use the Internet Backbone and Colocation Provider


### Automated discovery

Command | Description
--------|------------
```amass -active -d {domain} -o {domains}.txt``` | Use active information gathering techniques to attempt DNS zone transfers on all discovered authoritative name servers and obtain TLS/SSL certificates for discovered hosts on all specified ports
```subfinder -b -d {domain} -o {domains.txt} ``` | SubFinder is a subdomain discovery tool that uses various techniques to discover 
```masscan -p0-p65535 {ip}``` | This is the fastest Internet port scanner. It can scan the entire Internet in under 6 minutes, transmitting 10 million packets per second.
```subover -l {domains.txt}``` | [sub-domain takeover](https://github.com/EdOverflow/can-i-take-over-xyz/tree/abd42ea0259877f877134375e75f157231e5697f)
```gowitness file -s {domains.txt} -T 20 && gowitness generate``` | gowitness is a website screenshot utility written in Golang, that uses Chrome Headless to generate screenshots of web interfaces using the command line. Both Linux and macOS is supported, with Windows support 'partially working'.



### Automated application discovery

Command | Description
--------|------------
[Burpsuite](https://github.com/Zawadidone/WebHacking/blob/master/BurpSuite/README.md) | Spider, scan, discover content and ..
```nmap -sV --script vulners <domain>``` | Scanning for services running on ports and comparing with the vulners database(cve's)
```nikto -h {domain} -C all``` | Scan for configurations ...
```gobuster -w {wordlist.txt} -s {status codes} -u {url}``` | Bruteforce directories use [Fuzzdb](https://github.com/fuzzdb-project/fuzzdb)
```linkfinder -i {url} -o results.html ``` | Find endpoints in JavaScript files  
```whatweb {domain}``` | Identify technology on websites without using a third-party ;)
```parameth -u {url}``` | This tool can be used to brute discover GET and POST parameters

### Technologies
In [Technologies](https://github.com/Zawadidone/WebHacking/tree/master/Technologies) there are tips and tricks for different technologies like Wordpress, Drupal, Jira and so on.


### Write ups :)
[LinkFinder](https://gerbenjavado.com/discovering-hidden-content-using-linkfinder/)

[Subdomain enumeration](http://10degres.net/subdomain-enumeration/)

[Pro tip collection](https://medium.com/@khaled.hassan/bugbountyprotip-collection-4a19e5b5b296)
