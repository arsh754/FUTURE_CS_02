# Log Analysis – Task 2

## Overview
Authentication logs were analyzed to detect suspicious login activity.

## Findings
- Multiple failed login attempts were detected from IP address 192.168.1.10 targeting the user "admin".
- Multiple failed login attempts were also detected from IP address 203.0.113.45 targeting the user "root".
- These patterns indicate a possible brute-force attack.

## Normal Activity
- A successful login was observed for user "arsh" from IP address 192.168.1.5.

## Conclusion
The logs show evidence of unauthorized login attempts that should trigger a security alert and further investigation.
