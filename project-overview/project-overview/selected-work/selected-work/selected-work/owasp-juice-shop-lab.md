# OWASP Juice Shop Security Lab

## Overview

This lab documents a controlled offensive cybersecurity exercise using **OWASP Juice Shop**, a deliberately vulnerable web application designed for security training, awareness demonstrations, CTFs, and security-tool testing.

The objective of this exercise was to demonstrate how an offensive security practitioner can establish a controlled laboratory environment, deploy a vulnerable target, identify weaknesses, and safely investigate web application security issues.

> **Important:** All activities described in this lab are intended for authorized, isolated training environments only.

---

## Lab Objectives

The laboratory exercise focused on:

* Building a controlled web application security testing environment.
* Deploying OWASP Juice Shop inside a Kali Linux laboratory.
* Understanding the role of intentionally vulnerable applications in offensive-security training.
* Practicing vulnerability identification in an authorized environment.
* Developing a structured methodology for web application security assessment.
* Connecting practical testing activities with broader offensive cybersecurity principles.

---

## Laboratory Environment

### Primary Platform

* Kali Linux
* Oracle VM VirtualBox
* OWASP Juice Shop
* Node.js

### Target

**OWASP Juice Shop**

OWASP Juice Shop is an intentionally insecure web application containing vulnerabilities representative of real-world web application security weaknesses.

It includes challenges covering the OWASP Top Ten and additional security flaws, making it suitable for controlled security testing and training.

---

## Lab Architecture

The laboratory was designed around an isolated security-testing workflow:

```text
┌──────────────────────────────┐
│        Kali Linux VM         │
│                              │
│  Security Testing Tools      │
│  Terminal / Browser / Proxy  │
└──────────────┬───────────────┘
               │
               │ Authorized Testing
               ▼
┌──────────────────────────────┐
│       OWASP Juice Shop       │
│                              │
│   Intentionally Vulnerable   │
│      Web Application         │
└──────────────────────────────┘
```

The target application is used strictly as a laboratory target rather than an unauthorized external system.

---

# Deployment Procedure

## Step 1 — Start the Kali Linux Environment

The first stage involved launching the Kali Linux virtual machine through Oracle VM VirtualBox.

The Kali environment serves as the primary security-testing workstation.

---

## Step 2 — Open the Terminal

After starting Kali Linux, the terminal was opened to prepare the environment.

The terminal can be accessed through the Kali desktop environment or the standard terminal keyboard shortcut.

---

## Step 3 — Update the Laboratory Environment

Before installing the required components, the Kali Linux package repositories were updated.

```bash
sudo apt update
```

The system packages can then be upgraded where appropriate:

```bash
sudo apt upgrade
```

Keeping the laboratory workstation updated helps ensure that required packages and dependencies are available.

---

## Step 4 — Install Node.js

OWASP Juice Shop is built using JavaScript technologies and requires Node.js for running the application from source.

The laboratory setup therefore includes Node.js as part of the application environment.

Example installation:

```bash
sudo apt install nodejs
```

Verify the installation:

```bash
node --version
```

---

# Step 5 — Deploy OWASP Juice Shop

OWASP Juice Shop can be deployed using several supported approaches, including Node.js and container-based deployment.

For this laboratory, the application was prepared as a controlled local security-testing target.

The official OWASP project provides multiple installation approaches and documentation.

---

# Step 6 — Establish the Safe Practice Target

The purpose of deploying Juice Shop is to create an intentionally vulnerable target where offensive-security techniques can be practiced legally.

The target provides a controlled environment for investigating issues such as:

* Authentication weaknesses
* Authorization problems
* Injection vulnerabilities
* Cross-site scripting
* Access-control weaknesses
* Security misconfigurations
* Client-side security issues
* API-related weaknesses
* Other vulnerabilities represented within the Juice Shop challenge environment

---

# Step 7 — Security Testing Methodology

The laboratory follows a structured assessment process rather than simply attempting random attacks.

### Phase 1 — Reconnaissance

Identify:

* Application structure
* Available endpoints
* Application functionality
* Authentication mechanisms
* Client-side technologies
* API interaction points

### Phase 2 — Enumeration

Investigate:

* Routes
* Parameters
* Requests
* Responses
* Authentication flows
* Application behaviour

### Phase 3 — Vulnerability Identification

Analyze the application for weaknesses and determine whether observed behaviour represents a security issue.

### Phase 4 — Controlled Validation

Where appropriate, validate the identified weakness against the intentionally vulnerable laboratory target.

### Phase 5 — Impact Assessment

Determine:

* What security property is affected?
* What access could potentially be obtained?
* What information could be exposed?
* What business/security impact could result?

### Phase 6 — Remediation

Document defensive recommendations and explain how the weakness could be mitigated in a properly secured application.

---

# Step 8 — Evidence and Documentation

A professional security assessment should not end with identifying a vulnerability.

Each finding should be documented with:

```text
Finding
   ↓
Affected Component
   ↓
Observation
   ↓
Security Impact
   ↓
Controlled Validation
   ↓
Risk
   ↓
Recommended Remediation
```

This approach helps transform an offensive-security exercise into a professional security assessment.

---

# Key Learning Outcomes

Through this laboratory, the following practical skills were developed and reinforced:

* Secure laboratory construction
* Web application reconnaissance
* Vulnerability identification
* Controlled offensive-security testing
* Security evidence collection
* Risk interpretation
* Security remediation thinking
* Ethical hacking methodology
* OWASP-aligned application-security assessment

---

# Ethical Scope

This project is strictly intended for:

* Authorized security testing
* Cybersecurity education
* Security research
* Controlled laboratory environments
* Defensive security improvement

Testing should only be conducted against systems for which explicit authorization has been obtained.

Never apply techniques demonstrated in this laboratory against third-party systems without appropriate permission.

---

# Portfolio Significance

This laboratory forms part of the practical cybersecurity work associated with:

**THE INVISIBLE WAR — Volume I: The Invisible Attacker**

*A Mystic-Spiritual Guide to Offensive Cybersecurity*

The complete publication contains additional educational material, practical exercises, methodology, and controlled laboratory content.

This repository intentionally provides only a **selected portfolio demonstration** rather than reproducing the complete commercial publication.

---

## Related Project

**THE INVISIBLE WAR — Volume I: The Invisible Attacker**

Author: **Sodiq Adewale Babayemi**

Published by: **AI Info Tech Learning**

The complete book is commercially available through the author's official sales channels.

---

## Disclaimer

This portfolio project is provided for educational and authorized security-testing purposes.

The author does not encourage unauthorized access, exploitation, disruption, theft, or misuse of computer systems, networks, applications, or digital resources.

All practical testing should be performed within explicitly authorized and controlled environments.
