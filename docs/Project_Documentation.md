# Mos3ef Project Documentation

**Version:** 1.0  
**Date:** November 30, 2025

---

## Table of Contents
1.  [Executive Summary](#1-executive-summary)
2.  [Project Management](#2-project-management)
3.  [Requirements Analysis](#3-requirements-analysis)
4.  [System Architecture](#4-system-architecture)
5.  [UI/UX Design](#5-uiux-design)

---

## 1. Executive Summary

### 1.1 Overview
**Mos3ef** is a comprehensive digital healthcare platform designed to bridge the gap between patients and hospitals. It allows patients to search, filter, and compare medical services based on price, rating, location, and availability, while enabling hospitals to manage their service catalogs and analytics efficiently.

### 1.2 Objectives
*   **Accessibility:** Provide instant access to hospital service details and working hours.
*   **Transparency:** Enable price and rating comparisons between healthcare providers.
*   **Efficiency:** Digitalize hospital profile and service management.
*   **Quality Assurance:** Maintain high standards through a patient review system.

### 1.3 Scope
**In Scope:**
*   User Authentication (JWT) with Role-Based Access Control (Patient, Hospital, Admin).
*   Hospital Profile & Service Catalog Management.
*   Advanced Search & Filtering (Keyword, Category, Location).
*   Service Comparison Tool (Price, Rating, Availability).
*   Patient Reviews & Ratings.
*   Hospital Dashboard Analytics.

**Out of Scope:**
*   Real-time ambulance tracking.
*   In-app payment processing.
*   Telemedicine video calls.

---

## 2. Project Management

### 2.1 Timeline
The project follows a 13-week timeline from October 1 to December 30, 2025.

![Project Timeline](images/gantt_chart.png)

*   **Planning:** Oct 1 – Oct 15
*   **Analysis:** Oct 15 – Oct 29
*   **Design:** Oct 29 – Nov 12
*   **Implementation:** Nov 12 – Dec 10
*   **Testing:** Dec 10 – Dec 24
*   **Deployment:** Dec 24 – Dec 30

### 2.2 Risk Assessment
| Risk | Mitigation Strategy |
| :--- | :--- |
| **Data Privacy/Security** | Implementation of JWT authentication and secure token management. |
| **Data Accuracy** | Use of precise latitude/longitude fields for location mapping. |
| **Performance** | Implementation of caching strategies for high-load operations. |

---

## 3. Requirements Analysis

### 3.1 Stakeholders
*   **Patients:** End users seeking medical services. Needs: Fast search, accurate pricing, trusted reviews.
*   **Hospitals:** Service providers. Needs: Service management, user feedback, analytics.
*   **Administrators:** System owners. Needs: User management, system integrity.

### 3.2 Functional Requirements
*   **Authentication:** Secure registration and login for all roles.
*   **Hospital Module:** CRUD operations for services, profile management, dashboard stats.
*   **Patient Module:** Profile management, search/filter services, wishlist, reviews.
*   **Core Features:** Service comparison engine, geo-location filtering.

### 3.3 Non-Functional Requirements
*   **Performance:** API response time < 200ms for search queries.
*   **Scalability:** Modular 3-Tier Architecture (DAL, BLL, API).
*   **Reliability:** ACID compliance via SQL Server transaction management.

---

## 4. System Architecture

### 4.1 Technology Stack
*   **Backend:** .NET 8 Web API
*   **Frontend:** React 19 (Vite) with Tailwind CSS
*   **Database:** Microsoft SQL Server
*   **ORM:** Entity Framework Core (Code-First)
*   **Mapping:** AutoMapper

### 4.2 Database Design
The database utilizes a relational model to ensure data integrity.

![ER Diagram](images/erd.png)

![Database Schema](images/schema.png)
*   **Key Entities:** `User` (Base), `Patient`, `Hospital`, `Service`, `Review`.
*   **Relationships:** One-to-Many (Hospital -> Services), One-to-Many (Service -> Reviews).

---

## 5. UI/UX Design

### 5.1 Design Philosophy
The interface prioritizes accessibility and ease of use, utilizing a "Medical Blue" color palette for trust and calmness.

### 5.2 Key Screens
*   **Landing Page:** Centralized search bar with category filters.
*   **Results Grid:** Service cards displaying price, rating, and hospital info.
*   **Comparison Modal:** Side-by-side view of selected services highlighting best options.
*   **Hospital Dashboard:** Analytics cards (Views, Ratings) and service management table.

### 5.3 UX Considerations
*   **Feedback:** Toast notifications for user actions.
*   **Validation:** Real-time form validation.
*   **Performance:** Skeleton loaders during data fetching.
