# 🧪 Kali Linux Home Lab Documentation

This repository documents my personal home lab setup, where I experimented with offensive security tools on a Kali Linux virtual machine.

---

## ⚙️ Environment Setup

I installed **Kali Linux (Debian 12.x 64-bit Arm)** on my MacBook using **VMware Fusion**.

- **Host OS:** macOS
- **Virtualization:** VMware Fusion
- **VM Specs:**
  - 4 CPU cores
  - 2048 MB memory
  - Shared internet with host (NAT)

---

## 🧰 Tools Explored

### 🔍 Nmap — Network Scanning

I used Nmap to identify open ports, running services, and OS information on target machines within a private network.

**Skills Practiced:**

- TCP SYN scan (`-sS`)
- Full port scan (`-p-`)
- OS and service detection (`-A`)

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

- Analyzed session cookies and headers
- Reinforced the importance of HTTPS
- Learned to filter packets by criteria

---

## 💻 Metasploit & Keylogger Integration

I also used this Kali Linux machine as the **attacker host** in my separate [Hacking Tools](#) project.

Using Metasploit, I exfiltrated keystrokes from my MacBook (victim) to my Kali VM (attacker). This exercise helped me understand real-world post-exploitation techniques in a controlled lab environment.

---

> 💡 *This project is for educational and ethical hacking purposes only.*
