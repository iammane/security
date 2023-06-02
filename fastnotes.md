Pimp my Kali - https://github.com/Dewalt-arch/pimpmykali

Recon:

Hunter.io - emails\
Phonebook.cz - emails (need to sign up for account)\
Clearbit chrome extension - emails\
tools.verifyemailaddress.io -\
email-checker.net/validate - emails

Sublist3r - subdomain searching\
crt.sh - certificate search (%.domain.com)\
OWASP Amass - all of the above

builtwith.com - good, but A LOT OF information..\
Wappalyzer - website technology tool, browser extension\
whatweb - built into Kali (including the WSL version!!)

burp - duh. More to come

***

Scanning and enumeration:\
arp-scan -l - Run arp scan to match MAC address to IP\
nikto - Scan a website and runs vuln tests. Any site with good security will block this most likely.\
dirbuster - directory busting on http/s site, uses a word list to verify\
metasploit - various vuln / exploit framework\
searchsploit - offline searching of the metasploit framework\
nessus essentials - vuln scanner.

exploitation basics:\
msfconsole - as above\
hydra - brute force password - credential stuffing

Foxy Proxy - For Firefox, this makes switching proxy settings on/off VERY easy.

Web application enumeration:\
Assetfinder - like sublist3r but better, more modern. Finds domains and subdomaisn related to given domain. (sudo install assetfinder worked just fine...)\
amass - More domain finding, OWASP org tooling.\
httprobe - checks to see if domains respond\
subjack - check for subdomain takeover\
waybackurls - scan archive.org wayback machine for interesting things (various file extensions)\
gowitness / eyewitness - take screenshots of pages found (legion can also do this)

ccwillem/danglingdomains - CNAME checking, trying to look into this shortly... (seems to just crap out? needs a closer look).\
anshumanbh/tko-subs - also not working great, needs more research.\
Yahoo! SubdomainSleuth - https://github.com/yahoo/SubdomainSleuth - Looks like it runs analysis on a zone file offline (but queries active Internet resources). This might be helpful at some point but not right now.

