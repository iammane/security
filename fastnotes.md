Pimp my Kali - https://github.com/Dewalt-arch/pimpmykali

Recon:

Hunter.io - emails<br>
Phonebook.cz - emails (need to sign up for account)<br>
Clearbit chrome extension - emails<br>
tools.verifyemailaddress.io -<br>
email-checker.net/validate - emails

Sublist3r - subdomain searching<br>
crt.sh - certificate search (%.domain.com)<br>
OWASP Amass - all of the above

builtwith.com - good, but A LOT OF information..<br>
Wappalyzer - website technology tool, browser extension<br>
whatweb - built into Kali (including the WSL version!!)

burp - duh. More to come

***

Scanning and enumeration:<br>
arp-scan -l - Run arp scan to match MAC address to IP<br>
nikto - Scan a website and runs vuln tests. Any site with good security will block this most likely.<br>
dirbuster - directory busting on http/s site, uses a word list to verify<br>
metasploit - various vuln / exploit framework<br>
searchsploit - offline searching of the metasploit framework<br>
nessus essentials - vuln scanner.

exploitation basics:<br>
msfconsole - as above<br>
hydra - brute force password - credential stuffing

Foxy Proxy - For Firefox, this makes switching proxy settings on/off VERY easy.

Web application enumeration:<br>
Assetfinder - like sublist3r but better, more modern. Finds domains and subdomaisn related to given domain. (sudo install assetfinder worked just fine...)<br>
amass - More domain finding, OWASP org tooling.<br>
httprobe - checks to see if domains respond<br>
subjack - check for subdomain takeover<br>
waybackurls - scan archive.org wayback machine for interesting things (various file extensions)<br>
gowitness / eyewitness - take screenshots of pages found (legion can also do this)

ccwillem/danglingdomains - CNAME checking, trying to look into this shortly... (seems to just crap out? needs a closer look).<br>
anshumanbh/tko-subs - also not working great, needs more research.<br>
Yahoo! SubdomainSleuth - https://github.com/yahoo/SubdomainSleuth - Looks like it runs analysis on a zone file offline (but queries active Internet resources). This might be helpful at some point but not right now.<br>

ysoserial -- must check into.

