# Netdiscover Commands

## Display Help

```bash
netdiscover -h
```

## Start Automatic Discovery

```bash
sudo netdiscover
```

## Specify Interface

```bash
sudo netdiscover -i eth0
```

Example:

```bash
sudo netdiscover -i wlan0
```

## Scan Specific Range

```bash
sudo netdiscover -r 192.168.1.0/24
```

## Scan Smaller Range

```bash
sudo netdiscover -r 192.168.1.1-100
```

## Passive Mode

```bash
sudo netdiscover -p
```

Passive mode listens for ARP traffic without actively sending requests.

## Specify Scan Delay

```bash
sudo netdiscover -s 10
```

## Ignore Home Network Detection

```bash
sudo netdiscover -f
```

## Scan with Interface and Range

```bash
sudo netdiscover -i wlan0 -r 192.168.1.0/24
```

## View Network Interfaces

```bash
ip a
```

or

```bash
ifconfig
```
