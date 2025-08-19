# Intune Compliance Policy Documentation – Device Security Compliance Policy - v3.1

**Policy Name:** Win - OIB - Compliance - U - Device Security - v3.1  
**Platform:** Windows 10 and later  
**Policy Type:** Device Compliance Policy  
**Purpose:** Ensures that Windows devices meet essential security compliance requirements such as password strength, encryption, and antimalware protection before they are allowed access to corporate resources.

---

## Policy Overview
This compliance policy enforces baseline device security standards for Windows 10 and later devices. It validates that security features such as BitLocker, antivirus, antispyware, and firewall are enabled. It also enforces password requirements and device lockout policies to reduce the risk of unauthorized access. Devices that fail to meet these requirements will be marked non-compliant and may be blocked from accessing organizational resources.

---

## Configuration Details

| Setting | Configured Value | Purpose / Effect |
|---------|------------------|------------------|
| **Password Required** | True | Ensures devices must have a password set. |
| **Password Minimum Length** | 8 | Enforces a minimum password length of 8 characters. |
| **Password Block Simple** | True | Prevents users from using simple passwords (e.g., "1234"). |
| **Password Required Type** | Device Default | Uses the device’s default password type policy. |
| **Password Inactivity Lock (minutes)** | 5 | Locks device after 5 minutes of inactivity. |
| **Password Required to Unlock from Idle** | True | Requires password entry when waking from idle state. |
| **Active Firewall Required** | True | Ensures Windows Firewall is enabled. |
| **Antivirus Required** | True | Requires antivirus software to be active. |
| **Antispyware Required** | True | Requires antispyware protection to be active. |
| **BitLocker Enabled** | True | Requires BitLocker drive encryption to be enabled. |
| **TPM Required** | True | Requires Trusted Platform Module for security operations. |

---

## Key Security / Operational Benefits
- **Protects corporate resources** by ensuring only secure and compliant devices gain access.  
- **Improves password security** with minimum length, inactivity lock, and complexity requirements.  
- **Reduces malware risk** by requiring antivirus and antispyware.  
- **Ensures data protection** by enforcing BitLocker and TPM presence.  
- **Maintains firewall security** to prevent unauthorized inbound/outbound traffic.  

---

## Client Impact
- **End Users:** Must set strong passwords, use BitLocker, and keep security protections enabled (antivirus, antispyware, firewall).  
- **IT Admins:** Non-compliant devices will be flagged in Intune and can trigger Conditional Access restrictions.  
- **Ongoing Monitoring:** Admins must monitor compliance reports and remediate devices failing encryption or password requirements.  
