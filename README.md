# 🧪 Kali Linux Home Lab (No-Code)

This repository documents my personal home lab setup, where I experimented with offensive security tools on a Kali Linux virtual machine. Although there is no source code, this README captures the technical learning and exercises performed.

---

## ⚙️ Environment Setup

I installed **Kali Linux (Debian 12.x 64-bit Arm)** on my MacBook using **VMware Fusion**.

- **Host OS:** macOS
- **Virtualization:** VMware Fusion
- **VM Specs:**
  - 4 CPU cores
  - 2048 MB memory
  - Shared internet with host (NAT)

The VM serves as my **attacker machine** for various cybersecurity experiments.

---

## 🧰 Tools Explored

### 🔍 Nmap — Network Scanning

I used Nmap to identify open ports, running services, and OS information on target machines within a private network.

**Skills Practiced:**

- TCP SYN scan (`-sS`)
- Full port scan (`-p-`)
- OS and service detection (`-A`)
- NSE script usage

---

### 🌐 Gobuster — Directory Brute-Forcing

Used Gobuster to find hidden directories and files on web servers.

**Example Wordlist:**  
`/usr/share/wordlists/dirb/common.txt`

**Common Findings:**

- `/phpmyadmin`
- `/uploads`
- `/config`

---

### 📶 Wireshark — Packet Analysis

Captured and analyzed traffic from insecure web sessions.

**Key Takeaways:**

- Observed plaintext HTTP POST credentials
- Analyzed session cookies and headers
- Reinforced the importance of HTTPS

---

## 💻 Metasploit & Keylogger Integration

I also used this Kali Linux machine as the **attacker host** in my separate [Hacking Tools](#) project.

Using Metasploit, I exfiltrated keystrokes from my MacBook (target) to my Kali VM via a custom keylogger payload. This exercise helped me understand real-world post-exploitation techniques in a controlled lab environment.

---

## 🧠 Lessons Learned

- Enumeration is the foundation of any attack strategy
- Hidden directories often expose serious misconfigurations
- Packet sniffing reveals the dangers of insecure protocols
- Metasploit provides powerful capabilities for post-exploitation

---

## ✅ Next Steps

- Add IDS/IPS tools like **Snort** or **Suricata**
- Set up a Windows-based target for Red Team practice
- Automate scans and reports with Bash or Python
- Document defensive tooling in a Blue Team counterpart repo

---

> 💡 *This project is for educational and ethical hacking purposes only.*
