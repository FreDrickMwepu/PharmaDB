# PharmaDB

The Prescriptions-R-X chain of pharmacies has tasked us with designing a comprehensive database to manage their operations. This project aims to ensure efficient and secure handling of patient information, doctor records, pharmaceutical company data, drug details, prescriptions, and contracts between pharmacies and pharmaceutical companies.

## Project Overview

This project involves the following key components:

1. **Database Schema Design**:
    - **Patients**: SSN, name, address, and age.
    - **Doctors**: SSN, name, specialty, and years of experience.
    - **Pharmaceutical Companies**: Name and phone number.
    - **Drugs**: Trade name, formula, and associated pharmaceutical company.
    - **Pharmacies**: Name, address, and phone number.
    - **Prescriptions**: Date, quantity, patient, doctor, and drug details.
    - **Contracts**: Start date, end date, contract text, and supervisor information.

2. **Relationships**:
    - **Patient-Doctor**: Each patient has a primary physician, and each doctor has multiple patients.
    - **Pharmacy-Drug**: Many-to-many relationship with pricing details.
    - **Doctor-Prescription**: One-to-many relationship.
    - **Patient-Prescription**: One-to-many relationship.
    - **Pharmaceutical Company-Pharmacy**: Many-to-many relationship with contract details.
    - **Contract-Supervisor**: One-to-one relationship.

## Practical Requirements

### User Interface Design

Develop a user-friendly interface that allows pharmacy staff to easily enter and retrieve information about:
- Patients
- Doctors
- Pharmaceutical companies
- Drugs
- Prescriptions
- Contracts

### Data Integrity and Security

Implement measures to ensure the integrity and security of sensitive data:
- Use encryption for sensitive data (e.g., patient SSNs).
- Implement role-based access control to restrict access to sensitive information.
- Ensure referential integrity with proper constraints (e.g., foreign keys).

### Reporting and Analytics

Develop reporting and analytics tools to help analyze prescription trends, drug sales, and doctor performance. This includes:
- Generating monthly reports on drug sales per pharmacy.
- Analyzing patient demographics and prescription patterns.
- Creating dashboard views for quick access to key metrics.
