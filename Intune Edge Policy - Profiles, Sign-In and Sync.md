# Intune Policy Documentation – Win - OIB - SC - Microsoft Edge - U - Profiles, Sign-In and Sync - v3.0

**Policy Name:** Win - OIB - SC - Microsoft Edge - U - Profiles, Sign-In and Sync - v3.0  
**Platform:** Windows 10  
**Policy Type:** Device Configuration – Microsoft Edge Settings  
**Purpose:** To manage user profiles, sign-in behavior, and sync functionality in Microsoft Edge, ensuring secure, consistent browser configurations and controlled user experience.

---

## Policy Overview
This policy controls Microsoft Edge profile creation, sign-in behavior, and synchronization on Windows 10 endpoints. It prevents automatic import of data at first run, restricts profile additions, controls ephemeral profile usage, and enforces sign-in and sync behaviors. The policy applies to all managed Windows 10 devices to maintain security, user consistency, and compliance with organizational standards.

---

## Configuration Details

| Setting | Configured Value | Purpose / Effect |
|---------|-----------------|-----------------|
| **Auto-import at first run** | Disabled | Prevents automatic import of settings, favorites, and passwords when Edge is first launched. |
| **Browser sign-in** | Enabled | Allows users to sign in to Edge with their Microsoft account for access to work or school data. |
| **Non-removable profile** | Enabled | Ensures the main Edge profile cannot be deleted by users, maintaining organizational control. |
| **Add profile enabled** | Disabled | Prevents users from creating additional browser profiles. |
| **Force ephemeral profiles** | Disabled | Users’ profiles are persistent and not reset at logoff; organization maintains control. |
| **Force sync** | Enabled | Ensures data sync for signed-in users is active, keeping bookmarks, passwords, and settings consistent. |
| **Implicit sign-in enabled** | Enabled | Allows users signed into Windows with their work account to automatically sign into Edge. |
| **AAD websites using this profile** | Enabled | Automatically applies Azure AD profiles to relevant websites for seamless access to work resources. |

---

## Key Security / Operational Benefits
- **Data Security:** Prevents unauthorized profile creation or deletion.  
- **User Consistency:** Maintains consistent browser settings across all endpoints.  
- **Enterprise Sync:** Ensures user data is synchronized securely across devices.  
- **Controlled Sign-In:** Automatic sign-in for work accounts improves user experience while maintaining security.

---

## Client Impact
- **End Users:** Some sign-in behaviors are automatic; users cannot create or delete profiles at will.  
- **IT Administration:** Simplifies management of Edge profiles and sign-in settings; fewer support requests for browser setup issues.  
- **Maintenance:** Periodic review of Edge policies may be needed as browser versions or organizational needs change.
