# Intune Policy Documentation - OneDrive User Configuration - v3.0

**Policy Name:** Win - OIB - SC - Microsoft OneDrive - U - Configuration - v3.0  
**Platform:** Windows 10  
**Policy Type:** Device Configuration – OneDrive User Settings  
**Purpose:** To configure OneDrive user experience on Windows 10 devices, controlling file handling, tutorial prompts, root folder restrictions, and personal sync to maintain organizational compliance and prevent data leakage.

---

## Policy Overview
This policy enforces OneDrive user configuration settings for Windows 10 devices. It ensures that users cannot override organizational restrictions, disables unnecessary tutorials, enforces specific folder roots, and prevents personal OneDrive accounts from syncing. These controls maintain a secure and standardized OneDrive experience across the enterprise.

---

## Configuration Details

| Setting | Configured Value | Purpose / Effect |
|---------|-----------------|-----------------|
| **Enable Hold The File** | Enabled | Ensures that files are temporarily held before syncing, providing better control over file operations. |
| **Disable First Run Experience Tutorial** | Enabled | Prevents the OneDrive first-run tutorial from appearing to users. |
| **Disable Custom Root** | Enabled – `%OrganizationId%` set as enforced root | Restricts users from selecting a custom root folder; OneDrive is configured to use the organization-approved folder path. |
| **Disable Personal Sync** | Enabled | Prevents users from syncing personal OneDrive accounts, ensuring only corporate accounts are used. |

---

## Key Security / Operational Benefits
- **Controlled File Sync:** Users cannot bypass organizational folder structure, reducing risk of data being stored outside approved locations.  
- **Consistent User Experience:** First-run tutorials and custom folder options are disabled for all users, creating a uniform setup.  
- **Data Security:** Personal OneDrive accounts are blocked, preventing potential leakage of corporate data.  
- **Reduced Support Requests:** Simplified setup reduces user errors and IT support overhead.

---

## Client Impact
- **End Users:** OneDrive setup is preconfigured; some customization options are restricted.  
- **IT Administration:** Simplifies enforcement of organizational policies and compliance tracking.  
- **Maintenance:** Periodic review of the enforced root and personal sync restrictions may be necessary as organizational structure evolves.
