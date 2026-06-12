# Nikto Commands

## Basic Scan

```bash
nikto -h http://localhost
```

---

## Scan HTTPS Target

```bash
nikto -h https://localhost
```

---

## Scan by IP Address

```bash
nikto -h 192.168.1.10
```

---

## Specify Port

```bash
nikto -h 192.168.1.10 -p 8080
```

---

## Save Results

```bash
nikto -h http://localhost -output report.txt
```

---

## Save HTML Report

```bash
nikto -h http://localhost -Format htm -output report.html
```

---

## Display Help

```bash
nikto -Help
```

---

## Scan Multiple Ports

```bash
nikto -h 192.168.1.10 -p 80,443,8080
```

---

## Check Specific URL

```bash
nikto -h http://localhost/admin
```

---

## Display Version

```bash
nikto -Version
```
