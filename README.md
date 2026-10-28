\# Advanced VAPT — OWASP Juice Shop



\## Overview

This project documents an Advanced Vulnerability Assessment and Penetration Testing (VAPT) lab using OWASP Juice Shop and Burp Suite.



\## Objectives

\- Perform attack surface mapping.

\- Test for Basket IDOR/BOLA.

\- Investigate verbose error disclosure.

\- Validate whether findings form an attack chain.

\- Document security impact and remediation.



\## Tools Used

\- OWASP Juice Shop

\- Burp Suite

\- Browser Developer Tools



\## Findings

1\. \*\*Basket IDOR/BOLA:\*\* Cross-account basket access was observed in the local test environment.

2\. \*\*Verbose Error Disclosure:\*\* An HTTP 500 response exposed internal server paths and a stack trace.



The two findings were assessed independently. A combined attack chain was not demonstrated.



\## Remediation

\- Enforce server-side ownership checks for basket operations.

\- Return generic error messages to clients.

\- Store detailed diagnostic information in protected server logs.



\## Disclaimer

All testing was performed in a local, authorized lab environment for educational purposes.

