---
title: September — Week 2 - Detailed technical notes
parent: September
---

# Detailed technical notes on alpha prototype server setup

Connectivity

#### Server connectivity | FritzBox settings

- Fritzbox settings that work:
  
  - Under Internet > Permit Access:
    
    - tick 'Internet access to the Fritz!Box via HTTPS enabled'
      
    - tick 'Internet access to your storage media via FTP/FTPS enabled'
      
  - Under Internet > Account Information > DNS Server:
    
    - check 'Use DNSv4 servers assigned by the internet'
      
    - check 'Use DNSv6 servers assigned by the internet service provider'
      
    - tick 'Fallback to public DNS servers when DNS disrupted'
      
  - Under Internet > Account Information > IPV6
    
    - tick 'IPv6 support enabled'
      
    - check 'Use IPv6 with a tunnel protocol'
      
- Followed steps to change settings in this guide: [No access via port sharing to FRITZ! home network](https://fritz.com/service/wissensdatenbfank/dok/FRITZ-Box-7490/1083_Kein-Zugriff-uber-Portfreigabe-auf-FRITZ-Heimnetz/)
  
- Read this FritzBox related post: [Port forwarding trouble shooting - Support - YunoHost Forum](https://forum.yunohost.org/t/port-forwarding-trouble-shooting/13257)
  
- Followed these instructions: https://online.osba.nl/blog/en/category/fritz/ to try to edit the Fritzbox settings from a text file.
  
  - Result: no success.

#### Server connectivity | Internet tools/checks

- Used this tool to find out if the server was actually accessible to the internet through FritzBox [Open Port Check Tool - Test Port Forwarding on Your Router](https://www.yougetsignal.com/tools/open-ports/)

#### Server connectivity | Yunohost interface settings

- Enabled UPnP on Yunohost server
  
- Updated all packages and system on yunohost (connecting via yunohost.local)
  

#### Server connectivity | CLI Command Line Interface

- Added lines to document at etc/hosts/interfaces
  
  address xxx  
  netmask 255.255.255.0  
  gateway xxx  
  dns-nameservers xxx
  

#### Calculate reverse DNS via IPv6

ipv6: xxx

domain: xxx
