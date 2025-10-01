---
Title: September - Week 1 - Detailed technical notes
Parent: September
---

# Detailed Technical Notes for Setting up alpha protoytpe server using Yunohost 

### Set up Lenovo Thinkstation
  
  - Plug in computer to battery inverter
    
  - Plug in ethernet cable between computer and router (Fritzbox)
    
  - Plug keyboard into computer
    
  - Plug screen into computer
    
### Set up hard drive as back up (Western Digital SSD via FritzBox SMB)
  
  - Plug in hard drive to battery inverter
    
  - Plug in hard drive to FritzBox (SMB USB port)
    
### Look up instructions for how to flash a Lenovo thinkstation
  
  - Found in this article: [How to Boot a Lenovo ThinkStation from a USB Drive](https://codingmall.com/knowledge-base/25-global/11961-thinkstation-boot-from-usb)
### Make computer bootable from usb drive
  
  - Access BIOS menu by holding down F12 when restarting
    
  - Disable secure boot
    
  - Restart
    
  - Adjust boot order of 'automatic boot sequence' so USB is on top
    
  - Restart
    
  - Adjust boot order of 'primary boot sequence' so USB is on top
    
  - Restart
    
  - Enable CSM 'compatibility support module'
    
  - Restart - success! booting from USB now appears as an option
    
### Set up yunohost on computer
  
  - Plug in yunohost flash drive
    
  - Restart computer holding down F12
    
  - Launch graphical install
    
  - Select location
    
  - Select language
    
  - Select language key mapping
    
  - Select partition disk option: "guided - use entire disk"
    
    - Error: "Failed to create a file system The ext4 file system creation in partition #1 of /dev/nvme0n1 failed."
  - In graphical interface, select button "go back"
    
  - Try other settings. Result: no success.
    
  - Abort install and reboot holding down F12
    
### Set up yunohost on computer Attempt 2
  
  - Restart computer holding down F12
    
  - Launch graphical install
    
    Select location
    
    Select language
    
    Select language key mapping
    
    Select partition disk option: "guided - use entire disk and set up LVM"
    
    - Error: "Failed to creat a file system...." - same as last time
  - Abort install
    
### Make computer bootable from usb drive - change settings
  
  - Restart computer holding down F12
    
  - Enter BIOS mode
    
  - In 'security' tab, change 'boot mode' to 'UEFI only'
    
  - Save and restart
    
    - Result: Bad, usb not recognised
  - Repeat steps but change mode to 'Legacy only'
    
    - Result: Bad, usb not recognised
  - Repeate steps and change mde back to 'Auto'
    
    - Result: good, USB appears in BIOS as boot option
### Look up how to fix issue of interrupted install on Yunohost forum
  
  - Result: suggest installing debian 12 on computer first
- Create flash usb Debian 12
  
  - Open BalenaEtcher
    
    - Error: flagged as malware
  - Troubleshoot malware flag
    
  - Re-download latest version of BalenaEtcher
    
  - Find an empty (DHSI) usb stick with enough storage to be a flashed image
    
  - Find link to Debian 12 (bookworm) ISO (Not easy! V hidden on Debian site)
    
    - Need amd64 version
  - Download debian 12 iso
    
  - Plub in USB stick
    
  - Open Balena Etcher
    
  - Follow instructions for making a flash
    
    - Error: can't make a flash disk without admin rights
  - Save Debian 12 iso to usb flash drive
    
  - Log out of regular account
    
  - Log in to admin account on laptop Rabbit Pro
    
  - Move debian 12 ISO to desktop
    
  - Open balena etcher
    
  - Flash debian 12 to usb flash drive
    
    - Result: success!
  - Log out of admin account
    
  - Log in to regular account 
    
### Install Debian on yunohost computer
  
  - Insert Debian flash drive into yunohost computer
    
  - Restart holding down F12
    
  - Select: 'UEFI USB drive'
    
  - Follow install prompts
    
    - Result: Success!
      
    - Debian machine name: debian
      
    - Debian machine domain name: dds.ive.centre
      
    - See 1password for full details
      
    - At last stage of install:
      
      - Deselect: debian desktop environment
        
      - Select: ssh server
        
- Save Debian details (logins, IP address etc) on 1password
