# Phishing Email Forensic Analysis Report  
**Subject:** Amazon Order Cancellation Scam  
**Analysis Date:** [Insert Date]  

---

## **📌 Executive Summary**  
This report analyzes a simulated phishing email impersonating Amazon to:  
- Identify common social engineering tactics  
- Document technical indicators of compromise  
- Provide detection recommendations  

**Severity:** High (Credential Theft Risk)  

---

## **🔍 Technical Analysis**  

### **1. Email Header Analysis**  
| Field | Value | Red Flag |  
|-------|-------|----------|  
| From | `Amazon Head Office <contact@usps.com>` | Domain mismatch (USPS ≠ Amazon) |  
| Received | [Simulated] 3:13 AM EST | Unusual send time |  

### **2. Content Analysis**  
**Deceptive Elements Found:**  
- ❗ "Urgent: Your account has been suspended"  
- 🔗 **Masked URL:**  
  ```diff
  - Displayed: amazon.com/verify-my-account
  + Actual: http://phishing-site-example.com/amazon-verify-account
