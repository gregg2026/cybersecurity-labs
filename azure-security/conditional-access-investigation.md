\# Conditional Access Review – Risk-Based Authentication Controls



\## Objective

Review and evaluate Conditional Access policies to reduce identity-based attack risk and enforce secure authentication practices.



\## Environment

\- Microsoft Entra ID (Azure AD) lab tenant

\- Conditional Access policy configuration

\- Test user accounts



\## Scenario Overview

Identity-based attacks such as credential theft and MFA bypass attempts are common attack vectors.  

This lab reviews Conditional Access configurations to ensure authentication controls align with Zero Trust principles.



\## Policies Reviewed

\- Require MFA for all users

\- Require MFA for privileged roles

\- Block legacy authentication protocols

\- Enforce compliant or hybrid-joined devices (where applicable)



\## Review Process

1\. Reviewed existing Conditional Access policies

2\. Identified gaps in MFA enforcement

3\. Assessed privileged role coverage

4\. Evaluated exclusions and legacy authentication exposure

5\. Tested policy behavior using test accounts



\## Findings

\- MFA was not consistently enforced across all users

\- Privileged roles required stronger conditional controls

\- Legacy authentication presented unnecessary risk

\- Policy exclusions required tightening



\## Risk Assessment

Misconfigured or incomplete Conditional Access policies increase the likelihood of:

\- Credential-based compromise

\- MFA fatigue or bypass attacks

\- Privileged account abuse



Risk Level: \*\*High\*\* without proper enforcement



\## Recommended Improvements

\- Enforce MFA for all users, with stronger controls for admins

\- Block legacy authentication protocols

\- Limit Conditional Access exclusions

\- Monitor sign-in logs for risky authentication patterns

\- Periodically review and test policy effectiveness



\## Lessons Learned

Conditional Access is a foundational identity security control.  

Effective policies must balance usability with risk reduction and require ongoing review.



\## SOC \& Cloud Security Relevance

Identity is the primary security perimeter in modern environments.  

Understanding Conditional Access enables both SOC investigation and proactive cloud security hardening.



