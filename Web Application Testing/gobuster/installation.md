# Gobuster Installation

## Verify Installation

Check version:

```bash
gobuster version
```

---

## Install on Kali

```bash
sudo apt update
sudo apt install gobuster
```

---

## Verify Wordlists

Most wordlists are located in:

```bash
ls /usr/share/wordlists/
```

Common locations:

```text
/usr/share/wordlists/dirb/
/usr/share/wordlists/seclists/
```

---

## Popular Wordlists

### DIRB Common

```text
/usr/share/wordlists/dirb/common.txt
```

Good for beginners.

---

### SecLists

```text
/usr/share/seclists/
```

Contains:

- Directory wordlists
- File wordlists
- DNS wordlists
- Username lists

---

## Update Wordlists

```bash
sudo apt update
sudo apt install seclists
```

Verify:

```bash
ls /usr/share/seclists/
```
