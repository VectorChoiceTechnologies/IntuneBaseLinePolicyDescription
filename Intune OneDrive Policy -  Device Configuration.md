# Intune Policy Documentation -  Device Configuration - v3.2

**Policy Name:** Win - OIB - SC - Microsoft OneDrive - D - Configuration - v3.2  
**Platform:** Windows 10  
**Policy Type:** Device Configuration – OneDrive Settings  
**Purpose:** To configure OneDrive for enterprise deployment, controlling tenant access, sync behavior, bandwidth management, silent account setup, and file handling to ensure security, compliance, and optimal performance.

---

## Policy Overview
This policy manages OneDrive behavior on Windows 10 devices in a corporate environment. It restricts access to approved tenants, controls file synchronization and upload bandwidth, enables silent account configuration, and applies file type exclusions. The policy ensures consistent OneDrive setup for all users while enforcing organizational security and operational standards.

---

## Configuration Details

| Setting | Configured Value | Purpose / Effect |
|---------|-----------------|-----------------|
| **Allow Tenant List** | Enabled – `%OrganizationId%` | Restricts OneDrive accounts to the specified organizational tenant(s) only. |
| **Enable Feedback and Support** | Disabled | Users cannot send feedback or access support from OneDrive. |
| **Enable Automatic Upload Bandwidth Management** | Enabled | Automatically adjusts upload speeds to optimize network performance. |
| **Enable Sync Admin Reports** | Enabled | Generates reports on OneDrive sync activity for administrators. |
| **Enable OD Ignore List from GPO** | Enabled – Excluded file types: `*.accdb, *.appx, *.bat, *.cmd, *.exe, *.img, *.iso, *.jar, *.lnk, *.mdb, *.msi, *.pst, *.reg, *.vbs, *.vhd, *.vhdx, *.vmdk` | Prevents specific file types from syncing to OneDrive to reduce risk and storage issues. |
| **KFM Block Opt-Out** | Enabled | Users cannot opt out of Known Folder Move (KFM). |
| **GPO Setup Ring** | Enabled – Ring 5 | Controls the OneDrive setup experience via group policy ring. |
| **KFM Opt-In Wizard** | Enabled – Desktop, Documents, Pictures; Auto-select organization `%OrganizationId%` | Provides an interactive wizard for users to opt into KFM with preconfigured folders and organization information. |
| **Silent Account Configuration** | Enabled | OneDrive account is configured silently without user interaction. |
| **Files On-Demand Enabled** | Enabled | Files are available on-demand locally but stored in the cloud to save disk space. |

---

## Key Security / Operational Benefits
- **Tenant Restriction:** Prevents unauthorized OneDrive accounts, protecting organizational data.  
- **Bandwidth Optimization:** Reduces network congestion during large file uploads.  
- **Controlled Sync:** Excluded file types and KFM enforcement prevent accidental data loss or storage of inappropriate files.  
- **Automated Setup:** Silent account configuration reduces support requests and ensures uniform deployment.  
- **Administrator Visibility:** Sync reports allow IT teams to monitor activity and troubleshoot issues proactively.

---

## Client Impact
- **End Users:** OneDrive is preconfigured and partially restricted; some manual setup options are removed.  
- **IT Administration:** Simplifies deployment and compliance tracking for OneDrive across all managed devices.  
- **Maintenance:** Periodic review of file exclusions, tenant list, and KFM settings is recommended to adapt to organizational changes.
