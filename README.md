### 🛡️ Shells Overview

**Room:** [Shells Overview — TryHackMe](https://tryhackme.com/room/shellsoverview)  
**Status:** ✅ Completed  
**Date:** *07 June 2025* 

### 🎯 Objective
Learn about and practise using different types of shells in cyber security, including reverse shells, bind shells, and web shells. The focus was on understanding how each type works, how to deploy them manually, and how attackers use them in real-world scenarios.

---

### 🗝️ Key Concepts  
- **Shell** — A command-line interface that allows interaction with the OS. Attackers use shells to remotely control compromised machines.  
- **Reverse Shell** — Target connects back to the attacker’s machine. Common in real attacks to bypass firewalls.  
- **Bind Shell** — Target opens a port and listens for connections from the attacker. Easier to detect.  
- **Web Shell** — A script uploaded to a web server that executes OS commands remotely via a browser.  
- **Pivoting** — Using one compromised system as a launch point to access others in the network.  
- **Post-Exploitation** — Actions taken after initial access, like data theft, privilege escalation, or persistence.

---

### 🛠️ Tools Used
- **Netcat (nc)** — Used to create listeners or connect to remote shells.  
- **Ncat** — Improved version of Netcat with SSL support.  
- **Socat** — Used to create flexible socket connections between hosts.  
- **Rlwrap** — Wraps shells like Netcat to improve usability (e.g., arrow key support).  
- **PHP/Python/Bash scripts** — Various payloads used to generate shells.

---

### ⚠️ Challenges Faced
- Remembering the syntax for different reverse shell payloads across languages (especially Python and PHP) was tricky but improved with practice.
- Needed to test various listener tools to understand their behaviour and benefits (e.g., rlwrap vs ncat).
- Uploading and triggering a web shell felt realistic — had to properly format requests to make them work.

---

### 🧠 What I Learned
- Gained a solid understanding of how reverse, bind, and web shells function under the hood — not just tool-assisted setups.
- Learned the differences between each shell type and when an attacker might choose one over another.
- Practised several reverse shell one-liners in Bash, PHP, Python, AWK, and even BusyBox.
- Understood how web shells operate by executing commands via GET parameters, and how they’re often hidden in uploads.

---

### 🌐 Real-World Application:
> Knowing how shells work helps defenders detect unusual outbound connections or strange GET requests in logs. For attackers and penetration testers, it's key to be able to manually spawn shells when automated tools aren’t available or allowed.

---

### 💭 Reflections:
- This was one of the most hands-on and practical rooms. It really demystified shell payloads and made me more confident in setting them up manually.
