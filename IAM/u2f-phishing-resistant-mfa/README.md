🔐 Phishing-Resistant MFA Lab (U2F / WebAuthn)

🚀 Executive Summary



This lab demonstrates phishing-resistant multi-factor authentication (MFA) using U2F/WebAuthn by emulating a hardware security key with a Flipper Zero (Momentum firmware).



The focus is identity security decision-making, not device novelty: understanding why U2F stops MFA phishing, how it integrates with modern IAM platforms, and where it should and should not be used in enterprise environments.



🎯 Why This Matters (Recruiter View)



MFA bypass via phishing is a top attack vector



U2F/WebAuthn is a recommended control in Zero Trust architectures



Demonstrates IAM fluency, not just tool usage



Shows security judgment and compliance awareness



🧠 Key Skills Demonstrated



Identity \& Access Management (IAM)



Phishing-resistant authentication



WebAuthn / U2F protocols



Risk-based security decisions



Secure lab documentation



Policy-aware implementation



🧰 Tools \& Environment



Flipper Zero (Momentum firmware)



Windows 11



Chromium-based browser (Chrome / Edge)



U2F / WebAuthn-enabled identity provider



⚠️ Security \& Compliance Context



This lab is educational and non-production.



Flipper Zero lacks a certified secure element



Credentials are software-stored



Not suitable for CJIS, FISMA, or regulated production use



Enterprise recommendation: Certified hardware keys (e.g., YubiKey)



This distinction is intentional and documented.



🛠️ Implementation Summary

Enable U2F Mode

Flipper → Main Menu → USB → U2F



Register Security Key



Plug in Flipper via USB



Add as security key in supported service



Confirm user presence via button press



Authenticate



User presence required



No OTP, no shared secrets



Domain-bound authentication



🔍 Security Analysis (What I Evaluated)

Why U2F Beats OTP

Threat	OTP MFA	U2F

Phishing	❌	✅

Replay Attacks	❌	✅

Man-in-the-Middle	❌	✅

Shared Secrets	Yes	No

Risk Considerations



Device trust vs compliance requirements



Secure element importance



Physical access threat model



🧠 Lessons Learned



Phishing-resistant MFA eliminates entire attack classes



Hardware backing matters for compliance



Security controls must align with policy, not just capability



Labs should mirror real enterprise decision points



🏢 Enterprise Relevance



This lab directly supports:



Zero Trust identity strategy



MFA policy evaluation



IAM platform testing (Entra ID, Google Workspace, etc.)



Security awareness demonstrations for leadership



📈 Future Enhancements



Microsoft Entra ID enforcement testing



Flipper vs YubiKey security comparison



Phishing simulation failure analysis



WebAuthn challenge inspection



📸 Evidence



(Screenshots intentionally excluded to avoid sensitive data exposure)



👤 Author



Greggory Petty

Cybersecurity \& Identity Access Management

Lab-only environment

