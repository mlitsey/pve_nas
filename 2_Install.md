# Installing TrueNAS Scale

Followed the install guide on the [site](https://www.truenas.com/docs/scale/gettingstarted/install/installingscale/)  
[expanded instructions](https://www.truenas.com/docs/scale/gettingstarted/install/installingscale/#expand-6)  
click the arrow  
![](./assets/2025-02-15-11-41-27.png)

- created a drive from the downloade ISO
- set the server to boot from the usb
    - there was an issue that caused it not to see the usb after setting it in bios
- Launched a virtual console from iDRAC and setup Virtual Media to pull the ISO from my pc
- When the install was completed I shut the system down, removed the virtual media, and booted into the OS. 
- After it has booted fully the virtual console will display the URL for the remaining configuration
- I logged into the virtual console and checked the status of ssh
    - it was disabled and stopped
    - `systemctl status ssh`
    - `systemctl enable ssh`
    - `systemctl start ssh`
- 