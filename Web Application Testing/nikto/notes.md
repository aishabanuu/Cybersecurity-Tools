# Nikto Notes

## Key Concepts

### Web Server Enumeration

The process of gathering information about a web server.

Examples:

- Server software
- Version information
- Configuration details
- Exposed resources

---

### Security Headers

HTTP headers that improve security.

Common Examples:

| Header | Purpose |
|----------|----------|
| X-Frame-Options | Clickjacking protection |
| Content-Security-Policy | Restrict resource loading |
| X-Content-Type-Options | MIME protection |
| Strict-Transport-Security | HTTPS enforcement |

Nikto may identify missing security headers.

---

### Directory Indexing

Occurs when a web server displays directory contents.

Example:

```text
/uploads/
```

Potential Risk:

- Information disclosure

---

### Default Files

Some applications leave administrative or example files exposed.

Examples:

```text
/test/
/admin/
/backup/
```

These may reveal useful information.

---

### Outdated Software

Older software versions may contain known vulnerabilities.

Examples:

```text
Apache
Nginx
PHP
Tomcat
```

Nikto can help identify version information.

---

## Understanding Findings

Nikto findings generally fall into:

### Informational

Interesting observations requiring review.

### Configuration Issues

Server settings that may need improvement.

### Potential Risks

Items requiring additional investigation.

---

## Typical Workflow

```text
Identify Server
        ↓
Run Nikto
        ↓
Review Findings
        ↓
Validate Findings
        ↓
Document Results
```

---

## Common Mistakes

- Treating every finding as a vulnerability
- Ignoring false positives
- Failing to verify results manually
- Not documenting findings

---

## Relationship to Other Tools

| Tool | Purpose |
|--------|---------|
| Burp Suite | Analyze HTTP traffic |
| Gobuster | Content discovery |
| Nikto | Server assessment |
| SQLMap | Input testing |
| Nmap | Service enumeration |

---

## Personal Notes

- Nikto is excellent for initial web server reconnaissance.
- Always verify findings manually.
- Document server software and versions.
- Review missing security headers.
- Focus on understanding findings rather than collecting them.
