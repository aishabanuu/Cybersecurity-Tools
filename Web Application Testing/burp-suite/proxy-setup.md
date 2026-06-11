# Proxy Setup

## What is a Proxy?

A proxy sits between your browser and the target application.

```text
Browser
   ↓
Burp Suite
   ↓
Website
```

Burp can:

- View requests
- View responses
- Modify traffic
- Record browsing activity

---

## Using Burp Browser

Recommended for beginners:

```text
Proxy
→ Intercept
→ Open Browser
```

No additional configuration required.

---

## Manual Browser Configuration

Proxy Settings:

```text
Host: 127.0.0.1
Port: 8080
```

---

## Enable Interception

Navigate to:

```text
Proxy → Intercept
```

Click:

```text
Intercept is ON
```

---

## Disable Interception

Click:

```text
Intercept is OFF
```

This allows requests to pass normally.

---

## HTTP History

Navigate to:

```text
Proxy → HTTP History
```

Useful information:

- URLs
- Methods
- Parameters
- Cookies
- Status codes
- Response sizes

---

## Site Map

Navigate to:

```text
Target → Site Map
```

Purpose:

- Discover pages
- Understand application structure
- Organize testing activities
