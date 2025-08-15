# Intune Policy Documentation –  Audit and Event Logging - v3.1

**Policy Name:** Win - OIB - SC - Device Security - D - Audit and Event Logging - v3.1  
**Platform:** Windows 10  
**Policy Type:** Device Configuration – Endpoint Security / Audit & Event Logging  
**Purpose:** To enforce audit and event logging settings on Windows 10 devices, ensuring comprehensive logging of system, security, application, and account events for security monitoring and compliance purposes.

---

## Policy Overview
This policy configures audit and event logging on Windows 10 devices to capture critical system, security, and application events. It sets log size limits, retention policies, and audit behaviors to ensure that all relevant events are recorded. This policy applies to all managed Windows 10 endpoints in scope, supporting compliance, security monitoring, and forensic investigations.

---

## Configuration Details

| Setting | Configured Value | Purpose / Effect |
|---------|-----------------|-----------------|
| **Control Event Log Behavior** | Enabled | Ensures event logs cannot be overwritten and are properly controlled. |
| **Application Log – Maximum File Size** | 32,768 KB | Ensures application logs retain sufficient history for analysis. |
| **Security Log – Maximum File Size** | 196,608 KB | Captures detailed security events for auditing purposes. |
| **System Log – Maximum File Size** | 32,768 KB | Retains system event history for troubleshooting and security monitoring. |
| **Audit Account Logon – Credential Validation** | Success and Failure | Tracks successful and failed account logons to detect credential misuse. |
| **Audit Account Logon/Logoff – Account Lockout** | Success | Logs account lockouts to identify potential brute-force attacks. |
| **Audit Account Logon/Logoff – Logon** | Success and Failure | Captures all logon attempts for auditing purposes. |
| **Audit Account Management – User Account Management** | Success and Failure | Tracks changes to user accounts to detect unauthorized modifications. |
| **Audit Object Access – File Share** | Success and Failure | Monitors access to shared files to ensure sensitive data is protected. |
| **Audit Privilege Use – Sensitive Privilege Use** | Success and Failure | Detects use of sensitive privileges to identify potential misuse. |
| **Audit Policy Change – Authentication / Authorization / Policy Changes** | Success | Logs all changes to policies for compliance and security tracking. |
| **Audit Detailed Tracking – PnP Activity / Process Creation** | Success | Monitors device changes and process activity for forensic analysis. |
| **Audit System – Security System Extension / IPSec Driver / System Integrity / Security State Change / Other System Events** | Success | Captures system-level events to detect tampering or abnormal behavior. |

*(This table summarizes the main settings; the full policy includes 35 detailed configuration items.)*

---

## Key Security / Operational Benefits
- **Comprehensive Logging:** Ensures all critical events are captured for auditing and forensic purposes.  
- **Enhanced Security Monitoring:** Provides visibility into account activity, system changes, and privilege use.  
- **Compliance Support:** Helps meet regulatory and internal compliance requirements for event logging.  
- **Operational Insights:** Enables IT teams to troubleshoot and analyze system and application events effectively.

---

## Client Impact
- **End Users:** Minimal impact; primarily background logging, with no changes to day-to-day operations.  
- **IT Administration:** Requires monitoring of log sizes and retention; ensures logs are collected and retained for compliance.  
- **Maintenance:** Periodic review of audit logs and storage utilization to ensure continued compliance and system performance.
