# Part 1 — Suspicious Message Report Form

**Project:** Home SOC (Security Operations Centre)

**Status:** Live

**Live Form:** [Click here to report a suspicious message](https://j-dog22-cmd.github.io/suspicious-report-form)

---

## Overview

This is the first component of my Home SOC project. The goal is to create a simple way for family and friends to report suspicious messages, emails and links directly to me for analysis — rather than ignoring them or accidentally clicking them.

This form acts as the **first line of defence and intelligence gathering** for my home network security pipeline.

---

## The Problem

Non-technical people receive phishing messages and either:

- Click the link without thinking
- Ignore it and move on
- Don't know who to report it to

This form gives them a simple, accessible way to flag anything suspicious directly to me.

---

## How It Works

```
Family/friend receives suspicious message
              ↓
They visit the form and submit:
  - Their name and email
  - The message type (SMS / Email / Other)
  - The suspicious link
  - The full message text
  - A screenshot (optional)
  - Any additional notes
              ↓
I receive an email notification instantly
              ↓
I analyse the submission safely in a sandbox
              ↓
Confirmed malicious → added to Pi-hole blocklist
              ↓
Entire home network protected
```

---

## What Was Used To Build It

| Tool | Purpose |
| --- | --- |
| HTML / CSS / JavaScript | Front end form |
| EmailJS | Email notifications on submission |
| GitHub Pages | Free hosting |

---

## Features

- Clean, simple interface anyone can use
- Accepts suspicious links, message text and screenshots
- Instant email notification on submission
- Mobile friendly
- No personal data stored — submissions go straight to email

---

## Why I Built This

After analysing a real world DPD phishing SMS (see my [threat analysis report](https://github.com/j-dog22-cmd/Security_Portfolio/tree/7ae79d44b8bca6dd5c1fd13eca538bfa545615af/threat-analysis/DPD_URL)), I wanted to create a practical tool that would help protect people around me from similar attacks.

Rather than just documenting threats after the fact, this form allows me to intercept suspicious content before anyone clicks, analyse it safely and use the findings to protect my home network.

---

## Part of a Larger Pipeline

This form is Part 1 of my Home SOC project:

| Part | Description | Status |
| --- | --- | --- |
| 01 - Report Form | Suspicious message submission form | ✅ Complete |
| 02 - Pi-hole Setup | DNS level blocking on home network | 🔄 Coming soon |
| 03 - Blocklist Management | Adding confirmed malicious domains to Pi-hole | 🔄 Coming soon |

---

*Built as part of independent security research. All submissions are reviewed manually and handled responsibly.*
