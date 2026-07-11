# AWS DevOps Engineer Intern Assignment

## Objective
Deploy a simple static website on an AWS EC2 Ubuntu instance using the Nginx web server.

---

## Task 1: EC2 Setup

1. Logged in to AWS Management Console.
2. Launched an Ubuntu EC2 Instance.
3. Created a Security Group.
4. Allowed:
   - Port 22 (SSH)
   - Port 80 (HTTP)
5. Downloaded the Key Pair (.pem file).
6. Connected to the EC2 instance using SSH.

SSH Command:

```bash
ssh -i "contactapp.pem" ubuntu@13.233.74.176
```

---

## Task 2: Install Nginx

Updated the package list:

```bash
sudo apt update
```

Installed Nginx:

```bash
sudo apt install nginx -y
```

Checked Nginx status:

```bash
systemctl status nginx
```

Restarted Nginx:

```bash
sudo systemctl restart nginx
```

Checked Disk Usage:

```bash
df -h
```

Checked Memory Usage:

```bash
free -h
```

Checked Running Processes:

```bash
ps aux
```

---

## Task 3: Host Website

1. Created a simple HTML page.
2. Added:
   - Name
   - College
   - Branch
   - Email
   - Current Date
3. Replaced the default Nginx page.
4. Accessed the website using the EC2 Public IP.

Example:

```
http://13.233.74.176/
```

---

## Git Commands Used

```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin <GitHub-Repository-URL>
git push -u origin main
```

---

## AWS Services Used

- Amazon EC2
- Security Groups

---

## Web Server

- Nginx

---

## Author

**Name:** Mitesh Baikar
