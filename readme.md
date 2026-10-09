# Case Study: Form Spam Attack & Database Recovery (WordPress)

**Site type:** WordPress business website
**Service:** Troubleshooting, database cleanup, spam protection
**By:** Mr.Morningstar

---

## Overview

A WordPress business website stopped delivering contact form emails to the business inbox, which directly hurt lead generation and daily operations. At the same time, the hosting server showed constant 100% CPU load. The cause was a **large-scale, bot-driven form spam attack** that had filled the database with junk entries.

| | |
|---|---|
| **Problem** | Contact form emails not delivered, server stuck at 100% CPU, slow website |
| **Root cause** | Automated bot spam on a public contact form: 200,000+ junk entries in the database |
| **Solution** | Direct MySQL cleanup of spam entries and tables, plus CAPTCHA protection on the form |
| **Result** | Server load normal, emails delivered again, no recurring spam |

---

## The Problem

- Contact form emails were not reaching the business email
- The hosting server showed continuous 100% CPU load
- Website performance dropped significantly

---

## Investigation

### Step 1: Checking the usual suspects
Troubleshooting started with **DNS and email configuration**. Both were confirmed to be working correctly, so the email problem was a symptom, not the cause.

### Step 2: Looking at server load and database growth
To find the root cause faster, AI-assisted analysis was used to review the server overload pattern and the abnormal growth of the database. This pointed toward a **possible automated spam or bot attack**.

### Step 3: Confirming the attack
Further investigation revealed:

- **Over 200,000 spam form entries** stored in the database
- **Repetitive automated content** submitted in foreign-language text
- The attack was limited to **one public-facing frontend form**

---

## Solution

1. Identified form spam as the root cause of the server overload
2. Used AI-assisted guidance to validate a safe cleanup approach before touching live data
3. Ran direct MySQL queries to bulk-delete the spam entries
4. Cleaned the affected database tables
5. Added CAPTCHA protection to the vulnerable form
6. Re-tested form submission and email delivery

---

## Results

- All spam entries removed
- Server load back to normal levels
- Contact form delivering emails again
- Website performance stable
- No repeat spam incidents after the security hardening

---

## Key Takeaways

- **Email not arriving does not always mean an email problem.** Here the real cause was a flooded database and an overloaded server.
- **Constant 100% CPU with normal traffic is a clue.** Check for bots, spam submissions and abnormal database growth.
- **Bulk deletes should be planned.** Use a safe approach, and take a database backup first.
- **Cleanup alone is temporary.** CAPTCHA (or another bot filter) on public forms stops the problem from coming back.

---

## Skills Demonstrated

WordPress troubleshooting, form spam mitigation, MySQL database cleanup, server load analysis, website recovery, AI-assisted debugging, security hardening

---

## Ownership

This issue was handled independently end-to-end, combining technical expertise with AI-assisted analysis for faster diagnosis and resolution.

---
