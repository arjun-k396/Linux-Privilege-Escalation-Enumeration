# Linux Privilege Escalation Enumeration

🎓 Cybersecurity Student | Ethical Hacking Learner  
💻 Hands-on practice of Linux privilege escalation enumeration techniques used in cybersecurity labs.

---

## ⚠️ Disclaimer
This project is created for educational purposes only.  
All commands are tested in controlled environments (Kali Linux / TryHackMe labs).  
Do not use these techniques on unauthorized systems.

---

## 🔍 Topics Covered

### 1️⃣ Sudo Permissions
- `sudo -l` – Check allowed sudo commands  
- `sudo -V` – Show sudo version and configuration  
- `sudo -u root whoami` – Test sudo access  
- `sudo -u user command` – Run command as another user  

📸 Screenshots: screenshots/sudo/

---

### 2️⃣ SUID Files
- `find / -perm -4000 2>/dev/null` – Find SUID binaries  
- `find / -user root -perm -4000 2>/dev/null` – Root-owned SUID files  
- `ls -la /usr/bin | grep s` – Check SUID binaries  
- `getcap -r / 2>/dev/null` – Find file capabilities  

📸 Screenshots: screenshots/suid/

---

### 3️⃣ Writable Files
- `find / -writable 2>/dev/null` – Find writable files  
- `find / -type d -writable 2>/dev/null` – Writable directories  
- `ls -la /tmp` – Check temporary directory  
- `ls -ld /var/tmp` – Check permissions  

📸 Screenshots: screenshots/writable-files/

---

### 4️⃣ Cron Jobs
- `crontab -l` – List user cron jobs  
- `ls -la /etc/cron*` – System cron jobs  
- `cat /etc/crontab` – View cron configuration  
- `ls -la /var/spool/cron` – User cron jobs  

📸 Screenshots: screenshots/cron-jobs/

---

### 5️⃣ Environment Variables
- `env` – Display environment variables  
- `printenv` – Show environment variables  
- `echo $PATH` – Show PATH variable  
- `echo $HOME` – Show home directory  

📸 Screenshots: screenshots/env/

---

## 🛠 Tools Used
- Kali Linux  
- Bash Terminal  
- Git  
- GitHub  

---

## 🎯 Learning Outcomes
- Understand privilege escalation concepts  
- Identify misconfigurations in Linux systems  
- Perform system enumeration for ethical hacking  
- Build hands-on cybersecurity skills  

---

## 📁 Repository Structure
