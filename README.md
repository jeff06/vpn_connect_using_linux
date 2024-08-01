This command connect to a VPN using openvpn.
```
#!/bin/bash

sudo openvpn --config <VPN_FILE_LOCATION>.ovpn --data-ciphers AES-256-CBC --script-security 2 --up update-systemd-resolved --up-restart --down update-systemd-resolved --down-pre
```
