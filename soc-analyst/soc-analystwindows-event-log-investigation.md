\# Windows Event Log Investigation – Suspicious Authentication Activity



\## Objective

Analyze Windows Security Event Logs to identify and assess suspicious authentication behavior that may indicate brute-force activity, credential misuse, or misconfigured accounts.



\## Environment

\- Windows 10 / 11 virtual machine

\- Local Event Viewer

\- Security logging enabled



\## Data Sources

\- Windows Security Event Log

\- Local system timestamps and user context



\## Key Event IDs Analyzed

\- \*\*4624\*\* – Successful logon

\- \*\*4625\*\* – Failed logon attempt

\- \*\*4672\*\* – Special privileges assigned to new logon

\- \*\*4800 / 4801\*\* – Workstation lock/unlock events



\## Investigation Steps

1\. Filtered Security logs for Event ID 4625 to identify repeated failed logon attempts

2\. Correlated failed logons with subsequent successful logons (Event ID 4624)

3\. Reviewed Event ID 4672 to determine whether successful logons included elevated privileges

4\. Analyzed timestamps to determine frequency and pattern consistency

5\. Validated activity against expected user behavior



\## Findings

\- Multiple failed authentication attempts observed within a short time window

\- A successful logon occurred shortly after repeated failures

\- Successful logon included assignment of elevated privileges

\- Pattern increases likelihood of credential-based attack or weak password controls



\## Risk Assessment

This activity pattern could indicate:

\- Brute-force or password spraying attempts

\- Compromised credentials

\- Inadequate account lockout policies

\- Over-privileged user accounts



Risk Level: \*\*Medium to High\*\*, depending on account sensitivity and recurrence



\## MITRE ATT\&CK Mapping

\- \*\*T1110\*\* – Brute Force

\- \*\*T1078\*\* – Valid Accounts



\## Recommended Mitigations

\- Enforce account lockout thresholds

\- Review privileged group membership

\- Implement or strengthen MFA for privileged accounts

\- Monitor recurring authentication failures

\- Audit service and administrative accounts for misuse



\## Lessons Learned

Correlating failed and successful authentication events is critical for identifying credential-based attacks.  

Privileged logons following failed attempts should always be treated as higher-risk events in a SOC environment.



\## SOC Relevance

This investigation reflects common Tier 1 / Tier 2 SOC workflows involving authentication anomalies and highlights the importance of contextual log analysis over single-event alerting.



