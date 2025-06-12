# Introduction to Network Security Basics
---
## Objective
Understand and demonstrate basic network security concepts by identifying threats, setting up a secure network, capturing and analyzing traffic, and documenting your findings.
---
## Proficiencies obtained
- Basic Network Security
- Threat Identification
- Firewall Configuration
- Packet Analysis (Wireshark)
---
## Tools used :-
- **Windows Defender Firewall**
- **Wireshark** (for traffic capturing and analysis)
- Alternatively, **Kali Linux** can be used since Wireshark is already included by default.
---
## Core Concepts covered in **Network Security** 
### Common Type of Network Threats
1. Viruses
   - A virus is a type of malicious software that attaches itself to legitimate programs or files.
   - It activates when the infected file is opened and can corrupt, delete, or steal data.
   - Requires user interaction to spread.
2. Worms
   - Unlike viruses, worms are self-replicating programs that spread automatically across networks without user action.
   - They consume bandwidth and system resources, potentially crashing systems or networks.
   - Often used to deploy additional malware.
3. Trojans
   - Trojans disguise themselves as legitimate software to trick users into installing them.
   - Once installed, they can open backdoors, steal data, or give attackers remote control of the system.
   - Do not replicate like viruses or worms.
4. Phishing Attacks
   - Involve fraudulent communication (usually emails or websites) that appear to come from trusted sources.
   - Aim to trick users into providing sensitive data such as passwords, credit card details, or login credentials.
   - Often combined with social engineering techniques.

### Basic Security Concepts
1. Firewalls
   - A firewall is a network security system that monitors and controls incoming and outgoing traffic.
   - It establishes a barrier between trusted internal networks and untrusted external networks (like the internet).
   - Can be hardware-based, software-based, or both.
2. Encryption
   - Encryption is the process of converting data into a coded format to prevent unauthorized access.
   - Commonly used in data transmission (e.g., HTTPS) and storage (e.g., encrypted hard drives).
   - Ensures confidentiality and integrity of data.
3. Secure Network Configurations
   - Involves setting up systems and networks in a way that reduces vulnerability to attacks.
   - Includes disabling unused ports/services, updating software, using strong authentication, and applying security patches.
   - Helps minimize the attack surface and prevents unauthorized access.

### Summary
#### Network threats such as viruses, worms, trojans, and phishing attacks exploit system vulnerabilities and human error to compromise data and systems. Understanding and applying basic security concepts like firewalls, encryption, and secure configurations is essential to defend against these threats and maintain network integrity and confidentiality.
---
## Implement **Basic Security Measures**

### Network Environment Setup:
- You can use your **home network** or a **virtual lab setup**:
  - **Home Network**:
    - Connect your Windows PC to your home Wi-Fi router.
    - Ensure at least one or two other devices (e.g., smartphone, laptop) are connected for testing.
  - **Virtual Lab** (Optional for advanced users):
    - Use virtualization software like VirtualBox or VMware.
    - Set up a virtual router and 1-2 virtual machines to simulate networked devices.

---

### Security Actions Taken:
1. **Open Windows Security Settings**:
   - Press `Windows + I` > Go to **"Update & Security"** > **"Windows Security"** > **"Firewall & network protection"**.
2. **Enable Firewall for All Profiles**:
   - Click on each network type: **Domain network**, **Private network**, **Public network**.
   - Ensure the toggle for **Windows Defender Firewall** is turned **ON** for all.
3. **Allow or Block Apps**:
   - In "Firewall & network protection", click **“Allow an app through firewall”**.
   - Review the list and uncheck apps you do not want to allow through the firewall.
4. **Advanced Settings** :
   - Click **Advanced settings** for detailed rule configuration (Inbound/Outbound).
   - You can create new rules to block/allow specific ports or programs.

---

### **Supervise Network Data** Transmission 
  - Configuration view of Windows Defender Firewall settings.
  - Live packet captures taken during active web browsing sessions.
  - Protocol-specific filters demonstrated, including:
    - **HTTP**: Web page requests and responses.
    - **DNS**: Monitoring domain name resolution processes.
    - **TCP Handshakes**: Connection initiations.
    - **ICMP**: Network diagnostics (ping).
  - Detection of Suspicious Network Activity:
    - Identified multiple failed TCP handshake attempts.
    - Noted anomalous DNS queries and access attempts to unknown external IP addresses.
    
---
### Set Up Basic Security Configurations
#### a. Change Default Passwords:
1. **Wi-Fi Router**:
   - Open a web browser and enter your router IP (commonly `192.168.0.1` or `192.168.1.1`).
   - Login with credentials (default ones should be changed).
   - Navigate to **Administration** or **Security** section and **change the admin password**.
2. **User Account Passwords**:
   - Go to `Settings > Accounts > Sign-in options`.
   - Ensure strong passwords or use Windows Hello for added security.

#### b. Enable Network Encryption (WPA2/WPA3):
1. **Access Router Settings** (as above).
2. Go to **Wireless Settings**.
3. Set:
   - **Security Mode** to **WPA2-Personal** or **WPA3-Personal**.
   - Use a **strong Wi-Fi password** (at least 12 characters with mix of letters, numbers, symbols).

---
### Summary

| Task          | Description                                         |
|---------------|-----------------------------------------------------|
| Network Setup | Use home or virtual setup with router + 1-2 devices |
| Firewall      | Enable and customize Windows Defender Firewall      |
| Passwords     | Change all default and weak passwords               |
| Encryption    | Set WPA2/WPA3 and strong Wi-Fi credentials          |

---

## How Basic Security Measures Help Protect the Network

Implementing basic security measures significantly strengthens a network’s defense. Here's how:
- **Firewall Configuration**: Filters and blocks unauthorized access, reducing the risk of intrusion.
- **Changing Default Passwords**: Prevents easy exploitation by attackers using known credentials.
- **Network Encryption (WPA2/WPA3)**: Secures data transmission and prevents unauthorized data interception.
- **Monitoring Traffic with Wireshark**: Helps detect suspicious activity and identify threats early.
- **Secure Network Configuration**: Reduces vulnerabilities by disabling unused services and tightening settings.
Together, these steps build a layered defense that protects even small networks from common cyber threats.

---
## Reflection on Security Best Practices

### Additional Measures for Larger Networks
In a larger or enterprise network, more robust security controls are essential. These may include:
- **Intrusion Detection and Prevention Systems (IDS/IPS)** to monitor and react to malicious traffic.
- **Virtual LANs (VLANs)** to isolate departments or critical assets.
- **Centralized Authentication Systems** (e.g., RADIUS, LDAP) for managing user access securely.
- **Endpoint Detection and Response (EDR)** tools to monitor all endpoints.
- **Regular Patch Management** to fix known vulnerabilities promptly.
- **Network Access Control (NAC)** to ensure only authorized devices connect.

### Educating Others About Network Security

#### Educating others is crucial because human error is a common cause of security breaches. I would conduct awareness sessions emphasizing simple practices like **avoiding suspicious links, using strong passwords, enabling two-factor authentication, and updating software regularly**. Using real-life examples and interactive demonstrations, I would show how small actions can prevent large-scale security incidents, making network safety a shared responsibility.

---

##  Deliverables
- Report File: `network_security_report.pdf`
- Screenshots: `ssfile.pdf`
- This `README.md` file
  
---

## Author
**Intern Name**: _SATVIK BHAGAT_  
**Internship**: Cyber Security Internship @ The Red Users  
**Duration**: [25-05-2025] – [25-06-2025]
---
