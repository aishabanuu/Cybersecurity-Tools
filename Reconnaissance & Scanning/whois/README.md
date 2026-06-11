# Whois

## Overview

Whois is a protocol and command-line tool used to query domain registration information and IP address ownership records.

It helps security professionals, system administrators, and researchers identify:

- Domain ownership information
- Registrar details
- Registration and expiration dates
- Nameservers
- Network ownership information
- Contact information (when publicly available)

## Why Use Whois?

During reconnaissance, Whois can provide valuable information about:

- Target organizations
- Domain infrastructure
- Registration history
- DNS configuration
- Hosting providers

## Installation

Most Linux distributions include Whois.

Verify installation:

```bash
whois --version
```

Install on Debian/Kali:

```bash
sudo apt update
sudo apt install whois
```

## Common Use Cases

- Domain investigation
- Asset discovery
- OSINT collection
- Incident response
- Threat intelligence

## Notes

Modern privacy regulations and domain privacy services may hide some ownership details.
