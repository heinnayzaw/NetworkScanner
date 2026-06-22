# Python Network Scanner

A simple Python ARP scanner that discovers devices connected to a local network.

## Features

* Scans an IP address or IP range
* Displays connected devices
* Shows IP and MAC addresses
* Uses Scapy to send ARP requests

## Requirements

* Python 3
* Scapy
* Root privileges

Install Scapy:

```bash
pip install scapy
```

## Usage

```bash
sudo python3 network_scanner.py -t 192.168.1.0/24
```

## Arguments

* `-t`, `--target` — Target IP address or network range

## Example Output

```text
IP                      MAC Address
--------------------------------------
192.168.1.1             aa:bb:cc:dd:ee:ff
192.168.1.5             11:22:33:44:55:66
```

## Disclaimer

For educational purposes only. Use this tool only on networks you own or have permission to test.
