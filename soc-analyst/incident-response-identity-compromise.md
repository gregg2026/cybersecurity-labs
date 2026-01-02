\# Incident Response Tabletop – Identity Compromise Scenario



\## Incident Type

Identity-based account compromise involving a privileged user.



\## Objective

Simulate a SOC-led incident response to a suspected identity compromise, focusing on detection, containment, eradication, and recovery actions.



\## Scenario Overview

Security monitoring identified suspicious authentication activity involving a user account with elevated privileges.  

The activity included multiple failed sign-in attempts followed by a successful login and subsequent administrative actions.



The incident raises concern for potential credential compromise or account abuse.



\## Initial Indicators of Compromise (IOCs)

\- Repeated failed authentication attempts

\- Successful login from an unusual context

\- Privileged role activation via PIM

\- Administrative actions outside normal usage patterns



\## Detection \& Identification

\*\*Data Sources Reviewed:\*\*

\- Windows Security Event Logs

\- Entra ID sign-in logs

\- Privileged Identity Management audit logs



\*\*Assessment:\*\*

\- Authentication behavior deviates from baseline

\- Privileged access increases potential impact

\- Incident classified as a suspected identity compromise



Severity: \*\*High\*\*



---



\## Containment Actions

Immediate actions taken to limit impact:

1\. Disabled affected user account

2\. Revoked active sessions and refresh tokens

3\. Deactivated elevated role assignments

4\. Reviewed recent privileged actions for impact

5\. Increased monitoring on related accounts



---



\## Eradication

Steps taken to remove threat persistence:

\- Forced password reset for affected account

\- Reviewed MFA registration and authentication methods

\- Removed unnecessary role eligibility

\- Audited Conditional Access policy exclusions

\- Verified no additional persistence mechanisms were introduced



---



\## Recovery

Actions taken to restore secure operations:

\- Re-enabled account with least-privilege access

\- Required MFA re-registration

\- Limited PIM activation duration and scope

\- Monitored authentication activity post-restoration

\- Validated normal user behavior resumed



---



\## Post-Incident Review

\*\*Root Cause Analysis:\*\*

\- Weak authentication controls or credential exposure

\- Insufficient monitoring of privileged activity



\*\*Lessons Learned:\*\*

\- Identity is a primary attack surface

\- Privileged access must be tightly controlled and monitored

\- Early detection reduces blast radius significantly



---



\## Preventive Recommendations

\- Enforce MFA for all users, especially privileged roles

\- Use Privileged Identity Management for all administrative access

\- Block legacy authentication protocols

\- Regularly review sign-in and PIM audit logs

\- Conduct periodic identity-focused incident response exercises



---



\## SOC Relevance

This tabletop reflects a realistic SOC response to identity compromise incidents and demonstrates the importance of coordinated detection, containment, and recovery efforts in cloud-centric environments.



