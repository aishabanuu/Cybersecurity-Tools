# Gobuster Notes

## Key Concepts

### Content Discovery

Finding files and directories that are not linked from the website.

Examples:

```text
/admin
/uploads
/backup
/dev
```

---

### Wordlists

Gobuster relies on wordlists.

Common entries:

```text
admin
backup
config
test
uploads
```

Each word is tested against the target.

---

### Status Codes

Understanding responses is important.

| Code | Meaning |
|--------|---------|
| 200 | Resource Exists |
| 301 | Redirect |
| 302 | Temporary Redirect |
| 403 | Forbidden |
| 404 | Not Found |

---

### File Extensions

Applications often expose files such as:

```text
.php
.asp
.aspx
.html
.txt
```

Example:

```bash
-x php,txt,html
```

---

## Common Wordlists

### DIRB Common

```text
/usr/share/wordlists/dirb/common.txt
```

---

### SecLists

```text
/usr/share/seclists/
```

Popular source for enumeration wordlists.

---

## Typical Workflow

```text
Choose Target
      ↓
Select Wordlist
      ↓
Run Enumeration
      ↓
Review Results
      ↓
Verify Findings
      ↓
Document Findings
```

---

## Important Findings

Resources such as:

```text
/admin
/backup
/uploads
```

may indicate:

- Administrative interfaces
- Development environments
- Backup locations
- File storage locations

Always verify findings manually.

---

## Common Mistakes

- Using the wrong wordlist
- Ignoring redirects
- Forgetting file extensions
- Not saving results
- Assuming every result is important

---

## Personal Notes

- Start with small wordlists.
- Understand response codes.
- Verify findings in a browser.
- Keep records of discovered content.
- Use content discovery to improve application mapping.
