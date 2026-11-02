# Loki Café - Stock Inventory System

A lightweight, console-based stock and inventory management application written in Python.  
Designed to help coffee shop owners and staff manage stock levels, track deliveries, monitor ingredient expiration dates, and log shift handover reports seamlessly.

---

## Overview

Loki Café Inventory System simplifies daily cafe operations by separating tasks into **Admin** and **Staff** roles. It ensures real-time visibility over perishable ingredients to minimize waste and prevent inventory shortages.

---

## Key Features

### Admin Capabilities
1. **Full Inventory Control:** Add new ingredients, update stock quantities, or delete outdated items.
2. **Delivery Logs:** Record incoming shipments and view comprehensive delivery history tables.
3. **Alert Filtering:** Filter items by stock status (Low Stock, Expired, Expiring Soon).
4. **Shift Management:** Review handover reports submitted by staff members.
5. **Account Management:** Register new staff user accounts.

### Staff Capabilities
1. **Stock Deductions:** Record ingredient usage during regular shop operations.
2. **Delivery Registration:** Log incoming inventory items upon arrival.
3. **Alert Monitoring:** Check ingredients that need immediate attention or restock.
4. **Shift Handovers:** Submit shift reports before logging out.

---

## System Credentials

Default system accounts for initial testing:

Role | Username | Password
--- | --- | ---
**Admin** | `admin` | `admin123`
**Staff** | `loki` | `loki123`

---

## Initial Inventory Sample

ID | Item Name | Quantity | Unit | Threshold | Expiry Date | Status
--- | --- | --- | --- | --- | --- | ---
1 | Espresso Beans | 10 | kg | 3 | 2026-10-15 | Safe
2 | Dairy Cream | 2 | L | 5 | 2026-10-05 | Expired
3 | Caramel Syrup | 4 | L | 2 | 2026-12-01 | Safe
4 | Fresh Milk | 1 | L | 5 | 2026-10-12 | Low Stock / Expiring

---

## Installation & Execution

### Prerequisites
* Python 3.x installed on your system.

### How to Run
1. Clone or download this repository.
2. Open your terminal / command prompt.
3. Run the following command:

```bash
python inventory.py

or

python3 inventory.py

Technical Highlights

1. Automated Expiration & Low-Stock Detection: Checks expiration dates against the current date and flags items expiring within 7 days or falling below minimum thresholds.
2. Strict Input Validation: Prevents invalid user inputs (e.g., negative stock values, incorrect date formats like YYYY-MM-DD).
3. Zero External Dependencies: Built purely with Python's standard library (sys and datetime).

Limitations & Future Enhancements
1. In-Memory Storage: Current data resets upon program termination.
2. Console-Based Interface: Text-driven CLI environment.
3. Planned Improvements: File persistence (JSON/CSV), database integration (SQLite), and a Graphical User Interface (GUI).

Author
Developed as a student project.

Open for contributions, feedback, and further enhancements!
