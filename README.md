# Web Application Penetration Testing

 A structured security assessment focused on evaluating web application controls, identifying vulnerabilities that may expose sensitive information, and providing actionable recommendations to strengthen security.

## 🎯 Project Overview

| | |
|---|---|
| **Project** | Web Application Penetration Testing |
| **Program** | Networkwalks Internship |
| **Assessment type** | Black-box web application assessment |
| **Authorization** | The original report states that written permission was granted for the project |
| **Researcher** | [Your Name] |

This assessment examined how exposed files, weak access controls, and weak document passwords could put sensitive information at risk. The report describes access to confidential documents and a database backup containing employee and shareholder information.

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| Kali Linux | Assessment environment |
| Firefox | Manual application review |
| Burp Suite | HTTP traffic inspection |
| WhatWeb | Web technology fingerprinting |
| ffuf | Directory and file discovery |
| wget | Retrieving accessible files |
| pdf2john | Extracting password hashes from encrypted PDFs |
| John the Ripper | Auditing PDF password strength |

## 🔍 Findings

### 1. Exposed Backup and Directory Listing

**Severity: Critical**

The report describes a publicly accessible directory that exposed a database backup and restricted documents.

**Potential impact:**

- Unauthorized access to sensitive organizational information
- Exposure of employee and shareholder records
- Reputational, legal, and privacy consequences

### 2. Unprotected Confidential Documents

**Severity: High**

The report states that confidential documents could be accessed without appropriate authentication.

**Potential impact:**

- Unauthorized disclosure of private records
- Loss of confidentiality for affected individuals
- Possible breach of applicable privacy obligations

### 3. Weak PDF Passwords

**Severity: Medium**

The report describes encrypted PDFs protected by weak passwords that were recovered through dictionary-based password testing.

**Potential impact:**

- Unauthorized access to documents if encrypted files are obtained
- Reduced protection for sensitive information

## ⚙️ Methodology Summary

The original report describes a black-box assessment that included:

1. Reviewing publicly available application information.
2. Checking for exposed directories and files.
3. Assessing access controls around confidential documents.
4. Evaluating the password strength of encrypted PDFs.
5. Reviewing the exposed backup for categories of sensitive information.
6. Documenting risks and recommending remediation.

Target-specific URLs, paths, filenames, recovered passwords, and evidence screenshots are omitted from this public summary.

## 📊 Risk Summary

| Finding | Severity |
|---|---|
| Exposed backup and directory listing | Critical |
| Unprotected confidential documents | High |
| Weak PDF passwords | Medium |

## 🛡️ Recommended Remediation

- Disable directory indexing on web servers.
- Keep database backups outside publicly served directories.
- Require server-side authentication and authorization for confidential documents.
- Use strong, unique passwords and modern encryption for protected files.
- Avoid relying on `robots.txt` to protect sensitive resources.
- Review public-facing storage and configurations for unintended exposure.
- Assess any potential exposure of personal information and follow applicable incident-response requirements.

## 📚 Key Learning Outcomes

This project provided experience with:

- Web application reconnaissance and security assessment
- Identifying exposed files and access control weaknesses
- Evaluating password protection for encrypted documents
- Assessing potential privacy and organizational impact
- Communicating findings with practical remediation guidance

## ⚠️ Disclaimer

This README summarizes an educational project report. The reported findings, authorization, and impact have not been independently verified. Security testing should only be performed with explicit written authorization and within the approved scope.

This public summary excludes target identifiers, credentials, personal records, and raw evidence to reduce the risk of disclosure.

## 👨‍💻 Author

[Your Name]

**Project:** Networkwalks Week 4 Penetration Testing
