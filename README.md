# Penetration Test Report – ACME Bookkeeping

## 📋 Executive Summary

This penetration test assessed the security posture of ACME Bookkeeping's IT infrastructure, focusing on vulnerabilities that could potentially lead to unauthorized access or data compromise. The test revealed several critical and high-impact vulnerabilities, including SQL Injection, outdated systems, and weak password policies.

---

## 🛠️ Tools & Techniques Used

- **Nmap**: Scanned the network for open ports and services.
- **Metasploit**: Used for exploitation testing and post-exploitation analysis.
- **Hydra**: Tested password strength by attempting brute-force login.
- **Burp Suite**: Analyzed the web application for security weaknesses.
- **Wireshark**: Captured and analyzed network traffic to find unencrypted data.

---

## 🧪 Findings

### **SQL Injection**  
- **Severity**: Critical  
- **Description**: Exploited a vulnerable endpoint on the web server to bypass login authentication using SQL injection.  
- **Remediation**: Use prepared statements and proper input validation.

### **Outdated System**  
- **Severity**: Critical  
- **Description**: SQL Server 2012 is no longer supported, leaving it vulnerable to known exploits.  
- **Remediation**: Upgrade to a supported version of SQL Server.

### **Insufficient Data Encryption**  
- **Severity**: High  
- **Description**: Sensitive data (such as passwords) was transmitted in plaintext.  
- **Remediation**: Implement HTTPS and encrypt sensitive data in transit and at rest.

### **Weak Password Policy**  
- **Severity**: High  
- **Description**: Weak password policies and no multi-factor authentication.  
- **Remediation**: Enforce stronger password policies and implement multi-factor authentication.

---

## 🧠 Conclusion

The penetration test identified several critical vulnerabilities, including SQL injection and weak password policies. Immediate remediation of these issues will greatly improve ACME Bookkeeping's security posture, protecting both sensitive internal data and customer information.

---

## 📄 Full Report (PDF)

For the full penetration test report, detailing findings, remediation steps, and further recommendations, please download the PDF.

[Penetration Test Project PDF.pdf](https://github.com/user-attachments/files/19912514/Penetration.Test.Project.PDF.pdf)

