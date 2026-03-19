   # Wireless Security Assessment (WiFi & Bluetooth)

## Overview

Conducted a comprehensive wireless security assessment focusing on WiFi and Bluetooth communication. The project evaluates common vulnerabilities in wireless networks, demonstrates practical attack techniques, and implements security mechanisms such as encryption, authentication, and secure data transmission.

The assessment includes both offensive testing (wireless attacks) and defensive implementations (encryption, VPN, IDS).

---

## Objectives

* Identify vulnerabilities in wireless communication (WiFi & Bluetooth)
* Demonstrate real-world wireless attack techniques
* Analyze encryption and authentication mechanisms
* Implement secure wireless communication practices

---

## Tools Used

* Kali Linux
* Aircrack-ng Suite
* Airodump-ng
* Aireplay-ng
* Aircrack-ng
* Wireshark
* OpenVPN
* Snort IDS

---

## Methodology

### 1. Reconnaissance

* Identified wireless interfaces using `iwconfig`
* Enabled monitor mode using `airmon-ng`
* Scanned nearby networks using `airodump-ng`

### 2. Wireless Attack Simulation

* Captured WPA/WPA2 handshake
* Performed deauthentication attack
* Executed dictionary attack using Aircrack-ng

### 3. Bluetooth Analysis

* Discovered nearby Bluetooth devices
* Analyzed device visibility and pairing security

### 4. Security Implementation

* Configured WPA2/WPA3 encryption
* Implemented secure authentication (RADIUS)
* Setup VPN (OpenVPN) for encrypted communication
* Applied IDS monitoring using Snort

---

## Key Findings

* Weak WiFi passwords are vulnerable to dictionary attacks
* WPA2 networks can be targeted via handshake capture
* Bluetooth devices in discoverable mode increase attack surface
* Lack of encryption exposes wireless traffic to interception

---

## Proof of Concept

### WiFi Handshake Capture

* Captured WPA handshake using airodump-ng
* Forced reconnection using deauthentication attack

![Handshake Capture](images/handshake.png)

---

### Password Cracking

* Performed dictionary attack using Aircrack-ng
* Successfully recovered weak password

![Password Crack](images/crack.png)

---

### Network Traffic Analysis

* Used Wireshark to analyze encrypted vs unencrypted traffic

![Wireshark Analysis](images/wireshark.png)

---

## Impact

* Unauthorized access to wireless network
* Data interception risk
* Potential man-in-the-middle attacks
* Unauthorized device connections

---

## Mitigation

* Use strong, complex passwords
* Upgrade to WPA3 encryption
* Disable WPS
* Limit device discoverability (Bluetooth)
* Use VPN for secure communication
* Implement network monitoring (IDS)

---

## Key Learning

* Wireless networks are highly exposed attack surfaces
* Weak credentials are a major security risk
* Encryption and authentication are critical for protection
* Continuous monitoring improves detection of attacks

---

## Full Report

Detailed documentation available in: [report.pdf]
