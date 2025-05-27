# 1.Base64 Auth Key via Terminal

Use this command to create a base64-encoded string for HTTP Basic Authentication. This is commonly used when interacting with APIs that require credentials passed in an `Authorization` header.

---

### Basic Syntax

```bash
echo -n "bc0a2c2d2acb0f9:20ebfe67fbf273b" | base64
```
#### Example: 
```bash
echo -n "bc0a2c2d2acb0f9:20ebfe67fbf273b" | base64
```
#### Output:
```bash
YmMwYTJjMmQyYWNiMGY5OjIwZWJmZTY3ZmJmMjczYg==
```

---

### Common Use Cases
 When calling an API endpoint that requires Basic Authentication:

```bash
curl -H "Authorization: Basic YmMwYTJjMmQyYWNiMGY5OjIwZWJmZTY3ZmJmMjczYg==" https://api.example.com/data

```