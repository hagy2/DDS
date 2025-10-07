---
title: alpha prototupe server details
parent: technical-details
nav_order: 1
---

# Detailed Technical Notes on Alpha Prototype Server Setup

## Connectivity

### Server connectivity | FritzBox settings
Fritzbox settings that work:

- **Internet > Permit Access**
  - ✅ Internet access to the Fritz!Box via HTTPS enabled  
  - ✅ Internet access to your storage media via FTP/FTPS enabled  

- **Internet > Account Information > DNS Server**
  - ✅ Use DNSv4 servers assigned by the internet  
  - ✅ Use DNSv6 servers assigned by the internet service provider  
  - ✅ Fallback to public DNS servers when DNS disrupted  

- **Internet > Account Information > IPv6**
  - ✅ IPv6 support enabled  
  - ✅ Use IPv6 with a tunnel protocol  

References followed:
- Guide: *No access via port sharing to FRITZ! home network*  
- Post: *Port forwarding troubleshooting – Support – YunoHost Forum*  
- Instructions: [Online OSBA Fritzbox settings](https://online.osba.nl/blog/en/category/fritz/)  

**Result:** No success yet.

---

### Server connectivity | Internet tools/checks
- Used: **FritzBox Open Port Check Tool** to test if server is reachable.  

---

### Server connectivity | YunoHost interface settings
- Enabled **UPnP** on YunoHost server.  
- Updated all packages and system on YunoHost (`yunohost.local`).  

---

### Server connectivity | CLI (Command Line Interface)
Edited `/etc/hosts/interfaces` with:

