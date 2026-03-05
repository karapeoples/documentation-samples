# cake-base — API Routes Reference

## Overview

cake-base is a demo REST API built for a local retail business.  
The architecture was intentionally designed to be modular and reusable so the same API structure can support different database schemas and workflows with minimal configuration changes.

By adjusting database naming conventions and configuration points, the API can be adapted for different inventory, management, or operational systems without major structural changes.

This project demonstrates organized route documentation, modular API design, and maintainable backend architecture.

---

## Base URL

Local Development

http://localhost:<port>

Example Base Route

BASEURL/user

---

## API Structure

Routes are grouped by domain to improve readability and maintainability.

Major route groups include:

- Users
- Clerks
- Patients
- Admin
- Product Inventory
- Inventory Stock
- Payroll Management

---

## User Routes

| Action | Method | Endpoint |
|------|------|------|
| Get All Users | GET | /all_user |
| Get User By ID | GET | /all_user/:user_id |
| Update User | PUT | /all_user/:user_id |
| Delete User | DELETE | /all_user/:user_id |

---

## Clerk Routes

| Action | Method | Endpoint |
|------|------|------|
| Get Clerks | GET | /clerk |
| Get Clerk By ID | GET | /clerk/:clerk_id |
| Get Clerk Role Info | GET | /clerk_info/:clerk_id |
| Delete Clerk Role | DELETE | /del_clerk/:clerk_id |

---

## Patient Routes

| Action | Method | Endpoint |
|------|------|------|
| Get Patients | GET | /patient |
| Get Patient By ID | GET | /patient/:patient_id |
| Get Patient Card | GET | /card/:patient_id |
| Update Card | PUT | /card/:patient_id |
| Delete Card | DELETE | /card/:patient_id |

---

## Admin Routes

| Action | Method | Endpoint |
|------|------|------|
| Get Admins | GET | /admin |
| Get Admin By ID | GET | /admin/:admin_id |
| Get Admin Role Info | GET | /admin_info/:admin_id |
| Delete Admin Role | DELETE | /del_admin/:admin_id |

---

## Product Inventory Routes

Base Route

BASEURL/strain

| Action | Method | Endpoint |
|------|------|------|
| Get Products | GET | /flower |
| Get Product By Name | GET | /flower/name/:name |
| Get Product By ID | GET | /flower/:flower_id |
| Add Product | POST | /flower |
| Update Product | PUT | /flower/:flower_id |

---

## Current Inventory Routes

| Action | Method | Endpoint |
|------|------|------|
| Get Current Inventory | GET | /flower_stock |
| Get Inventory By ID | GET | /flower_stock/:currentFlower_id |
| Add Inventory | POST | /flower_stock |
| Delete Inventory | DELETE | /flower_stock/:currentFlower_id |

---

## In-House Payroll Routes

| Action | Method | Endpoint |
|------|------|------|
| Get Payroll Entries | GET | /preRoll |
| Get Payroll By ID | GET | /preRoll/:preRoll_id |
| Add Payroll Entry | POST | /preRoll |
| Delete Payroll Entry | DELETE | /preRoll/:preRoll_id |

---

## Company Payroll Routes

| Action | Method | Endpoint |
|------|------|------|
| Get Company Payroll | GET | /companyPR |
| Get Payroll By Name | GET | /companyPR/name/:name |
| Get Payroll By ID | GET | /companyPR/:pr_id |
| Add Payroll Entry | POST | /companyPR |
| Update Payroll Entry | PUT | /companyPR/:pr_id |

---

## Current Payroll Routes

| Action | Method | Endpoint |
|------|------|------|
| Get Current Payroll | GET | /pr_stock |
| Get Current Payroll By ID | GET | /pr_stock/:currentPR_id |
| Add Current Payroll | POST | /pr_stock |
| Delete Current Payroll | DELETE | /pr_stock/:currentPR_id |

---

## Design Notes

The API structure was intentionally designed with:

- modular route groupings
- reusable database schema concepts
- clear documentation for developer onboarding

Although originally created as a demo for a retail environment, the architecture can be adapted for many types of inventory or administrative systems.
