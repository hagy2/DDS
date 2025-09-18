---
title: September — Week 2
---

# Week 2 — September

**Summary:**  
This week focused on .....

---

## ✅ Tasks Completed

- **Fine tuned documentation static site**  
  Adding links between static site and repo site.  

- **.  
  .  


- **Set up local Yunohost server | KJH**  
  Using a dedicated, refurbished tiny PC on a home network to host the test server.
  
  - Set up Lenovo mini PC & connect to router
    
  - Change BIOS settings on PC to allow flashing from USB
    
  - Make flash USB with Debian 12 Bullseye ISO
    
  - Make flash USB with Yunohost 12.12 ISO*
    *Note this step failed when I tried without installing Debian first
  - Flash PC with Debian from USB
    Following installation prompts in graphical install. Save Debian details in 1password project vault. 
  - Flash PC with Yunohost from USB
    Following installation prompts in graphical install. Save Yunohost details in 1password project vault
  - 

- **Set up local backup storage via SMB | KJH**

- **Set up shared project password store | KJH**
  Share details

- **Allow local Yunohost server required internet access | KJH**
  On router, opened local ports

---

## 📌 Notes
- **Setting up a Lenovo PC:**  
  Followed instructions here: [How to Boot a Lenovo ThinkStation from a USB Drive](https://codingmall.com/knowledge-base/25-global/11961-thinkstation-boot-from-usb)  

- **Flashing software ISOs to USB:**  
  Using FOSS Software Etcher in admin account of another computer. The process fails unless you are logged into an admin account.  

- **Installing Yunohost 12.12**  
  I tried installing Yunohost first, it failed part way through. Installing Yunohost was only successful after installing Debian first. It seems to be something about how the Lenovo PC interprets the formatting of the USB drive. Some USB drives/flashed ISOs are read by the BIOS as 'UEFI', some as 'Legacy', some appear as two drive options ie 'UEFI' and 'Legacy.' Choosing a 'UEFI' drive results in successful installation, chosing a 'Legacy' drive results in a failed install.

---

## 🧐 Rationale
- Why set up a local server for testing and alpha prototyping?  
  - Test the conditions
  
---
