# 🐾 Paw-Care Center - Pet Care Database Management System

A centralized Relational Database Management System (RDBMS) designed to organize, secure, and streamline operational data for the **Paw-Care Center**. The system replaces paper-based records with structured data tracking for pet owners, pets, caretakers, medical health records, and billing invoices.

---

## 📌 Project Overview
* **Domain:** Healthcare & Pet Care Center Operations Management
* **Development Methodology:** Waterfall Lifecycle (Requirement Analysis ➔ Database Design ➔ Normalization ➔ SQL Implementation ➔ Testing)
* **Core Technologies:** MySQL / SQL, Relational Database Modeling
* **User Interfaces:** Front-end system UI wireframes designed for registration, records tracking, and invoicing

---

## 🎯 Key Objectives & Solutions
1. **Data Centralization:** Replaces manual records to eliminate data duplication, inconsistencies, and record loss.
2. **Accurate Tracking:** Links pet health histories, diagnoses, treatments, caretaker shift assignments, and owner details.
3. **Role-Based Security & Confidentiality:** Implements distinct user roles and SQL views/grants:
   * **Admin:** Full CRUD access (Create, Read, Update, Delete) across all database tables.
   * **Caretakers:** Access to manage pet treatments and update health records.
   * **Pet Owners:** Read-only access restricted strictly to their personal and pet data via customized SQL Views.

---

## 📐 Database Architecture & Schema
The relational database structure consists of five main entities:
* `owner` – Stores client contact details and total pet counts.
* `pet` – Tracks pet details, species, admission dates, and current health status.
* `caretaker` – Manages caretaker profiles, contact info, and shift schedules.
* `healthrecord` – Records diagnostic dates, medical observations, and prescribed treatments.
* `invoice` – Tracks payment types (Cash, Card, QR Payment) and transaction amounts.

---

## 💻 Key SQL Features & Views
* **Relational Joins:** Multi-table `INNER JOIN` queries linking Owners, Pets, Caretakers, and Health Records.
* **Data Security Views:** Custom views (`Owner1000View`) restricted with `GRANT SELECT` to ensure privacy.
* **Billing & Audit Queries:** Filters unpaid invoice transactions and automates record updates/deletions.

