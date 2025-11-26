Email Sender With Attachments (Python)

This project is a Python-based email automation script that allows you to send emails using Gmail SMTP with support for file attachments such as PDFs, images, documents, ZIP files, and more.
It uses secure SMTP (SSL) along with Gmail App Password authentication to ensure safe email delivery.

Features
✔ Send Emails Programmatically

Send any email using your Gmail account with a subject and message body.

✔ Attachment Support

Attach any file type including:

PDF documents

JPG/PNG images

TXT files

ZIP/RAR archives

Any binary file

✔ MIME Auto-Detection

Automatically detects correct MIME type (file format) so attachments open properly.

✔ Secure Login

Uses:

Gmail SMTP server

SSL encryption

App Password authentication

✔ Error Handling

Catches:

Invalid credential errors

Missing file errors

Connection issues

Technologies Used

Python

smtplib (SMTP handling)

ssl (secure connection)

email.message (email formatting)

mimetypes (file type detection)

How to Use
1. Enable Gmail App Password

Generate an App Password from your Google Account.

2. Store Credentials as Environment Variables

Windows:

setx GMAIL_ADDRESS "yourgmail@gmail.com"
setx GMAIL_APP_PASSWORD "your_app_password"

3. Run the Script
python send_email.py

Code Overview

The script includes:

A send_email_with_attachment() function

SMTP SSL connection

Optional attachment parameter

Automatic MIME detection

Full email construction with headers
