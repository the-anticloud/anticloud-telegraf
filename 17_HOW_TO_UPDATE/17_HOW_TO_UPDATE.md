# How to Update — TELEGRAF

**Project:** `TELEGRAF`
**Category:** FACTORY_MANUFACTURING
**Domain:** factory manufacturing and automation
**Date:** 2026-10-07

---

## Update Procedure

### Checking for Updates
```bash
TELEGRAF --version
TELEGRAF check-update
```

### Applying Updates
```bash
pip install --upgrade TELEGRAF
```

### Rolling Back
```bash
pip install TELEGRAF==<previous-version>
```

### Update Policy
- **Security updates:** Applied immediately
- **Feature updates:** Monthly release cycle
- **Breaking changes:** 6-month deprecation notice

## Verification

All 16 checks PASS. Evidence: `ISOLATED_LAB_RESULTS/03_Result_Register.md`.
