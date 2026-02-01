\# Secure Reverse Proxy with PKI (Nginx Proxy Manager)



\## 📌 Overview

This project demonstrates building a secure reverse proxy environment using Docker and Nginx Proxy Manager, secured with a private Certificate Authority (PKI).



The lab simulates enterprise-style internal certificate trust and HTTPS traffic management.



---



\## 🧱 Architecture



\- Host OS: Windows 11

\- Hypervisor: VirtualBox

\- Admin VM: Zorin OS

\- Server VM: Ubuntu Server

\- Containers: Docker + Docker Compose

\- Reverse Proxy: Nginx Proxy Manager

\- Test Service: Traefik WhoAmI



---



\## 🔐 Security Components



\- Private Certificate Authority (OpenSSL)

\- Signed internal certificates

\- HTTPS termination

\- Trusted root certificate deployment

\- Secure container networking



---



\## 🛠️ Tools \& Technologies



\- Ubuntu Server

\- Docker / Docker Compose

\- OpenSSL

\- Nginx Proxy Manager

\- Portainer

\- VirtualBox

\- SSH



---



\## 📋 Implementation Steps



1\. Built Ubuntu Server VM

2\. Installed Docker \& Docker Compose

3\. Deployed Nginx Proxy Manager

4\. Created private CA

5\. Generated signed certificates

6\. Imported certs into proxy

7\. Configured HTTPS routing

8\. Verified trusted access



---



\## ✅ Results



\- Internal domains secured with HTTPS

\- Valid certificate chain

\- Encrypted proxy traffic

\- Centralized access management



---



\## 📚 Lessons Learned



\- Certificate lifecycle management

\- PKI trust chains

\- Reverse proxy architecture

\- Docker networking

\- TLS troubleshooting

\- Enterprise-style security design



---



\## 🚀 Future Improvements



\- ACME automation

\- Vault integration

\- SSO authentication

\- MFA gateway

\- Logging/monitoring stack



---



\## 📎 Screenshots



\_(Add screenshots here later)\_



---



\## 👤 Author



Gregg Petty  

Cybersecurity | IAM | Cloud Security



