# 🔐 SQROCK IT Solution — Cybersecurity Internship

# Day 7: Password Attacks & Credential Stuffing — Local Lab

![Kali Linux](https://img.shields.io/badge/Kali_Linux-2026.2-557C94?logo=kalilinux\&logoColor=white)
![Python](https://img.shields.io/badge/Python-3.13.12-3776AB?logo=python\&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-Local_Lab-000000?logo=flask\&logoColor=white)
![Cybersecurity](https://img.shields.io/badge/Cybersecurity-Training-red)
![Password Security](https://img.shields.io/badge/Password-Security-orange)
![Brute Force Simulation](https://img.shields.io/badge/Brute_Force-Simulation-yellow)
![Defensive Security](https://img.shields.io/badge/Defensive-Security-green)
![Ethical Hacking](https://img.shields.io/badge/Ethical-Hacking-blue)
![Lab Only](https://img.shields.io/badge/Environment-Local_Lab-purple)

---

## 📌 Project Overview

As part of **Day 7 of the SQROCK IT Solution Cybersecurity Internship**, this project focuses on understanding **password attacks, brute-force attacks, and credential stuffing** from both an offensive-awareness and defensive-security perspective.

The project uses a **local Flask test server** to simulate repeated login attempts using dummy credentials. The objective is to demonstrate how attackers may systematically attempt passwords while also developing an understanding of defensive mechanisms such as **rate limiting, account protection, and authentication controls**.

The entire exercise was performed in a controlled local laboratory environment using `localhost`. No real accounts, credentials, websites, or external systems were targeted.

---

## 🎯 Objectives

The main objectives of this project were to:

* Understand the concept of password attacks.
* Differentiate between brute-force attacks, dictionary attacks, and credential stuffing.
* Understand how repeated authentication attempts can be detected.
* Build a local Flask authentication test server.
* Simulate repeated login attempts using dummy credentials.
* Observe how an application responds to repeated authentication requests.
* Implement a basic defensive rate limiter.
* Understand the importance of MFA, account lockout, CAPTCHA, and password hygiene.
* Develop practical skills in Python and Flask.
* Practice ethical and controlled security testing.

---

## 🛠️ Tools and Technologies Used

| Tool / Technology     | Purpose                                   |
| --------------------- | ----------------------------------------- |
| **Kali Linux 2026.2** | Cybersecurity laboratory environment      |
| **Python 3.13.12**    | Programming and automation                |
| **Flask**             | Local web application/test server         |
| **Python Requests**   | Sending local HTTP requests               |
| **HTML**              | Login page structure                      |
| **Terminal**          | Running and testing the application       |
| **Nano**              | Creating and editing project files        |
| **Git & GitHub**      | Version control and project documentation |

---

## 🧠 Skills Demonstrated

* Password security awareness
* Brute-force attack concepts
* Credential stuffing concepts
* Authentication testing
* Python programming
* Flask web application development
* HTTP request handling
* Local security testing
* Rate-limiting implementation
* Defensive security
* Linux command-line skills
* Security documentation
* Ethical hacking principles

---

## 🔬 Methodology

The project followed a controlled laboratory methodology:

### Step 1 — Study Password Attack Concepts

The first stage involved understanding the differences between common password attacks.

### Brute Force

A brute-force attack systematically attempts different password combinations until a valid credential is found.

### Dictionary Attack

A dictionary attack uses a predefined list of commonly used or previously known passwords.

### Credential Stuffing

Credential stuffing uses previously leaked username/password combinations against another service, relying on password reuse.

---

### Step 2 — Create a Local Flask Server

A simple Flask application was created to provide a controlled login endpoint.

The server was configured to run locally:

```text
http://127.0.0.1:5000
```

This ensured that the exercise remained inside the authorized laboratory environment.

---

### Step 3 — Create Dummy Credentials

The test application used fictional credentials for educational purposes.

Example:

```text
Username: testuser
Password: TrainingPassword123
```

No real credentials were used.

---

### Step 4 — Test Authentication Requests

A Python testing script was used to send a controlled sequence of login requests to the local Flask server.

The purpose was to observe:

* Successful authentication
* Failed authentication
* Repeated login attempts
* Server responses
* Authentication behavior

---

### Step 5 — Implement Defensive Rate Limiting

A basic rate-limiting mechanism was introduced to demonstrate how applications can restrict excessive authentication attempts.

The defensive mechanism can:

* Count repeated attempts
* Identify excessive requests
* Temporarily block further attempts
* Reduce automated password guessing
* Protect authentication endpoints

---

### Step 6 — Analyze the Results

The final stage involved reviewing the authentication logs and comparing the behavior before and after the defensive mechanism was introduced.

The analysis focused on:

* Number of login attempts
* Failed authentication attempts
* Successful authentication
* Repeated requests
* Rate-limit behavior
* Security improvements

---

## 🧪 Laboratory Environment

The project was performed in an isolated cybersecurity training environment.

```text
Operating System : Kali Linux 2026.2
Python           : 3.13.12
Framework        : Flask
Testing Address  : 127.0.0.1
Port             : 5000
Environment      : Localhost / Authorized Lab
```

### Environment Architecture

```text
┌──────────────────────────────┐
│       Kali Linux 2026.2     │
│                              │
│  ┌────────────────────────┐  │
│  │   Flask Test Server    │  │
│  │   127.0.0.1:5000       │  │
│  └────────────┬───────────┘  │
│               │              │
│               ▼              │
│  ┌────────────────────────┐  │
│  │ Python Authentication   │  │
│  │ Test / Simulation       │  │
│  └────────────┬───────────┘  │
│               │              │
│               ▼              │
│  ┌────────────────────────┐  │
│  │ Rate Limiting /        │  │
│  │ Defensive Controls     │  │
│  └────────────────────────┘  │
└──────────────────────────────┘
```

---

## ⚙️ Environment Configuration

The project directory was created inside the SQROCK internship workspace.

```bash
mkdir -p ~/sqrock-internship/day7-password-attacks
cd ~/sqrock-internship/day7-password-attacks
```

Python version was verified using:

```bash
python3 --version
```

Expected environment:

```text
Python 3.13.12
```

Flask can be installed in the laboratory environment with:

```bash
python3 -m pip install flask requests
```

---

## 📂 Project Structure

```text
day7-password-attacks/
│
├── app.py
├── brute_force_simulator.py
├── rate_limiter.py
├── login.html
├── attack_log.txt
├── analysis.md
```

### File Description

| File                       | Description                        |
| -------------------------- | ---------------------------------- |
| `app.py`                   | Local Flask authentication server  |
| `brute_force_simulator.py` | Controlled login-attempt simulator |
| `rate_limiter.py`          | Defensive rate-limiting logic      |
| `login.html`               | Local login interface              |
| `attack_log.txt`           | Authentication/testing results     |
| `analysis.md`              | Security analysis and findings     |
              
---

## 🔐 Defensive Security Measures

The project demonstrated several mechanisms that can reduce the impact of password attacks.

### 1. Rate Limiting

Limits the number of authentication requests that can be made within a specific period.

### 2. Account Lockout

Temporarily disables an account after multiple failed authentication attempts.

### 3. Multi-Factor Authentication

MFA provides an additional authentication factor beyond the password.

### 4. CAPTCHA

CAPTCHA can help distinguish automated requests from normal human interaction.

### 5. Strong Password Policies

Users should avoid predictable and reused passwords.

### 6. Breach Monitoring

Organizations can monitor for compromised credentials and require affected users to change passwords.

### 7. Login Monitoring

Security teams can monitor authentication logs for unusual patterns such as:

* Large numbers of failed attempts
* Repeated requests from the same source
* Multiple usernames being tested
* Unusual login times
* Geographic anomalies

## ⚠️ Security and Ethical Considerations

This project was conducted strictly for **authorized cybersecurity education and awareness training**.

The following restrictions were maintained:

* Testing was performed only against `localhost`.
* Only fictional credentials were used.
* No real accounts were targeted.
* No external websites were tested.
* No stolen credential databases were used.
* No real users were affected.
* No unauthorized access was attempted.
* The exercise was performed within the SQROCK IT Solution internship laboratory environment.

> **Important:** Password-testing techniques should only be used against systems where explicit authorization has been provided.

## 🎓 Learning Outcomes

After completing this project, I gained practical understanding of:

* How brute-force attacks work conceptually.
* How credential stuffing differs from brute force.
* How authentication endpoints can be abused through repeated requests.
* How Python can be used to automate controlled security tests.
* How Flask can be used to create a local security-testing environment.
* How rate limiting can mitigate automated authentication attempts.
* Why MFA is important for account protection.
* Why password reuse increases security risks.
* How authentication logs can support security monitoring.
* The importance of conducting cybersecurity testing ethically.

## 🏆 Project Conclusion

Day 7 provided practical exposure to **password security and authentication attacks** within a controlled cybersecurity laboratory.

By combining a local Flask authentication server, Python-based testing, and defensive rate limiting, the project demonstrated both the mechanics of repeated authentication attempts and the importance of implementing appropriate security controls.

The exercise strengthened my understanding of **Python, Flask, authentication security, password attacks, defensive programming, and ethical cybersecurity testing**.

---
