# AutopilotDoctor

**Portable, zero-telemetry Windows Autopilot, Entra ID, Intune MDM, TLS/SSL Inspection & 802.1X diagnostic engine.**

Built for SysAdmins and MSPs troubleshooting stubborn OOBE (`Shift+F10`) and Enrollment Status Page (ESP) failures without installing agents or collecting heavy `MDMDiagnostics` CAB logs first.

[![Download Latest Release](https://img.shields.io/badge/Download-v1.3.0%20(Free%20Edition)-2563eb?style=for-the-badge&logo=windows)](https://github.com/autopilotdoctor/AutopilotDoctor/releases/latest)
[![Live Overview](https://img.shields.io/badge/Website-Documentation-0f172a?style=for-the-badge)](https://autopilotdoctor.github.io/AutopilotDoctor/)
[![Pro & MSP License](https://img.shields.io/badge/Upgrade-Pro%20%2F%20MSP%20License-16a34a?style=for-the-badge)](https://autopilotdoctor.gumroad.com/l/qtryi)

---

### Interactive HTML Dashboard Preview (Anonymized Mode)

![AutopilotDoctor Anonymized HTML Diagnostic Report](a1.png)

---

## What It Checks in ~10 Seconds

* **Identity & Hardware Readiness:** Entra ID join state, Primary Refresh Token (PRT) health, MDM enrollment URLs, TPM 2.0 attestation readiness, and BitLocker status.
* **Network & SSL Inspection Validation:** Direct TCP 443 and TLS certificate chain checks against Microsoft Autopilot, Intune, Delivery Optimization, and Graph endpoints (immediately flags Zscaler, Palo Alto, or FortiGate SSL decryption breaks).
* **Certificates & 802.1X:** SCEP/PKCS client certificate validity, private key permissions, and wired/wireless 802.1X supplicant health.
* **Intune Management Extension (IME):** Win32 app and PowerShell script failure parsing, exit codes, and deployment bottlenecks.
* **1-Click Safe Sharing Anonymizer:** Automatically masks Tenant IDs, hostnames, UPNs, Wi-Fi SSIDs, and internal app names before exporting a standalone dark/light HTML report for ticket escalations.

---

## Quick Start (OOBE or Live Desktop)

1. Download **`AutopilotDoctor.exe`** from the [Releases](https://github.com/autopilotdoctor/AutopilotDoctor/releases/latest) page.
2. Run as **Administrator** (or launch directly from a USB drive inside Windows OOBE via `Shift + F10`).
3. *(Optional)* Check **Anonymize Sensitive Identifiers** before scanning if you plan to share the report externally.
4. Click **Run Full Diagnostic Scan** to generate an interactive standalone HTML report.

---

## Editions

| Feature | Free Edition | Pro / MSP Edition |
| :--- | :---: | :---: |
| Full Diagnostic Engine (Modules A–E) | Yes | Yes |
| Standalone Dark/Light HTML Report | Yes | Yes |
| 1-Click Tenant, Hostname & UPN Anonymizer | Yes | Yes |
| Copy-Paste CLI Remediation Commands | — | **Yes** |
| Hex Error Root-Cause Mapping | — | **Yes** |
| Raw `.json` Export for Automation/SIEM | — | **Yes** |
| Offline 30-Day OOBE License Caching | — | **Yes** |

* **Zero Telemetry:** Runs 100% locally using native PowerShell and .NET sockets. No diagnostic data ever leaves the endpoint.
* **Perpetual Licensing:** One-time license options for [Pro SysAdmin (3 Seats) & MSP Teams (15 Seats)](https://autopilotdoctor.gumroad.com/l/qtryi).
