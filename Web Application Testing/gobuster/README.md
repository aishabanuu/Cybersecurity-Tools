# Gobuster

## Overview

Gobuster is a fast command-line tool used for content discovery and enumeration.

It is commonly used to discover:

- Hidden directories
- Hidden files
- Virtual hosts (vhosts)
- DNS subdomains

Gobuster works by testing words from a wordlist against a target and checking which resources exist.

## Why Use Gobuster?

Many web applications contain pages or directories that are not linked from the main website.

Examples:

```text
/admin
/backup
/uploads
/dev
/config
```

Gobuster helps identify these resources.

## Common Modes

### Directory Enumeration

Discover hidden directories and files.

### DNS Enumeration

Discover subdomains.

### Virtual Host Enumeration

Identify hidden virtual hosts.

## Benefits

- Fast
- Lightweight
- Easy to use
- Supports multiple enumeration modes

## Typical Workflow

```text
Identify Target
      ↓
Choose Wordlist
      ↓
Run Gobuster
      ↓
Review Results
      ↓
Verify Findings
```

## Learning Objectives

- Understand content discovery
- Learn wordlists
- Identify hidden resources
- Document discovered content
