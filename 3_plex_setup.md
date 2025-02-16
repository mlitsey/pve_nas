# Setting up the Plex Container

## Grant access to outside of network
- App settings in Truenas Scale
    - Enable Host Network.

- Plex settings
    - Disable IPv6 support in Plex settings.
- Select my preferred network interface (the actual network interface, not a kubernetes one).
- Set Custom server access URLs to the http & https versions of the server's IP on port 32400.
- Manually specify public port.
- Router settings
    - Forward 32400 traffic to my server's IP.

