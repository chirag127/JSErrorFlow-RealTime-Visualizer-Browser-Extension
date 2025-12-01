# 🛡️ Security Policy for JSErrorFlow Real-Time Visualizer Extension

This document outlines the security procedures for reporting and addressing vulnerabilities found in the `JSErrorFlow-RealTime-Visualizer-Browser-Extension`.

As an elite tool operating within the browser sandbox, security is paramount. We adhere to the **Zero Trust** principle for all user data and extension interactions.

## 1. Supported Versions

We actively support and patch the latest production version of the extension. Security fixes will be prioritized and backported to the immediately preceding minor release if applicable.

| Version | Support Status | Maintenance Cycle |
| :--- | :--- | :--- |
| **v2.x.x** | Active Support | Immediate Patch Release |
| v1.x.x | Limited Support | Critical Fixes Only |

## 2. Vulnerability Disclosure Policy (VDP)

We strongly encourage responsible disclosure. Do not disclose vulnerabilities publicly (e.g., GitHub Issues, public forums) before a patch has been deployed or coordination has concluded.

### Reporting Procedure

All security reports **must** be submitted privately via a GitHub Security Advisory (or securely emailed if the advisory feature is unavailable).

1.  **Navigate to the 'Security' Tab** on this repository.
2.  Click **'Report a vulnerability'** and fill out the required details.

If you cannot use the GitHub Advisory tool, please use the following fallback email, which is monitored by the Apex Security Team:

`security+jserrorflow@apex-architects.io` (Replace with a real contact if this were a live project)

### Required Information in Report
To ensure rapid triage, please include:

*   **Vulnerability Type:** (e.g., XSS, CSRF, Information Leak).
*   **Affected Component:** (e.g., `content-script.ts`, `background-service.js`).
*   **Proof of Concept (PoC):** Detailed, minimal steps to reproduce the issue.
*   **Impact Assessment:** How could an attacker exploit this? (e.g., Steal user data, disrupt extension functionality).
*   **Suggested Mitigation:** Any known workarounds or fixes.

## 3. Security Response Times & SLA

We commit to the following service level objectives (SLO) for security issues, based on severity:

| Severity | Initial Acknowledgment | Target Fix & Release |
| :--- | :--- | :--- |
| **Critical** (Remote Code Execution, Data Exfiltration) | Within 4 Business Hours | Within 48 Business Hours |
| **High** (DOM Manipulation, Privilege Escalation) | Within 12 Business Hours | Within 7 Calendar Days |
| **Medium** (Information Disclosure, Logic Flaws) | Within 24 Business Hours | Within 14 Calendar Days |
| **Low/Informational** (Best Practice Suggestions) | Within 3 Business Days | Next Scheduled Minor Release |

## 4. Security Practices & Tooling

This project enforces a strict DevSecOps pipeline to minimize vulnerabilities:

*   **Dependency Scanning:** All dependencies are scanned on every CI run using specialized tools (e.g., Snyk integration) to detect known CVEs. Updates for vulnerable dependencies are automatically prioritized via Dependabot/Renovate.
*   **Static Analysis:** **Biome** and **TypeScript (Strict Mode)** are configured to catch common pitfalls like type coercion errors and insecure API usage.
*   **Content Security Policy (CSP):** Strict CSP headers are enforced within the extension manifest to prevent injection attacks where feasible.
*   **Input Sanitization:** **ALL** data passed between the Content Script, Background Script, and any user-facing rendering layers is rigorously sanitized (using DOMPurify equivalents or trusted native methods).
*   **Principle of Least Privilege:** The extension operates with the minimum necessary host permissions.

## 5. Remediation Process

1.  **Triage:** Security team classifies the issue and assigns severity.
2.  **Patch Development:** A dedicated, isolated branch is created for the fix.
3.  **Verification:** The fix is thoroughly tested using specialized E2E tests (**Playwright**) to confirm the vulnerability is closed and no regressions are introduced.
4.  **Review:** The patch undergoes mandatory review by at least two senior architects.
5.  **Release:** A patched version is immediately released to the relevant extension stores (or deployed via the CI workflow).