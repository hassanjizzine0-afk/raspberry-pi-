
### Show Wi-Fi interface details and connection status
```bash
iwconfig
```

### Test internet connection by sending 4 packets to Google DNS
```bash
ping -c 4 8.8.8.8
```

### Find devices on local network with IP starting with 10.42
```bash
ip neigh | grep "10.42"
```

### Open Raspberry Pi configuration menu
```bash
sudo raspi-config
```

### Disconnect Wi-Fi on wlan0 interface
```bash
sudo nmcli dev disconnect wlan0
```

### Connect to a specific saved Wi-Fi network by name
```bash
sudo nmcli connection up "NAME"
```

### List all saved network connections
```bash
nmcli connection show
```

### Show network connections with priority settings
```bash
nmcli -f NAME,AUTOCONNECT-PRIORITY connection show
```

### Set high priority for a preferred Wi-Fi network
```bash
sudo nmcli connection modify "YOUR_NETWORK_NAME" connection.autoconnect-priority 20
```

### Lower priority for another network
```bash
sudo nmcli connection modify "OTHER_NETWORK_NAME" connection.autoconnect-priority 5
```
```
