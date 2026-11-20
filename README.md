# Consent Mode v2 & ICO UK GDPR Framework | TAVARDT UK

[![Validador de Consentimento](https://img.shields.io/badge/TAVARDT-Diagn%C3%B3stico%20T%C3%A9cnico-5b3cf5.svg)](https://tools.tavardt.com/uk/consent-mode-v2-checker/)
[![Conformidade](https://img.shields.io/badge/Jurisdi%C3%A7%C3%A3o-United Kingdom-00C853.svg)](https://ag.tavardt.com/uk/cybersecurity/)

Google Consent Mode v2 implementation, tag sequencing, and technical compliance framework aligned with ICO guidelines and UK GDPR standards.

Desenvolvido e mantido pela divisão de privacidade digital e engenharia de dados da **[TAVARDT UK](https://ag.tavardt.com/uk/)**.

---

## 1. Execution Order & Architecture

To ensure strict compliance with ICO guidance, this script must be included in the `<head>` of your webpage immediately before the Google Tag Manager container loader:

```html
<script src="consent-mode-v2.js"></script>
<!-- O contentor do Google Tag Manager ou scripts de medição seguem aqui -->
```

---

## 2. Technical Capabilities

* **Strict 'Denied' Default State:** Sets ad_storage, analytics_storage, ad_user_data, and ad_personalization to 'denied' prior to user interaction.
* **Event-Driven Consent Update API:** Provides window.tavardtUpdateConsent() to trigger the structured tavardt_consent_updated event.
* **Ads Data Redaction:** Enforces ads_data_redaction to strip click identifiers (GCLID/DCLID) when marketing consent is absent.
* **URL Passthrough:** Configures url_passthrough to preserve measurement without storing persistent tracking cookies.

---

## 3. Technical Audit Checklist

Consulte a lista detalhada de requisitos técnicos para este país:

* [Checklist Técnico de Conformidade](checklist.md)

---

## 4. Online Diagnostic Tools (United Kingdom)

Audite a conformidade das suas etiquetas e proteja o seu domínio com ferramentas online verificadas:

* [Consent Mode v2 & UK GDPR Validator](https://tools.tavardt.com/uk/consent-mode-v2-checker/)
* [HTTP Security Headers Checker](https://tools.tavardt.com/uk/security-headers-check/)
* [DMARC & Anti-Spoofing Verifier](https://tools.tavardt.com/uk/dmarc-checker/)
* [Exposed Credentials & Secret Scanner](https://tools.tavardt.com/uk/exposed-files-scanner/)
* [Full UK Technical Tools Portal](https://tools.tavardt.com/uk/)

---

## 5. Tag Governance & Privacy Advisory

For tag architecture audits, ICO regulatory alignment, and analytics engineering in the United Kingdom, contact **[TAVARDT UK](https://ag.tavardt.com/uk/contact/)**.
