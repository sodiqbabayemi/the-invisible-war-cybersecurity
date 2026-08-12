# Cybersecurity Methodology

## Overview

The methodology presented in *The Invisible War – Volume I: The Invisible Attacker* is designed to move the learner from cybersecurity theory into controlled, practical offensive-security activities.

The approach emphasizes **understanding, observation, controlled experimentation, validation, and responsible security practice** rather than unauthorized exploitation.

The practical methodology follows a progressive model:

1. **Understand the security concept**
2. **Identify the attack surface**
3. **Establish a controlled laboratory environment**
4. **Observe the target and its behaviour**
5. **Test identified weaknesses**
6. **Validate findings**
7. **Document the results**
8. **Apply appropriate defensive thinking**

## 1. Authorized Environment First

All practical offensive-security activities should be performed only against systems for which the tester has explicit authorization.

The book therefore uses deliberately vulnerable training environments rather than real-world systems.

A key example is **OWASP Juice Shop**, an intentionally insecure web application designed for security training, awareness demonstrations, CTF activities, and security-tool testing. OWASP describes Juice Shop as encompassing vulnerabilities from the OWASP Top 10 and other real-world security flaws.

This establishes the fundamental rule:

> **Operate only within authorized environments.**

## 2. Reconnaissance and Information Gathering

The first technical stage is understanding the environment before attempting exploitation.

Activities include:

* identifying the target application;
* identifying available entry points;
* observing application functionality;
* examining requests and responses;
* identifying technologies and frameworks;
* identifying parameters and input points;
* mapping application behaviour.

This follows the general principle that security testing should first establish an understanding of the application's attack surface before active testing begins. OWASP's Web Security Testing Guide separates passive information gathering from active testing and emphasizes documenting identified access points and application functionality.

## 3. Attack-Surface Mapping

Once the environment is understood, the tester maps the areas that may require security validation.

Typical areas include:

* authentication;
* authorization;
* session management;
* input handling;
* APIs;
* client-side functionality;
* configuration;
* error handling;
* cryptographic controls;
* business logic.

These areas correspond closely with the categories used by the OWASP Web Security Testing Guide.

The objective is not simply to find a vulnerability, but to understand **where security controls exist, what they are intended to protect, and how they behave under testing**.

## 4. Controlled Vulnerability Testing

After mapping the attack surface, testing moves from observation to controlled validation.

The learner evaluates whether weaknesses can actually be demonstrated within the authorized laboratory.

Examples include testing concepts associated with:

* injection;
* broken access control;
* authentication failures;
* security misconfiguration;
* sensitive-data exposure;
* cross-site scripting;
* insecure components;
* inadequate security logging;
* other application-security weaknesses.

The current OWASP Top 10:2025 provides a contemporary risk framework including Broken Access Control, Security Misconfiguration, Software Supply Chain Failures, Cryptographic Failures, Injection, Insecure Design, Authentication Failures, Software or Data Integrity Failures, Security Logging & Alerting Failures, and Mishandling of Exceptional Conditions.

## 5. Safe Practical Laboratory Model

Practical exercises use isolated or deliberately vulnerable environments.

For example, the manuscript introduces a safe practice target using **OWASP Juice Shop** and demonstrates its deployment within a Kali Linux laboratory.

The laboratory model consists of:

**Kali Linux → Security Tools → Deliberately Vulnerable Application → Controlled Testing → Evidence → Analysis**

The purpose is to give the learner an environment where security concepts can be explored without targeting unauthorized infrastructure.

OWASP officially supports Juice Shop as a security-training and testing environment and provides multiple deployment options, including Docker and local installations.

## 6. Validation of Findings

A suspected weakness is not automatically treated as a confirmed vulnerability.

The tester should:

1. identify the suspected weakness;
2. reproduce the behaviour;
3. determine the affected security control;
4. collect appropriate evidence;
5. determine the potential security impact;
6. avoid unnecessary exploitation;
7. document the result.

This reflects OWASP's emphasis on methodically validating and verifying the effectiveness of application-security controls and documenting identified security issues.

## 7. Documentation and Reporting

Every practical exercise should produce a clear record.

A useful finding structure is:

| Section        | Purpose                                              |
| -------------- | ---------------------------------------------------- |
| Finding        | What security weakness was identified                |
| Location       | Where the weakness exists                            |
| Observation    | What was observed                                    |
| Validation     | How the behaviour was confirmed                      |
| Impact         | What could happen if exploited                       |
| Evidence       | Supporting screenshots, requests, responses, or logs |
| Risk           | Relative significance of the finding                 |
| Recommendation | Appropriate defensive improvement                    |

The objective is to transform technical activity into a professional security finding that another security practitioner can understand and reproduce.

## 8. Defensive Perspective

Offensive cybersecurity is treated as a means of improving security rather than destruction.

The methodology therefore connects every offensive observation to a defensive question:

> **What security control failed, why did it fail, and how can it be strengthened?**

This makes the practical work useful not only for penetration testing but also for vulnerability management, secure development, security awareness, and defensive security operations.

## 9. Continuous Learning Model

The methodology follows a continuous cycle:

**Learn → Observe → Map → Test → Validate → Document → Remediate → Re-test**

Security testing is not presented as a one-time activity. OWASP's testing framework similarly emphasizes security activities across the software lifecycle, including definition and design, development, deployment, maintenance, and operations.

## Ethical Rule of Engagement

All practical activities described in this portfolio are intended for:

* authorized security testing;
* educational laboratories;
* deliberately vulnerable applications;
* controlled research environments;
* defensive security improvement.

Unauthorized access, disruption, data theft, or exploitation of systems without permission is outside the scope of this methodology.

The central principle is simple:

> **Knowledge is powerful. Apply it within authorization, document what you discover, and use the result to strengthen security.**

### Methodology Summary

The methodology can therefore be represented as:

**Authorization → Reconnaissance → Attack-Surface Mapping → Controlled Testing → Validation → Evidence Collection → Risk Analysis → Reporting → Remediation → Re-testing**

This framework provides the foundation for the practical laboratories and offensive-security exercises presented in the portfolio.
