 Target: https://www.bridgeapi.io/

 Tools & Techniques

1. Whois
Using command: whois bridgeapi.io
Findings:
Domain Name: bridgeapi.io
Registry Domain ID: fd64e3652b0b4b91900fa6f1fae4e1bf-DONUTS
Registrar WHOIS Server: whois.gandi.net
Registrar URL: https://www.gandi.net
Updated Date: 2025-03-17T09:23:12Z
Creation Date: 2017-05-03T16:02:51Z
Registry Expiry Date: 2026-05-03T16:02:51Z
Registrar: Gandi SAS
Registrar IANA ID: 81
Registrar Abuse Contact Email: abuse@support.gandi.net
Registrar Abuse Contact Phone: +33.170377661
Domain Status: clientTransferProhibited https://icann.org/epp#clientTransferProhibited


2. Dig
Using command: dig +short bridgeapi.io
Findings:
75.2.70.75
99.83.190.102

3. NSLookup
Using command: nslookup bridgeapi.io
Findings:
Server:		192.168.29.1
Address:	192.168.29.1#53

Non-authoritative answer:
Name:	bridgeapi.io
Address: 75.2.70.75
Name:	bridgeapi.io
Address: 99.83.190.102

4. Shodan 
Search this ip: 99.83.190.102

Hostnames
aacb0a264e514dd48.awsglobalaccelerator.com
camdenbuildersinc.com

                awsglobalaccelerator.com
 Domains
                camdenbuildersinc.com
 
Cloud Provider- Amazon_
Cloud Region   -GLOBAL_
Cloud Service  -GLOBALACCELERATOR_
Country       - United States_
City           -Seattle_
Organization   -Amazon.com, Inc_
ISP            -Amazon.com, Inc_
ASN            -AS16509.


## Basic Automation Scripts
### Bash Script: gather_info.sh
#!/bin/bash
DOMAIN="bridgeapi.io"

echo "[*] WHOIS:"
whois $DOMAIN

echo "[*] DIG:"
dig $DOMAIN any

echo "[*] NSLOOKUP:"
nslookup $DOMAIN

### Python Script: gather_info.py
import os
import subprocess

domain = "bridgeapi.io"

print("[*] WHOIS")
subprocess.run(["whois", domain])

print("\n[*] DIG")
subprocess.run(["dig", domain, "any"])

print("\n[*] NSLOOKUP")
subprocess.run(["nslookup", domain])
