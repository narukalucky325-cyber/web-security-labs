# NoSQL Injection Notes
# NoSQL Injection Notes
<br><br>

## What is NoSQL Injection?
<br>

NoSQL Injection is a web security vulnerability where an attacker manipulates database queries in NoSQL databases such as MongoDB.
<br><br>

It happens when user input is not properly validated or sanitized before being used in backend database queries.
<br><br>

## Common Causes
<br>
- Improper input validation
<br>
- Unsafe database queries
<br>
- Directly using user input in backend queries
<br>
- Weak authentication handling
<br><br>

## MongoDB Operators Used in Attacks
<br>
### $ne
Means "not equal".
<br>
Example:
<br>
```json
{"username":{"$ne":null},"password":{"$ne":null}}
<br>
$regex

Used for pattern matching.
<br>

Example:
<br>

{"username":{"$regex":"admin.*"},"password":{"$ne":null}}
<br>
Authentication Bypass
<br>

Attackers can bypass login forms by modifying JSON values and abusing MongoDB operators.
<br><br>

Example:
<br>

{"username":{"$ne":null},"password":{"$ne":null}}
<br>

This payload may return the first valid user from the database.
<br><br>

Tools Used
<br>
Burp Suite <br>
Firefox Developer Tools <br>
Kali Linux
<br><br>
What I Learned
<br>
How NoSQL Injection vulnerabilities work <br>
How MongoDB queries process user input <br>
How authentication bypass attacks happen <br>
How HTTP requests and responses can be modified <br>
How Burp Suite helps analyze web traffic <br>
How insecure backend logic creates vulnerabilities <br>
How to safely practice web security in lab environments
<br><br>
Practical Skills Gained
<br>
Intercepting requests using Burp Suite <br>
Modifying JSON request bodies <br>
Testing authentication systems <br>
Understanding MongoDB operators <br>
Identifying insecure server-side behavior
<br><br>

```json
{"username":{"$ne":null},"password":{"$ne":null}}
