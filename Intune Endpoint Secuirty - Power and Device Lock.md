# Intune Policy Documentation – Power and Device Lock - v3.6

**Policy Name:** Win - OIB - SC - Device Security - U - Power and Device Lock - v3.6  
**Platform:** Windows 10  
**Policy Type:** Device Configuration – Endpoint Security / Power & Device Lock  
**Purpose:** To enforce secure device wake, sleep, and display timeout settings, ensuring devices require authentication after sleep and follow power management best practices to protect data and improve energy efficiency.

---

## Policy Overview
This policy configures power management and device lock settings on Windows 10 endpoints. It enforces password requirements when devices wake from sleep, sets timeouts for standby and display off events, and defines unattended sleep behavior for battery and AC power states. These settings apply to all managed Windows 10 devices, helping secure unattended devices and reduce the risk of unauthorized access.

---

## Configuration Details

| Setting | Configured Value | Purpose / Effect |
|---------|-----------------|-----------------|
| **Require password on wake (battery)** | Enabled | Ensures users must authenticate when the device wakes from sleep on battery power. |
| **Require password on wake (plugged in)** | Enabled | Requires authentication when waking from sleep while plugged in. |
| **Standby timeout (battery)** | 600 seconds (10 min) | Automatically puts the device into standby after 10 minutes on battery to save power. |
| **Standby timeout (plugged in)** | 900 seconds (15 min) | Automatically puts the device into standby after 15 minutes when plugged in. |
| **Display off timeout (battery)** | 300 seconds (5 min) | Turns off the display after 5 minutes on battery to reduce power usage. |
| **Display off timeout (plugged in)** | 600 seconds (10 min) | Turns off the display after 10 minutes when plugged in. |
| **Unattended sleep timeout (battery)** | 600 seconds (10 min) | Puts the device into sleep automatically after 10 minutes of inactivity on battery. |
| **Unattended sleep timeout (plugged in)** | 900 seconds (15 min) | Puts the device into sleep automatically after 15 minutes of inactivity when plugged in. |

---

## Key Security / Operational Benefits
- **Device Security:** Reduces risk of unauthorized access by requiring authentication on wake.  
- **Energy Efficiency:** Optimizes power usage with automated standby and display off timeouts.  
- **User Compliance:** Encourages secure handling of devices by enforcing consistent lock and sleep behavior.  
- **Operational Consistency:** Ensures all endpoints follow standardized power management settings.

---

## Client Impact
- **End Users:** Devices will automatically sleep or turn off the display after defined periods; users must enter a password to resume.  
- **IT Administration:** Minimal management required; ensures secure device wake and energy-efficient settings across endpoints.  
- **Maintenance:** Periodic review of device compliance with power and lock policies; adjustments may be needed based on organizational workflow changes.
