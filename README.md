## Exercise 1: Phishing Analysis Fundamentals (TryHackMe)

### Introduction
This exercise introduces the fundamentals of phishing attacks and how security analysts analyze emails to determine whether they are malicious or harmless.

---

### Email and Phishing Basics
Phishing is a social engineering attack that uses emails to trick users into revealing sensitive information or downloading malicious files.

An email address consists of:
- User mailbox
- @ symbol
- Domain name

Email technology was first introduced in the 1970s.

---

### Email Delivery Protocols
Emails are sent and received using the following protocols:
- SMTP: Used to send emails
- POP3: Downloads emails to a single device
- IMAP: Stores emails on the server and allows access from multiple devices

Secure ports used:
- SMTP (STARTTLS): 587
- IMAP (Secure): 993
- POP3 (Secure): 995

---

### Email Header Analysis
Email headers contain important information for phishing analysis.

Important header fields:
- From
- To
- Subject
- Date
- Reply-To

The email header that functions the same as "Reply-To" is:
- Return-Path

After identifying the sender’s IP address, more information can be retrieved using:
- ARIN (American Registry for Internet Numbers)

---

### Email Body and Attachments
The email body can be in plain text or HTML format and may include images, links, or attachments.

From the analysis:
- Blocked image URI: https://i.imgur.com/LSWOtDI.png
- PDF attachment name: Payment-updateid.pdf
- Decoded PDF content: THM{BENIGN_PDF_ATTACHMENT}

---

### Types of Phishing
Common types of phishing include:
- Spam
- Phishing
- Spear phishing
- Whaling
- Smishing
- Vishing

---

### Phishing Email Case Analysis
Based on the analyzed email sample:
- Masqueraded trusted entity: Home Depot
- Sender email: support@teckbe.com
- Subject line: Order Placed : Your Order ID OD2321657089291 Placed Successfully
- Malicious URL (defanged): hxxp[://]t[.]teckbe[.]com

---

### Conclusion
This exercise helped me understand how emails work and how phishing attacks are identified through email headers, email content, and attachments.

Business Email Compromise (BEC) refers to attacks where attackers gain access to a legitimate business email account to perform fraudulent activities.
