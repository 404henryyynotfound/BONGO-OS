# Security Policy

## Supported Versions

Security updates and bug fixes are actively provided for the following versions of **BongoOS 11**:

| Version | Channel | Supported |
| ------- | ------- | --------- |
| `v1.1.0-beta` | Insider Preview (Beta) | :white_check_mark: Active |
| `v1.0.0` | Stable Release | :white_check_mark: Active |
| `< 1.0.0` | Pre-release / Prototypes | :x: Unsupported |

---

## Reporting a Vulnerability

We take the security and safety of **BongoOS 11** and its users seriously. If you discover a security vulnerability (such as Cross-Site Scripting (XSS), unsafe iframe sandboxing, or unintended data exposure), please report it responsibly:

1. **Do not** open a public GitHub Issue with exploit details before a fix is available.
2. If **Private Vulnerability Reporting** is enabled on this repository, go to the **Security** tab → **Advisories** → **Report a vulnerability**.
3. Alternatively, contact the repository maintainer directly via GitHub with:
   - A clear description of the vulnerability and potential impact.
   - Steps to reproduce the issue (or a minimal proof-of-concept).
   - Affected version (`v1.0.0` or `v1.1.0-beta`).

You can expect an initial acknowledgment within **48 hours**, and we will work with you to verify and patch the issue promptly.

---

## Security & Privacy Notes for Self-Hosting

Because **BongoOS 11** runs entirely in the user's browser as a static web application:

- **Local Storage Only**: All virtual files, notes, and drawings created in BongoOS are stored locally in the visitor's browser via `localStorage` and are never uploaded to a central server.
- **Protecting Your Gemini API Key**: If you add a Google Gemini API key to `index.html` for public hosting (such as GitHub Pages), make sure to restrict the key in [Google Cloud Console](https://console.cloud.google.com/) using **HTTP referrer restrictions** (e.g., `https://<your-username>.github.io/*`) and set usage quotas so others cannot abuse your key.
- **External Embedded Frames**: **BongoChrome** embeds third-party public sites (such as Wikipedia and OpenStreetMap) via standard `<iframe>` elements, which remain isolated by the browser's Same-Origin Policy.
