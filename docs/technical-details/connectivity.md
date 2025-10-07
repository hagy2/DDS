---
title: connectivity details
parent: technical-details
nav_order: 3
---

# Connectivity

This page documents how the Yunohost server was connected to the internet and the challenges encountered.

## FritzBox settings
- Internet > Permit Access:
  - ✅ Internet access to the Fritz!Box via HTTPS enabled
  - ✅ Internet access to your storage media via FTP/FTPS enabled
- Internet > Account Information > DNS Server:
  - ✅ Use DNSv4 servers assigned by the ISP
  - ✅ Use DNSv6 servers assigned by the ISP
  - ✅ Fallback to public DNS servers when DNS disrupted
- Internet > Account Information > IPv6:
  - ✅ IPv6 support enabled
  - ✅ Use IPv6 with a tunnel protocol

Reference guides tested:
- [No access via port sharing to FRITZ! home network](https://en.avm.de/service/knowledge-base/dok/FRITZ-Box-7490/25_No-access-to-FRITZ-Box-over-the-Internet/)
- [Port forwarding troubleshooting (YunoHost forum)](https://forum.yunohost.org/)
- [Editing FritzBox config](https://online.osba.nl/blog/en/category/fritz/)

## Internet tools/checks
- Used **Open Port Check Tool** to verify if ports were open.
- Confirmed external access worked inconsistently.

## Yunohost interface
- Enabled UPnP.
- Updated system via `yunohost.local`.

## CLI configuration
Edited `/etc/network/interfaces` with:
