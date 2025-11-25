# Junior Security Analyst Intro

## Task 1: Which team do you work with as a Junior Security Analyst?

**Answer:**  
You work with the **SOC**, which is short for **Security Operations Center**.

---

## Task 3:

### Q1: Click on the green "View Site" button in this task and open the lab.

Just open the site — no answer needed.

---

### Q2: What was the malicious IP address in the alerts?

In the first tab called **SIEM Dashboard**, some alerts appear:

- **Nov 25th 2025 at 20:22 — Critical**  
  Successful SSH login from the suspicious IP address **221.181.185.159**

- **Nov 25th 2025 at 20:18 — Critical**  
  Unauthorized login attempts from IP address **221.181.185.159** to port 22

The first column shows the **date**,  
the second shows the **severity**,  
and the third explains what the attacker (or even a normal user) tried to do, including the IP and the port targeted.

This alert is suspicious, so we need to check if this IP is related to any other attack using the **IP Hunter** tab.

**Result from IP Hunter:**  
**221.181.185.159 was found in our database!**  
**Malicious — Involved in 4 Cyber Attacks**

So now we know that this IP is a threat to our system.

We escalate the problem to the SOC Team Leader.

After getting permission, we block the IP in our firewall.

---

### Q2: What was the malicious IP address in the alerts?

**Answer:** **221.181.185.159**

---

### Q3: To whom did you escalate t
