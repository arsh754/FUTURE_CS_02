# Incident Response Report – Task 2

## Incident Summary
During routine security monitoring, multiple failed login attempts were detected in the authentication logs. These attempts targeted privileged user accounts, indicating a potential brute-force attack.

## Detection
The incident was detected by reviewing authentication logs (`auth.log`) and identifying repeated failed login attempts from the same IP addresses within short time intervals.

## Affected Systems
- Authentication service
- User accounts: admin, root

## Indicators of Compromise (IOCs)
| Type | Value |
|-----|------|
| IP Address | 192.168.1.10 |
| IP Address | 203.0.113.45 |
| Targeted Accounts | admin, root |

## Impact Assessment
- No successful unauthorized access was detected.
- Risk of credential compromise if attacks continued.
- Increased load on authentication services.

## Response Actions Taken
- Identified and documented suspicious IP addresses.
- Recommended blocking malicious IPs using firewall rules.
- Suggested enabling account lockout policies.

## Recommendations
- Implement rate limiting on login attempts.
- Enable multi-factor authentication (MFA).
- Monitor logs continuously using a SIEM tool.
- Conduct regular security audits.

## Conclusion
The incident was identified at an early stage and no systems were compromised. Proper security controls and monitoring can prevent similar attacks in the future.
