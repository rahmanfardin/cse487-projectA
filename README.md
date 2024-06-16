# CSE487-projectA
Project: Securing a networked system with PKI

Activity: Moderately complex security systems design project with report writing and oral presentation


##Requirements: 

Configuration of Certification Authority AcmeCA with AcmeRootCA as the RootCA.
Configuration of the SubCA as the AcmeSubCA.
Configuration of the Web Server with Apache2 on a Linux Host. 
Configuration of multiple websites on a single server. 
DNS server configuration to resolve www.ewubdca.com, www.cnn.com, www.bbc.com. For both forward and reverse zones. DNS server should resolve multiple domains.
DNS server configuration to resolve two subdomains:
apply.ewubdca.com 
download.ewubdca.com
Firewall configuration to allow necessary ports (22, 53, 80, 443, 3000) only, deny all other ports.
Installing and configuring OpenSSH to enable SSH to the server and the CA.
Change the SSH default port from 22 to 3000.
CSR Configuration and Generation for the www.ewuca.com and for any of its subdomains *..ewuca.com
Create a webpage and place a form to take CSR from the visitors as text input, and include textboxes to take relevant information from the requester for Organizational Validation.
Transfering the CSR to AcmeCA by SFTP/SCP/VM networking/CA Web-interface. 
Certification process (Verification and Certificate Generation from CSR).
Transferring the certificate from AcmeCA to the server www.verysecureserver.com by SFTP/SCP/VM networking. 
Installation of the signed the SSL certificate in the server of www.verysecureserver.com
Making the system trust Acme-RootCA (the certificate of the SubCA should not be imported into the client PC). 
Implementation of a simple file uploading page in the server. 
Automatically redirect all http:// traffic to https:// 
Verifying the security of the connection by inspection (the padlock icon).
Identify the TCP three-way-handshake and TLS four-way-handshake packets in Wireshark from another computer while connecting to https://www.verysecureserver.com
Revoke the certificate issued to www.verysecureserver.com from the CA and distribute the first CRL.
Verifying the revocation of previous certificate from the CRL (no padlock icon).
Configuring IDS, and demonstrating a SYN flood attack and identifying the attacker from the log files. 
Block the attack by any means (e.g., blacklist the attacker’s ip address in the firewall).
Creating a Website called www.acmeca.com where the users can paste their CSRs and get a signed certificate ready to be downloaded.
Configuring OCSP to manage certificates and CRLs.
Revoke the certificate and show the padlock is gone.
