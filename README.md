# Chemistry Lab Clearance & Asset Management System

A web-based administrative inventory and clearance tracking portal designed for academic chemistry laboratories to manage apparatus checkouts, fine collections, and student semester promotion holds.

---

## Key Features

* Granular Inventory Tracking: Real-time stock monitoring for glassware, chemical reagents, and precision laboratory instruments with digital checkout tracking.
* Academic Promotion Clearance Guards: Automated validation gate preventing students with unsettled apparatus breakage fines from obtaining semester registration clearance passes.
* Audit Logs & Incident Logging: Comprehensive record keeping of all item allocations, breakage reports, fine receipts, and supervisor clearances.
* Alumni Batch Archiving: End-of-year batch archival that moves graduating student records into a long-term read-only historical datastore.

---

## Technical Stack

* Backend: PHP 8.x, MySQL (Prepared Statements, Foreign Key Constraints)
* Frontend: Vanilla JavaScript (ES6+), Glassmorphic CSS, HTML5
* Data Layer: Normalized Relational Database Schema

---

## Clearance Pipeline Workflow

[Student Lab Session] ────► [Breakage Occurs] ────► [Lab Instructor Logs Incident]
                                                                  │
                                                                  ▼
[Promotion Clearance Pass: LOCKED] ◄─── [Fine Assessed & Added to Student Account]
                │
                ▼
      [Fee Settlement Made]
                │
                ▼
[Promotion Clearance Pass: ISSUED] ────► [Record Archived to Alumni Ledger]

---

## Live Deployment & Verification

* Live Instance: https://ssvchemlab.infinityfree.io/?i=1
* Access Role: Academic laboratory management interface featuring live apparatus accounting, breakage penalty processing, and student clearance logs.
