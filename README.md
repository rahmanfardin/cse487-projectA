# CSE487-projectA
# Securing a Networked System with Public Key Infrastructure (PKI)

This project is a moderately complex exercise in designing, configuring, and hardening a secure network environment using Public Key Infrastructure (PKI). The project involves both practical implementation and comprehensive documentation and presentation components.

## Project Goals

1. **Establish a Robust PKI:** Create and manage a hierarchical PKI with a Root CA (AcmeRootCA) and a Subordinate CA (AcmeSubCA).
2. **Secure Web Server Configuration:** Set up a secure web server (Apache2) with multiple websites and virtual hosts on a Linux machine.
3. **Domain Name System (DNS) Setup:** Configure a DNS server to handle multiple domains, subdomains, and both forward and reverse lookups.
4. **Firewall and OpenSSH Hardening:** Implement strict firewall rules and configure secure remote access using OpenSSH with a non-standard port.
5. **Certificate Management:** Handle the entire certificate lifecycle, from Certificate Signing Requests (CSR) generation and validation to issuance, installation, and revocation.
6. **Web Traffic Security:** Ensure secure (HTTPS) connections and automatic redirection from HTTP.
7. **Network Traffic Analysis:** Use Wireshark to observe and understand the TCP and TLS handshakes.
8. **Intrusion Detection and Prevention:** Configure an Intrusion Detection System (IDS) to detect and mitigate threats, including a simulated SYN flood attack.
9. **Advanced PKI Services:** Implement a self-service CA website and utilize Online Certificate Status Protocol (OCSP) for efficient certificate management.

## Project Requirements

* **Tools:** Linux host, Apache2, OpenSSL, Wireshark, IDS software
* **Knowledge:** PKI principles, web server configuration, DNS, firewalling, SSH, network protocols (TCP/IP, TLS), security best practices

## Detailed Tasks

1. **PKI Setup:**
   * Create and configure AcmeRootCA as the Root CA.
   * Create and configure AcmeSubCA as the Subordinate CA.
2. **Web Server Configuration:**
   * Install and configure Apache2.
   * Set up virtual hosts for `www.ewubdca.com`, `www.cnn.com`, and `www.bbc.com`.
3. **DNS Server Configuration:**
   * Configure DNS zones for the main domains and subdomains (`apply.ewubdca.com`, `download.ewubdca.com`).
   * Enable both forward and reverse DNS resolution.
4. **Firewall and OpenSSH Configuration:**
   * Configure firewall rules to allow only ports 22 (later changed to 3000), 53, 80, 443.
   * Install and configure OpenSSH, changing the default port to 3000.
5. **Certificate Management:**
   * Generate and submit CSRs for `www.ewubdca.com` and its subdomains.
   * Validate CSRs and issue certificates.
   * Transfer and install certificates on the web server.
6. **Web Traffic Security:**
   * Enforce HTTPS using the installed certificates.
   * Automatically redirect HTTP traffic to HTTPS.
7. **Network Traffic Analysis:**
   * Use Wireshark to capture and analyze TCP and TLS handshake packets.
8. **Intrusion Detection and Prevention:**
   * Configure and enable IDS.
   * Simulate a SYN flood attack.
   * Identify the attacker from IDS logs and block the attack.
9. **Advanced PKI Services:**
   * Create `www.acmeca.com` for self-service certificate issuance.
   * Configure and utilize OCSP for certificate revocation checking.

## Deliverables

* **Functional PKI:** A working, secure PKI infrastructure
* **Secure Web Server:** A hardened web server serving multiple sites over HTTPS
* **Detailed Report:** A comprehensive report documenting the entire project, including explanations, screenshots, and analysis
* **Oral Presentation:** A presentation summarizing the project, findings, and insights

## Project Summary Image

<a href="https://imgbb.com/"><img src="https://i.ibb.co/TwZsYHh/image.png" alt="image" border="0"></a>

## Disclaimer

This project is intended for educational purposes. Use the knowledge gained responsibly and in accordance with ethical guidelines.
