# Netdiscover Notes

## What is ARP?

ARP (Address Resolution Protocol) maps IP addresses to MAC addresses on a local network.

Example:

```text
IP Address  →  MAC Address
192.168.1.1 → AA:BB:CC:DD:EE:FF
```

Netdiscover relies heavily on ARP to identify active hosts.

---

## Active vs Passive Discovery

### Active Discovery

Sends ARP requests to identify hosts.

Example:

```bash
sudo netdiscover -r 192.168.1.0/24
```

Advantages:

- Fast
- Comprehensive
- Finds most hosts

Disadvantages:

- Generates network traffic
- More detectable

---

### Passive Discovery

Listens for ARP traffic already present on the network.

Example:

```bash
sudo netdiscover -p
```

Advantages:

- Stealthier
- No additional traffic generated

Disadvantages:

- Slower
- May miss inactive devices

---

## Understanding Output

Typical output contains:

| Field | Description |
|---------|-------------|
| IP Address | Device IP |
| MAC Address | Hardware address |
| Vendor | Manufacturer based on MAC prefix |
| Count | Number of ARP responses |
| Length | Packet length |

---

## Common Vendors

| Vendor | Device Type |
|----------|------------|
| Cisco | Routers, Switches |
| Dell | Workstations, Servers |
| HP | Computers, Printers |
| Apple | Macs, iPhones |
| Samsung | Mobile Devices |
| Intel | Network Interfaces |

---

## Reconnaissance Workflow

```text
Identify Interface
        ↓
Determine Network Range
        ↓
Run Netdiscover
        ↓
Identify Live Hosts
        ↓
Record IP/MAC Addresses
        ↓
Use Nmap for Service Enumeration
```

---

## Personal Notes

- Always verify the correct network interface before scanning.
- Document discovered hosts.
- Compare Netdiscover results with Nmap host discovery.
- Use passive mode when learning network behavior.
- Record vendor information for asset identification.
- Save findings for later enumeration phases.

---

## Useful Commands

Check interfaces:

```bash
ip a
```

Check routing table:

```bash
ip route
```

Start discovery:

```bash
sudo netdiscover
```

Scan specific range:

```bash
sudo netdiscover -r 192.168.1.0/24
```
