# SSH Authentication Investigation Report

## Objective

Investigate SSH authentication events generated during a controlled security lab exercise.

---

## Environment

Target Machine:
- Ubuntu 24.04 LTS

Attack Simulation Machine:
- Kali Linux

Service:
- OpenSSH

---

## Investigation Summary

The SSH authentication logs were reviewed to identify authentication activity and determine whether unauthorized access occurred.

---

## Timeline

### Event 1

An SSH login attempt was made using an invalid username.

Result:
- Authentication failed.

---

### Event 2

Multiple login attempts were made against an existing user account using incorrect passwords.

Result:
- Authentication failed.

---

### Event 3

A successful SSH login was observed for the user account:

- IT-support

Result:
- Authentication successful.

---

## Indicators

### Source IP

192.168.150.128

### Target System

192.168.150.129

### Service

SSH (Port 22)

### Targeted Accounts

- admin
- barakuser
- IT-support

---

## Findings

- Invalid username authentication attempts were detected.
- Multiple failed password attempts were recorded.
- One successful SSH authentication was identified.
- No evidence of attacks targeting the root account.
- All events originated from the same source IP.

---

## Conclusion

The investigation successfully identified both failed and successful SSH authentication events.

No authentication attempts targeting the root account were found.

This exercise demonstrates the basic process of reviewing Linux authentication logs and extracting security-relevant information for SOC investigations.
