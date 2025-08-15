# Intune Baseline Policy Documentation

This repository contains documentation for all baseline Intune policies applied across managed Intune Environments.  
Each document explains the purpose, configuration, and impact of the policy for easy reference by clients and internal teams.

---

## 📂 Policy Index

### Required Polices
| Policy Name | Platform | Type | Purpose |
|-------------|----------|------|------|
| **[Win - OIB - ES - Encryption - D - BitLocker (OS Disk) - v3.0](https://github.com/VectorChoiceTechnologies/IntuneBaseLinePolicyDescription/blob/main/Intune%20Endpoint%20Security%20%E2%80%93%20BitLocker%20Policy.md#intune-endpoint-security--bitlocker-policy)** | Windows 10 and later | Endpoint Security – Disk Encryption (BitLocker) | Enforces encryption settings for the Operating System (OS) drive to protect data in case of device loss or theft.|
| **[Win - OIB - SC - Device Security - D - Audit and Event Logging - v3.1](https://github.com/VectorChoiceTechnologies/IntuneBaseLinePolicyDescription/blob/main/Intune%20Endpoint%20Security%20-%20Audit%20and%20Event%20Logging.md#intune-policy-documentation---audit-and-event-logging---v31)** | Windows 10 and later | Endpoint Security – Audit and Event Logging | To enforce audit and event logging settings on Windows 10 devices, ensuring comprehensive logging of system, security, application, and account events for security monitoring and compliance purposes. |
| **[Win - OIB - SC - Device Security - U - Power and Device Lock - v3.6](https://github.com/VectorChoiceTechnologies/IntuneBaseLinePolicyDescription/blob/main/Intune%20Endpoint%20Secuirty%20-%20Power%20and%20Device%20Lock.md#intune-policy-documentation--power-and-device-lock---v36)** | Windows 10 and later | Endpoint Security - Power and Device Lock | To enforce secure device wake, sleep, and display timeout settings, ensuring devices require authentication after sleep and follow power management best practices to protect data and improve energy efficiency. |
| **[Win - OIB - SC - Microsoft OneDrive - D - Configuration - v3.2](https://github.com/VectorChoiceTechnologies/IntuneBaseLinePolicyDescription/blob/main/Intune%20OneDrive%20Policy%20-%20%20Device%20Configuration.md#intune-policy-documentation----device-configuration---v32)** | Windows 10 and later | OneDrive Configuration - Device | To configure OneDrive for enterprise deployment, controlling tenant access, sync behavior, bandwidth management, silent account setup, and file handling to ensure security, compliance, and optimal performance. |

### Optional Polices
| Policy Name | Platform | Type | Purpose |
|-------------|----------|------|------|
| **[Win - OIB - SC - Microsoft Edge - U - Profiles, Sign-In and Sync - v3.0](https://github.com/VectorChoiceTechnologies/IntuneBaseLinePolicyDescription/blob/main/Intune%20Edge%20Policy%20-%20Profiles,%20Sign-In%20and%20Sync.md#intune-policy-documentation--edge-settings---profiles-sign-in-and-sync---v30)** | Windows 10 and later | Microsoft Edge Settings - Profiles, Sign-In, and Sync | To manage user profiles, sign-in behavior, and sync functionality in Microsoft Edge, ensuring secure, consistent browser configurations and controlled user experience.|
---

## 📌 How to Use This Documentation
1. **Find the policy** in the table above.
2. Click **Policy Name** to open its detailed documentation.
3. Review the **Configuration Details** and **Client Impact** to understand how it affects devices.

---

_Last Updated: {{date}}_
