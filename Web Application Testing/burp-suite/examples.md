# Burp Suite Examples

## Example 1: Capture Login Request

Steps:

1. Open Burp Browser
2. Enable Intercept
3. Visit login page
4. Submit credentials

Captured Request:

```http
POST /login HTTP/1.1

username=test
password=test123
```

Observe:

- Method
- Parameters
- Headers
- Cookies

---

## Example 2: Explore Application

Browse through the site.

Open:

```text
Target → Site Map
```

Result:

```text
/
├── login
├── register
├── dashboard
└── profile
```

---

## Example 3: Review Cookies

Navigate:

```text
Proxy → HTTP History
```

Example:

```http
Cookie: session=abc123xyz
```

Questions:

- Is a session cookie present?
- Does it change after login?

---

## Example 4: Use Repeater

Right-click request.

```text
Send to Repeater
```

Modify values and resend.

Purpose:

- Understand application behavior
- Test parameters manually

---

## Example 5: Analyze Response Codes

Common responses:

```text
200 OK
302 Redirect
403 Forbidden
404 Not Found
500 Internal Server Error
```

Understanding responses is a critical web testing skill.
