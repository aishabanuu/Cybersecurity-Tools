# Nikto

## Overview

Nikto is an open-source web server assessment tool that checks for common web server misconfigurations, outdated software versions, exposed files, and other security-related issues.

Nikto is often used during the reconnaissance and enumeration phases of a web application assessment to quickly identify areas that may require further investigation.

## What Nikto Can Identify

- Default files and directories
- Outdated web server software
- Insecure server configurations
- Directory indexing
- Dangerous HTTP methods
- Missing security headers
- Common administrative interfaces

## Why Use Nikto?

Nikto helps testers quickly gather information about a web server and identify common issues that may affect security.

## Typical Workflow

```text
Identify Web Server
        ↓
Run Nikto Scan
        ↓
Review Findings
        ↓
Validate Results
        ↓
Document Findings
```

## Advantages

- Easy to use
- Fast initial assessment
- Extensive signature database
- Useful for web server reconnaissance

## Limitations

- Produces many informational findings
- Can generate false positives
- Does not replace manual testing
- Not designed for exploitation

## Learning Objectives

- Understand web server enumeration
- Learn common web misconfigurations
- Practice interpreting scan results
- Document findings effectively
