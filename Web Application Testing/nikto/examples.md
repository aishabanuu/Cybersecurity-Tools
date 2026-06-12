# Nikto Examples

## Example 1: Basic Scan

Command:

```bash
nikto -h http://localhost
```

Possible Output:

```text
Server: Apache
Directory indexing found
Missing security headers
```

Purpose:

- Identify server information
- Discover common weaknesses

---

## Example 2: HTTPS Assessment

Command:

```bash
nikto -h https://localhost
```

Possible Findings:

```text
SSL configuration issues
Outdated software
```

Purpose:

- Review HTTPS configuration
- Identify potential security concerns

---

## Example 3: Save Report

Command:

```bash
nikto -h http://localhost -output report.txt
```

Output File:

```text
report.txt
```

Useful for documentation and reporting.

---

## Example 4: Scan Alternate Port

Command:

```bash
nikto -h 192.168.1.10 -p 8080
```

Purpose:

- Assess applications running on non-standard ports

---

## Example 5: Review Security Headers

Potential Finding:

```text
X-Frame-Options Header Missing
```

Possible Impact:

- Increased risk of clickjacking

Purpose:

- Understand server hardening opportunities
