
# Safe Offensive Cybersecurity Labs

## Overview

This portfolio project presents a controlled laboratory methodology for learning and demonstrating offensive cybersecurity techniques safely.

The practical exercises are designed around intentionally vulnerable environments, particularly **Kali Linux** and **OWASP Juice Shop**, allowing reconnaissance, vulnerability identification, attack simulation, documentation, and defensive reflection without targeting real-world systems.

> **Ethical boundary:** All activities are performed only against systems that are owned, intentionally vulnerable, or explicitly authorized for security testing.

## Laboratory Environment

The practical environment developed for the project includes:

* Kali Linux
* Oracle VM VirtualBox
* OWASP Juice Shop
* Nmap
* Burp Suite Community
* Directory discovery tools
* Local virtual networking
* A structured lab journal for documenting findings

OWASP Juice Shop is an intentionally insecure web application designed for security training, awareness demonstrations, CTFs, and security-tool testing.

## Lab Methodology

The offensive-security workflow follows a controlled progression:

1. **Environment Preparation**

   * Establish the isolated laboratory.
   * Deploy the vulnerable training application.
   * Verify that the target is locally accessible.

2. **Reconnaissance**

   * Identify available services.
   * Map the application's attack surface.
   * Record relevant observations.

3. **Application Mapping**

   * Examine login functionality.
   * Identify input points.
   * Observe application routes and interfaces.
   * Document the structure of the test environment.

4. **Controlled Vulnerability Testing**

   * Use intentionally vulnerable challenges.
   * Examine security weaknesses within the training application.
   * Study authentication, input validation, XSS, SQL-injection and related security concepts.

5. **Analysis**

   * Record observations and results.
   * Identify the security weakness involved.
   * Consider how the weakness could affect a real organization.

6. **Defensive Reflection**

   * Determine how the vulnerability could be mitigated.
   * Translate offensive observations into defensive recommendations.
   * Maintain responsible-use principles throughout the exercise.

## Example: Safe Reconnaissance

The manuscript demonstrates reconnaissance against the local laboratory environment using Nmap.

Example target:

`127.0.0.1`

The exercise focuses on identifying services and understanding the exposed attack surface while ensuring that reconnaissance remains inside the controlled lab.

The manuscript also introduces service/version identification and documentation of observed results.

## OWASP Juice Shop Practice

The laboratory uses OWASP Juice Shop as the primary vulnerable web-application target.

Practice areas include:

* Authentication weaknesses
* Input validation
* Cross-site scripting concepts
* SQL injection concepts
* Application navigation
* Security challenge analysis

The purpose is not simply to exploit vulnerabilities, but to understand **why the weakness exists, how it can be identified, and how defenders can reduce the risk**.

## Offensive Attack Workflow

The project introduces a structured offensive workflow:

**Reconnaissance → Mapping → Weakness Identification → Controlled Testing → Analysis → Documentation → Defensive Recommendations**

This approach demonstrates how offensive security can be conducted as a disciplined assessment process rather than uncontrolled exploitation.

## Case Study Approach

The later laboratory exercises extend the methodology into simulated offensive-security case studies.

A typical case study involves:

* Selecting a controlled target
* Defining assessment objectives
* Mapping the target
* Planning safe testing activities
* Executing the assessment inside the laboratory
* Recording observations
* Evaluating results
* Producing defensive recommendations

The final documentation is designed to resemble the structure and discipline expected in professional penetration-testing reporting.

## Security & Ethics

A central principle of the project is responsible security practice.

The laboratory explicitly prohibits testing systems without authorization.

The practical exercises are intended to develop:

* Technical awareness
* Reconnaissance skills
* Vulnerability-analysis skills
* Security documentation
* Attacker-perspective thinking
* Defensive reasoning
* Ethical decision-making

## Portfolio Evidence

The complete project contains practical laboratory material, visual demonstrations, methodology, and structured exercises.

This public repository intentionally provides a **selected portfolio preview** rather than the complete commercial manuscript.

### Full Publication

The complete *THE INVISIBLE WAR – Volume I: The Invisible Attacker* is commercially published by **AI Info Tech Learning**.

For the complete book and full laboratory material:

* [Purchase through Selar](https://selar.com/655l633a37)
* [Purchase through Amazon](https://www.amazon.co.uk/dp/B0GTGGWVYY)

## Source Publication

**THE INVISIBLE WAR – Volume I: The Invisible Attacker**

*A Mystic-Spiritual Guide to Offensive Cybersecurity*

**Author:** Sodiq Adewale Babayemi
**Publisher:** AI Info Tech Learning
**Organization:** AI Info Tech Limited

The GitHub repository contains selected educational material and portfolio evidence only. The full manuscript remains commercially protected.

## Disclaimer

This portfolio material is provided for educational and cybersecurity-awareness purposes.

Do not perform security testing against systems, networks, applications, accounts, or infrastructure without explicit authorization.

Always conduct offensive-security exercises within an isolated laboratory, authorized assessment environment, or intentionally vulnerable training platform.
