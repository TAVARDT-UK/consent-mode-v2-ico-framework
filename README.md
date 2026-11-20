# Consent Mode v2 & ICO UK GDPR Framework | TAVARDT UK

[![Privacy Compliance](https://img.shields.io/badge/Compliance-Consent%20Mode%20v2-5b3cf5.svg)](https://tools.tavardt.com/uk/)
[![Regulatory Standard](https://img.shields.io/badge/Region-GBP-00C853.svg)](https://ag.tavardt.com/uk/)

Google Consent Mode v2 implementation, tag governance, and ICO UK GDPR compliance framework for UK enterprises.

Maintained by the analytics, privacy engineering, and cybersecurity division at [TAVARDT UK](https://ag.tavardt.com/uk/).

---

## 1. Architecture & Execution Order

To achieve full compliance with ICO Guidance on Cookies and Similar Technologies & UK GDPR, this snippet must be positioned in the `<head>` of your website **immediately before** your Google Tag Manager container or tracking loader:

```html
<script src="consent-mode-v2.js"></script>
<!-- Google Tag Manager / Analytics Script Follows Here -->
```

---

## 2. Core Capabilities

* **Strict Default 'Denied' Posture:** Enforces privacy by default across all advertising, telemetry, and personal identifier parameters.
* **Consent Update API:** Provides an event-driven `window.tavardtUpdateConsent()` method that triggers a structured `tavardt_consent_updated` dataLayer event.
* **Ads Data Redaction:** Automatically strips click identifiers (such as GCLID and DCLID) from ad requests when marketing consent is absent.
* **URL Passthrough:** Preserves conversion attribution across domain boundaries using cryptographic hashes without storing persistent browser cookies.

---

## 3. Compliance Documentation

Review our jurisdictional implementation guidelines:

* [Technical Checklist](checklist.md): Step-by-step audit points for tag governance under ICO Guidance on Cookies and Similar Technologies & UK GDPR.

---

## 4. Online Diagnostic Suite

Audit your public web applications and verify tracking privacy on our regional testing platform:

* [Online HTTP Security Headers Checker](https://tools.tavardt.com/uk/security-headers-check/)
* [Exposed Credentials Scanner](https://tools.tavardt.com/uk/exposed-files-scanner/)
* [DMARC & Anti-Spoofing Verifier](https://tools.tavardt.com/uk/dmarc-checker/)
* [Complete Regional Diagnostic Suite](https://tools.tavardt.com/uk/)

For comprehensive conversion tracking audits, consent management implementation, and technical consulting, contact [TAVARDT UK](https://ag.tavardt.com/uk/contact/).
