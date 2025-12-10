---
title: September — Week 2
parent: September
---

# Week 2 — September 21-27, 2025

**Summary:**  
This week focused on three main areas:  
1. Continuing technical setup work for the local Yunohost server (hardware, flashing, backups, passwords).  
2. Starting the first review of Yunohost applications through the demo environment, especially testing **categorical filters** and **keyword search accuracy**.  
3. Announcing the project on the Yunohost community forum to begin building awareness and collaboration.  

---

## ✅ Tasks Completed

- **Fine tuned documentation static site**  
  Adding links between static site and repo site.  

- **Set up local Yunohost server**  
  Using a dedicated, refurbished tiny PC on a home network to host the test server.
  
  - Set up Lenovo mini PC & connect to router  
  - Change BIOS settings on PC to allow flashing from USB  
  - Make flash USB with Debian 12 Bullseye ISO  
  - Make flash USB with Yunohost 12.12 ISO*  
    *Note: This step failed when I tried without installing Debian first*  
  - Flash PC with Debian from USB (graphical install, details saved in 1Password vault)  
  - Flash PC with Yunohost from USB (graphical install, details saved in 1Password vault)  

- **Set up local backup storage via SMB**  

- **Set up shared project password store**  
  Share details  

- **Allow local Yunohost server required internet access**  
  On router, opened local ports  

- **Reviewed Yunohost apps via demo site**  
  - Tested **categorical filters** (Synchronization, Communication, Office, Productivity, Social Media, etc.)  
  - Tested **keyword search** (email, mail, calendar, contacts, files, drive, CRM, PKM, chat, docs, password manager).  
  - Documented mismatches, missing apps, and synonym gaps (e.g. “email” vs “mail,” “PKM” shows nothing, “events” shows nothing).  

- **Announced the project on Yunohost forums**  
  - Shared the project goals and description.   
  - Started building visibility and potential for community input and collaboration.  

- **Complete base Yunohost setup**
  - Problem solve outstanding issues
    - server/router IP mismatch
    - web not reachable
    - dns issues
    - Router <> Yunohost compatibility
   
- **Create backup account**
  Set up BorgBase for backups
  
---

## 📌 Notes

- **Server Setup (Lenovo PC):**  
  Followed instructions here: [How to Boot a Lenovo ThinkStation from a USB Drive](https://codingmall.com/knowledge-base/25-global/11961-thinkstation-boot-from-usb).  

- **Flashing ISOs:**  
  Used FOSS Software Etcher in admin mode. Non-admin attempt failed.  

- **Installing Yunohost 12.12:**  
  Yunohost install only worked after first installing Debian. Likely an issue with how Lenovo BIOS interprets UEFI vs Legacy USB. UEFI worked, Legacy failed.  

- **App Review (Demo environment):**  
  - Categorical filters: generally accurate but sometimes overlapping (e.g. Office vs Productivity). Some apps lacked descriptions.  
  - Keyword search: very sensitive to exact terms. Some important apps missing under common words. Suggest metadata improvements.  

- **Community engagement:**  
  Early outreach via the Yunohost forum helps align the project with community needs and highlights accessibility priorities from the start.  

---

## 🧐 Rationale

- **Why set up a local server?**  
  To provide a realistic environment for alpha prototyping and accessibility testing.  

- **Why review apps now?**  
  Early testing helps identify gaps in categories, metadata, and usability — critical for making the system more accessible for disabled users.  

- **Why engage with the Yunohost community?**  
  Open source projects thrive on collaboration, and feedback from existing Yunohost users will guide better adaptation for accessibility.  

---
