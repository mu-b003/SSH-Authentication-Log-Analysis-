# SSH Authentication Log Analysis

A beginner SOC investigation project focused on analyzing SSH authentication logs after generating login attempts in a controlled lab environment.

## Overview

This project demonstrates how to investigate SSH authentication events by reviewing Linux authentication logs (`/var/log/auth.log`).

The objective was to identify:
- Failed login attempts
- Successful logins
- Targeted user accounts
- Source IP address
- SSH authentication events

## Lab Environment

- VMware Workstation
- Ubuntu 24.04 LTS (Target)
- Kali Linux (Testing Machine)
- OpenSSH Server

## Scenario

Several SSH login attempts were generated from a Kali Linux machine against an Ubuntu system.

The investigation included:
- Invalid username attempt
- Failed password attempts
- Successful authentication
- Log analysis using Linux command-line tools

## Tools Used

- grep
- systemctl
- ip
- ssh
- Hydra (Lab Environment Only)

## Key Findings

- Source IP identified
- Invalid user login detected
- Multiple failed authentication attempts observed
- Successful SSH login identified
- No SSH activity targeting the root account

## Skills Practiced

- Linux Log Analysis
- SSH Authentication Investigation
- Incident Investigation
- Command Line Log Parsing
- Basic SOC Analysis

## Project Structure

```
SSH-Authentication-Log-Analysis/
│
├── README.md
├── REPORT.md
├── COMMANDS.md
├── EVIDENCE/
├── LICENSE
└── DISCLAIMER.md
```

## Disclaimer

All activities were performed in an isolated personal lab for educational purposes only.
