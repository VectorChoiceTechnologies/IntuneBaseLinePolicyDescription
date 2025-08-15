# Intune Endpoint Security – BitLocker Policy

**Policy Name:** Win - OIB - ES - Encryption - D - BitLocker (OS Disk) - v3.0  
**Platform:** Windows 10 and later  
**Policy Type:** Endpoint Security – Disk Encryption (BitLocker)  
**Purpose:** Enforces encryption settings for the Operating System (OS) drive to protect data in case of device loss or theft.

---

## Policy Overview
This policy ensures all organization-managed Windows devices have BitLocker enabled with standardized encryption settings for compliance, security, and recoverability. It applies to the OS drive (system drive) only.

---

## Configuration Details

| Setting | Configured Value | Purpose / Effect |
|---------|------------------|------------------|
| **System Drive Encryption Type** | Full Encryption (XTS-AES 256-bit) | Encrypts the entire OS drive with strong encryption for maximum data protection. |
| **Startup Authentication Requirement** | TPM only (no PIN or startup key required) | Simplifies user experience while still leveraging Trusted Platform Module (TPM) for secure key storage. |
| **Change PIN Restriction** | Standard users cannot change BitLocker PINs | Prevents unauthorized modification of encryption credentials. |
| **Recovery Options** | Recovery key required; recovery page hidden from users; Active Directory (or Azure AD) backup enforced | Ensures recovery keys are stored securely for IT access and prevents users from bypassing policy. |
| **Encryption Method** | XTS-AES 256-bit for OS, fixed, and removable drives | Provides consistent encryption strength across all drive types. |
| **Device Encryption Requirement** | Device must be encrypted | Prevents devices from operating without encryption enabled. |
| **Other Disk Encryption Warning** | Disabled (standard users can start encryption) | Avoids unnecessary warnings if other encryption is present but still allows authorized encryption operations. |
| **Recovery Password Rotation** | Enabled after use | Ensures recovery passwords are rotated for better security after they are used. |

---

## Key Security Benefits
- **Data Protection:** Protects all OS drive data at rest using enterprise-grade encryption.
- **Compliance:** Meets common regulatory requirements (HIPAA, GDPR, CJIS, etc.).
- **User Transparency:** Minimal disruption to end users while enforcing strong security.
- **Recovery Assurance:** Recovery keys are securely backed up for IT use.
- **Future-Proof Encryption:** Uses 256-bit encryption to meet evolving security standards.

---

## Client Impact
- Users will **not** need to manually enable BitLocker — it is enforced automatically.
- Devices will encrypt in the background after policy application.
- Users will not be prompted for additional startup authentication (TPM handles this securely).
- If a device enters BitLocker recovery mode, IT will have the recovery key stored in Azure AD/Active Directory.
- Recovery passwords will automatically rotate after use to prevent re-use.
