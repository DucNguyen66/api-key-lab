#Developer Security Policy

## 1. Purpose
This document provides security guidelines for developers to prevent secret leakage, data exposure, and insecure configurations within the source code.

## 2. Scope
Applies to all contributors in this repository (`api-key-lab`) and any future project under organization `DucNguyen66` .

## 3. Secure Development Rules
  **Never commit secrets** (API keys, tokens, passwords) into Git.
  **Scan before commit** using `pre-commit` hooks with Gitleaks.
  **Use environment variables** for temporary credentials only.
  **Encrypt sensitive files** (config.yaml, .env) before storing or sharing.

## 4. Incident Response Steps
  If a secret is found committed:
  1. Revoke the exposed key immediately.
  2. Alert the security or DevOps lead.
  3. Remove the secret from Git history.
  4. Replace it with a new one.
  5. Document the incident in `incident_report.txt`

## 5. Developer Awareness
  - All team members must complete annual traning on Secure Coding and Secret Management.
  - Developers must review this policy before contributing code.

## 6. Enforcement
Violation of this policy may result in removal of commit access of other disciplinary action per organization guidelines.


---
**Maintainer:** DucNguyen
**Last Updated:** October 2025
