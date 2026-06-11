# Whois Notes

## What Information Does Whois Provide?

A Whois record may contain:

- Domain Name
- Registrar
- Creation Date
- Expiration Date
- Updated Date
- Nameservers
- Registrant Information
- Administrative Contacts
- Technical Contacts

---

## Key Terms

### Registrar

The company through which the domain was registered.

Examples:

- GoDaddy
- Namecheap
- Cloudflare Registrar

---

### Registrant

The individual or organization that owns the domain.

Note:

Privacy services often hide registrant details.

---

### Nameserver

A server responsible for answering DNS queries.

Example:

```text
ns1.example.com
ns2.example.com
```

---

### Creation Date

The date the domain was originally registered.

Example:

```text
Creation Date: 2020-01-15
```

Useful for:

- Domain age assessment
- Threat intelligence investigations

---

### Expiration Date

Indicates when a domain registration expires.

Example:

```text
Registry Expiry Date: 2028-01-15
```

---

## Whois for IP Addresses

Whois can also identify:

- Network owners
- Hosting providers
- Autonomous Systems (ASNs)

Example:

```bash
whois 1.1.1.1
```

---

## Common Reconnaissance Questions

### Who owns this domain?

Use:

```bash
whois domain.com
```

---

### Which company hosts this IP?

Use:

```bash
whois x.x.x.x
```

---

### Which nameservers are used?

Use:

```bash
whois domain.com | grep "Name Server"
```

---

### When was the domain registered?

Use:

```bash
whois domain.com | grep Creation
```

---

## Limitations

- Privacy protection may hide ownership information.
- Some registries return limited data.
- Results vary by country and TLD.
- Whois does not provide subdomains.

---

## Relationship to Other Tools

| Tool | Purpose |
|--------|---------|
| Whois | Registration information |
| Dig | DNS records |
| Nmap | Host and service discovery |
| theHarvester | OSINT collection |
| Netdiscover | Local network discovery |

---

## Personal Notes

- Whois is usually one of the first passive reconnaissance steps.
- Record registrar and nameserver information.
- Investigate unusual registration patterns.
- Compare Whois results with DNS records from Dig.
- Document all findings for later analysis.
