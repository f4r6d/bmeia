# Analysis of Security Vulnerabilities in the BMEIA Appointment System (Tehran Case Study)

## ⚠️ Disclaimer & Ethical Statement
This project is created for **educational and reporting purposes only**. Its primary goal is to demonstrate the technical vulnerabilities and the lack of bot-protection mechanisms in the official appointment system of the Austrian Federal Ministry for European and International Affairs (BMEIA).

**Important Note:**
- This website/code **does not** book actual appointments.
- This project is **not** for sale.
- I strongly condemn the use of automated scripts for financial gain or to create an unfair advantage for applicants.
- As a professional developer, I have chosen to report these vulnerabilities rather than exploit them.

---

## 🧐 The Problem Statement
The current appointment system for the Austrian Embassy in Tehran (located at `appointment.bmeia.gv.at`) is currently being exploited by scalpers and black-market intermediaries. 

Due to the absence of advanced bot-mitigation tools (such as behavioral analysis, modern CAPTCHAs, or rate-limiting), automated scripts are able to:
1.  Monitor the website 24/7 with millisecond precision.
2.  Bypass simple form validations.
3.  Exhaust all available slots before a human user can even load the page.

## 🛠 Technical Analysis (Vulnerability Proof of Concept)
This repository demonstrates how easily the system can be interfaced with automated tools. 

### Key Vulnerabilities Identified:
* **Predictable Endpoints:** Lack of obfuscation in the API calls for checking slot availability.
* **Weak Bot Detection:** No integration of modern challenges like Cloudflare Turnstile or reCAPTCHA v3.
* **Static Form Submission:** The form structure allows for easy payload injection via scripts without session-based integrity checks.

## 🎯 The Goal of this Project
The goal is to urge the **IT department of the Austrian Foreign Ministry (BMEIA)** and the **Austrian Embassy in Tehran** to:
1.  Acknowledge the existence of bot interference.
2.  Implement a more secure, "human-first" booking process.
3.  Protect the rights of honest applicants who are being extorted by black-market dealers.

## ✉️ Contact
If you represent the BMEIA or the Austrian Embassy and wish to discuss these findings or seek technical advice on how to mitigate these bots, please feel free to reach out to me.

**Author:** Farshid Gholizadeh
