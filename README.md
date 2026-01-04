# phishing-analysis-fundamentals

# Phishing Analysis Writeup

## Exercise 1: Phishing Analysis Fundamentals (TryHackMe)

### Target Machine Information
- Title: Phishing Emails 1 v2.2-badr
- Target IP Address: 10.48.175.211

### Introduction
This exercise focuses on understanding how phishing emails work and how security analysts analyze email headers and email content to determine whether an email is malicious or benign.

### Understanding Phishing and Email Basics
Phishing is a type of social engineering attack that uses emails to trick users into revealing sensitive information.

An email address consists of three parts:
- User mailbox
- @ symbol
- Domain name

Email technology was first introduced in the 1970s.

### Email Delivery Protocols
Emails are sent and received using several protocols:

- SMTP: Used to send emails
- POP3: Downloads emails to one device
- IMAP: Stores emails on the server and allows access from multiple devices

Secure ports used:
- SMTP (STARTTLS): 587
- IMAP (Secure): 993
- POP3 (Secure): 995

### Email Header Analysis
Email headers contain important information used to analyze suspicious emails.

Important email header fields:
- From: Sender email address
- To: Recipient email address
- Subject: Email subject
- Date: Time email was sent
- Reply-To: Address used when replying

The email header field that functions the same as "Reply-To" is:
- Return-Path

After identifying the sender’s IP address, additional information can be retrieved using:
- ARIN (American Registry for Internet Numbers)

### Email Body and Attachments
The email body may be written in plain text or HTML format.

HTML emails may include:
- Images
- Embedded links
- Attachments

From the analysis:
- Blocked image URI: https://i.imgur.com/LSWOtDI.png
- PDF attachment name: Payment-updateid.pdf
- Decoded PDF content: THM{BENIGN_PDF_ATTACHMENT}

### Types of Phishing
Different phishing techniques include:
- Spam
- Phishing
- Spear phishing
- Whaling
- Smishing
- Vishing

### Phishing Email Case Analysis
From the analyzed email (email3.eml):

- Masqueraded trusted entity: Home Depot
- Sender email: support@teckbe.com
- Subject line: Order Placed : Your Order ID OD2321657089291 Placed Successfully
- Malicious URL (defanged): hxxp[://]t[.]teckbe[.]com

### Conclusion
Through this exercise, I learned how phishing emails are structured and how to analyze email headers, email bodies, and attachments. This knowledge is important for identifying phishing attacks and preventing security incidents.

Business Email Compromise (BEC) refers to attacks where an attacker gains access to a legitimate business email account to perform fraudulent activities.
