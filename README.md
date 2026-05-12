# DPDP-Compliant Healthcare Document Intelligence Platform

## Overview

This project was developed during my internship at DataDives as a Data Engineering Intern. The platform focuses on secure healthcare document processing using OCR automation, intelligent PII detection, and compliance-oriented workflows aligned with India’s Digital Personal Data Protection (DPDP) Act 2023.

The system processes healthcare documents such as prescriptions, lab reports, and discharge summaries while ensuring secure handling of sensitive patient information through masking, encryption, immutable audit logging, and consent-driven access control.

---

## Problem Statement

Healthcare organizations process thousands of medical PDFs daily containing sensitive information such as:
- Patient Names
- Aadhaar Numbers
- Phone Numbers
- Clinical Data
- Prescription Information

Manual review and masking of such information is not scalable. The objective of this platform was to automate OCR extraction, PII detection, secure storage, and compliance workflows using a cloud-native architecture.

---

## Key Features

### OCR & Document Intelligence
- OCR extraction using AWS Textract
- Sync and Async OCR workflows
- Document classification:
  - LAB_REPORT
  - PRESCRIPTION
  - OTHER
- Text normalization and structured extraction

### PII Detection & Protection
- AWS Comprehend-based NLP detection
- Regex fallback validation
- Aadhaar, PAN, Phone, Email detection
- Multi-layer protection:
  - Masking
  - SHA-256 Hashing
  - AWS KMS Encryption

### Security & Compliance
- JWT Authentication
- Role-Based Access Control (RBAC)
- Consent-Gated Unmasking
- Immutable Audit Logging
- Data Subject Rights (DSR) workflows
- Legal Hold & Retention Policies

### Cloud-Native Architecture
- AWS EC2
- AWS S3
- AWS Textract
- AWS Comprehend
- AWS KMS
- PostgreSQL RDS

---

## Technology Stack

| Category | Technologies |
|---|---|
| Backend | FastAPI, Python |
| Database | PostgreSQL |
| Cloud | AWS EC2, S3, RDS |
| OCR | AWS Textract |
| NLP | AWS Comprehend |
| Security | JWT, AWS KMS |
| Storage | S3 |
| Dev Tools | GitHub, Ubuntu |

---

## Architecture Highlights

- Multi-tenant healthcare document processing
- Async OCR orchestration for large PDFs
- Tenant-aware isolation and secure access control
- Hash-chained immutable audit logging
- Compliance-oriented healthcare workflows

---

## Security Features

- AES-256 encryption using AWS KMS
- SHA-256 tamper-evident audit chain
- Consent-based access workflows
- Role-based masking enforcement
- Secure HTTPS communication
- IAM least-privilege architecture

---

## Learning Outcomes

This internship provided hands-on experience in:
- Cloud-native backend engineering
- OCR system orchestration
- AWS architecture
- Privacy-focused healthcare systems
- Compliance engineering
- Multi-tenant system design
- Production-oriented API development

---

## Disclaimer

This repository contains only high-level architectural and educational material developed as part of an internship project. No proprietary company source code, credentials, internal APIs, or confidential implementation details are included.

---

## Author

P. Pushyamithra  
B.Tech CSE — IIIT Guwahati  
Data Engineering Intern — DataDives
