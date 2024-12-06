# WAF-Bypass-Headers
A comprehensive list of HTTP headers used for testing WAF bypass techniques. Includes localhost, private, and public IP examples for penetration testing and security assessments.

---

### README: `waf-bypass-headers`

#### Overview  
This file contains HTTP headers to simulate various client behaviors for testing WAFs or server configurations.

#### Usage  
- Copy headers into tools like Burp Suite or custom scripts.  
- Modify IPs or values as needed for testing.  

#### Example Script  

```python
import requests

url = "http://target-website.com"
headers = {
    "X-Forwarded-For": "127.0.0.1",
    "Client-IP": "10.0.0.1",
    "Origin": "http://127.0.0.1",
    "Referer": "http://localhost/"
}

response = requests.get(url, headers=headers)
print(response.status_code)
```

#### Disclaimer  
Use responsibly and only for authorized testing.
