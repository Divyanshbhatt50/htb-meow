# Hack The Box – Meow 🐱

This repository contains my personal walkthrough and screenshots for the Hack The Box machine **Meow**, part of the Beginner Track.

---

## 🖥️ Machine Info

- **Name**: Meow  
- **IP Address**: `10.129.138.117`  
- **Difficulty**: Very Easy  
- **OS**: Linux  
- **Skills Demonstrated**:
  - Service enumeration with Nmap
  - Telnet basics
  - Accessing unsecured services
  - Linux command-line usage
  - Flag enumeration

---

## 🚀 Walkthrough

I started by scanning the target IP using Nmap:
**nmap -sV 10.129.138.117**
From the result, I found that only Telnet service (port 23/tcp) was open.

📸 Screenshot: ![🛰️ Nmap Scan Result](./screenshots/Nmap-Output.png)


Then I used the following command to connect via Telnet:
**telnet 10.129.138.117 23**

Once connected, it only asked for a username. I tried:
**root**

And I gained direct access into the system without any password.

📸 Screenshot: ![📡 Telnet Login](./screenshots/Telnet-Login.png)

After getting access inside Telnet, I started searching for files using:
**ls -la**

📸 Screenshot:![📁 File Listing](./screenshots/File-List.png)

I saw a file named flag.txt, so I ran:
**cat flag.txt**

This revealed the flag.

📸 Screenshot: ![🏁 Flag Captured](./screenshots/Flag-Access.png)

---

🙋‍♂️ About Me
I'm Divyansh Bhatt, a cybersecurity graduate and active Hack The Box learner, focused on hands-on security labs and CTF challenges.

🔗 GitHub: github.com/DivyanshBhatt

🔗 LinkedIn: linkedin.com/in/divyansh-bhatt-05637a335
