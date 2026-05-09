

### iwconfig
```bash
# Show Wi-Fi interface details and connection status
iwconfig
```

### ping -c 4 8.8.8.8
```bash
# Test internet connection by sending 4 packets to Google DNS
ping -c 4 8.8.8.8
```

### ip neigh | grep "10.42"
```bash
# Find devices on local network with IP starting with 10.42
ip neigh | grep "10.42"
```

### sudo raspi-config
```bash
# Open Raspberry Pi configuration menu
sudo raspi-config
```

### sudo nmcli dev disconnect wlan0
```bash
# Disconnect Wi-Fi on wlan0 interface
sudo nmcli dev disconnect wlan0
```

### sudo nmcli connection up "NAME"
```bash
# Connect to a specific saved Wi-Fi network by name
sudo nmcli connection up "NAME"
```

### nmcli connection show
```bash
# List all saved network connections
nmcli connection show
```
```
