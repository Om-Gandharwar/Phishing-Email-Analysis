**# Phishing Email Investigation Project -**

**##Project Overview -**

This project demonstrates a complete Phishing Email Investigation using the workflow of an L1 SOC Analyst.
The goal is to analyze a suspicious email’s metadata, authentication results, links, sender reputation, and overall risk to understand whether it is malicious. 

**# Objectives**

Understand how attackers use phishing to target users.
Learn how L1 SOC analysts investigate suspicious emails.
Analyze real email headers (SPF, DKIM, DMARC).
Inspect sender infrastructure, URLs, and artifacts safely.
Document a clean investigation report.

**# Investigation Workflows - **

**# 1. Email Header Check**

Extract and review the email header to verify:

Sender domain

Mail server path (Received chain)

SPF, DKIM, DMARC authentication results

**# 2. Link & URL Inspection**

Without clicking:

Hover over URLs

Extract them safely

Analyze using tools like VirusTotal, URLScan, ANY.RUN

Check if the domain is suspicious, newly registered, or impersonating a brand

**# 3. Attachment Analysis**

If an attachment exists:

Upload to sandbox (ANY.RUN, Joe Sandbox)

Identify malware behavior (script execution, outbound connections)

**# 4. Sender Reputation Check**

Use tools to validate:

Domain age

WHOIS information

Blacklist status

Email service provider used

**# 5. User Impact Assessment**

Confirm whether the user:

Clicked the link

Entered credentials

Downloaded anything

**# 6. Take Action**

Depending on findings:

Block malicious domain/IP/URL

Quarantine emails in the environment

Force password reset if needed

Update SIEM with indicators (IOCs)

**# 7. Document & Report**

Create a short incident note:

What was found

Evidence (headers, URLs, sandbox results)

Steps taken

Recommendations for the user

**# Tools Used**

MXToolbox – SPF, DKIM, DMARC verification

VirusTotal – URL and domain analysis

URLScan.io – Website screenshot + behavior

WHOIS / DomainTools – Domain age and ownership

Header Analyzer – Visual interpretation of email headers

ANY.RUN – Sandbox (if attachments exist)

**# About This Project**

This project is part of my cybersecurity learning journey.
It reflects my ability to:

Think like a SOC Analyst

Perform structured investigations

Document findings clearly

Use industry tools

Analyze threats safely

**# Feedback Welcome**

If you're a SOC professional or cybersecurity practitioner, your feedback would be valuable.
Feel free to open an issue or share suggestions.
