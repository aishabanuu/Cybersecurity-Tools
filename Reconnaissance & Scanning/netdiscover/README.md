# Netdiscover

## Overview

Netdiscover is an active/passive network reconnaissance tool that uses ARP requests to discover live hosts on a local network.

It is particularly useful when:

- You do not know the network layout.
- DHCP is assigning IP addresses dynamically.
- You want to identify devices on the same LAN.
- Traditional ping sweeps are blocked.

## Features

- ARP-based host discovery
- Passive network monitoring
- Active network scanning
- MAC address identification
- Vendor detection through OUI lookup

## Installation

Netdiscover is typically pre-installed on Kali Linux.

Verify installation:

```bash
netdiscover -h
```

Install manually:

```bash
sudo apt update
sudo apt install netdiscover
```

## Typical Workflow

1. Identify your network interface.
2. Determine your subnet.
3. Discover live hosts.
4. Record IP and MAC addresses.
5. Perform further enumeration using tools such as Nmap.

## Advantages

- Fast host discovery
- Effective on local networks
- Works even when ICMP responses are blocked
- Simple and lightweight

## Limitations

- Works only on local Layer 2 networks.
- Cannot scan across the Internet.
- Requires access to the target network segment.
