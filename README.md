# web-security-labs
A collection of my web security learning journey, PortSwigger lab practice, server-side vulnerability notes, payloads, Burp Suite testing, and cybersecurity writeups.

# Server-Side Vulnerabilities

Hii, this repository contains my learning journey, notes, lab practice, payloads, and writeups related to Server-Side Vulnerabilities.
<br><br>

Author - Lucky Naruka
<br><br>

## About
In this repository, I document my practical learning from PortSwigger Web Security Academy and other cybersecurity platforms.
<br><br>

I share:
- Notes
- Lab writeups
- Payloads used
- Request/Response analysis
- What I learned from each vulnerability
<br><br>

## Topics Covered
- NoSQL Injection
- SQL Injection
- Authentication Vulnerabilities
- Access Control Vulnerabilities
- File Path Traversal
- Command Injection
- Server-Side Request Forgery (SSRF)
<br><br>

## Tools Used
- Burp Suite
- Kali Linux
- Browser Developer Tools
<br><br>

## Platform
- PortSwigger Web Security Academy
<br><br>

## What I Learned
- How client requests interact with servers
- How vulnerable inputs can affect backend databases
- How authentication and access control work
- How to analyze HTTP requests and responses
- How to test web applications safely in lab environments
- How attackers exploit insecure server-side logic
<br><br>

## Example Payloads

### NoSQL Injection Payloads
```json
{"username":{"$ne":null},"password":{"$ne":null}}
<br><br>
### SQL Injection Payloads
' OR '1'='1
<br>
admin' --
<br>
