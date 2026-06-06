# Ants-Review Architecture

## Review Engines

### Open Code Review

Purpose:
- PR Review
- Diff Review
- Maintainability

### Metis

Purpose:
- Security Review
- OWASP
- CWE Mapping

### CyberAnts Layer

Purpose:
- Business Logic Review
- Tenant Isolation
- Authorization Review
- Human Verification

## Review Flow

Repository
    ↓
OCR
    ↓
Metis
    ↓
Normalizer
    ↓
CyberAnts Rules
    ↓
Final Verdict
