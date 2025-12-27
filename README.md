

# ⚙️ GearGuard – Maintenance Management System (Odoo)

## 📖 About the Project

**GearGuard** is a practical maintenance management system built using **Odoo Community Edition**.
The project focuses on managing **company assets**, assigning them to **maintenance teams**, and handling **repair and servicing requests** through a structured workflow.

The system is designed to simulate how maintenance operations work in real organizations such as factories, offices, and IT environments.

---

## 🎯 Purpose of the System

The main goals of GearGuard are:

* To maintain a **single source of truth for all equipment**
* To clearly define **who is responsible** for maintaining each asset
* To handle both **emergency repairs** and **scheduled maintenance**
* To visualize maintenance work using **Kanban boards and calendars**
* To demonstrate a **realistic business workflow using Odoo**

---

## 🧱 System Structure

The project is divided into three main components:

1. Equipment Records
2. Maintenance Teams
3. Maintenance Requests

Each component is interconnected to create a complete maintenance lifecycle.

---

## 🏭 Equipment Records

Equipment records represent all physical and IT assets owned by the organization.

### What information is stored:

* Equipment name and category
* Serial number and model
* Vendor and purchase-related details
* Warranty expiration date
* Physical location of the equipment
* Responsible maintenance team
* Assigned technician

### Equipment tracking is done by:

* **Department** (e.g., CNC Machine → Production)
* **Employee** (e.g., Laptop HR → Assigned user)

### Sample equipment used in the project:

* Generator
* Air Conditioner (AC)
* CNC Machine
* Printer 01
* Laptop HR

Each equipment record includes a **smart maintenance button** that displays the number of related maintenance requests.

---

## 👥 Maintenance Teams

To ensure proper responsibility and workflow separation, multiple maintenance teams are configured.

### Teams created:

* Mechanics
* Electricians
* IT Support
* Internal Maintenance

Each equipment is assigned to one of these teams.
When a maintenance request is created, it is automatically linked to the relevant team.

---

## 🔧 Maintenance Requests

Maintenance requests represent the actual maintenance work performed on equipment.

### Types of maintenance handled:

#### Corrective Maintenance

Used when equipment fails unexpectedly and needs immediate repair.

Examples:

* Generator not starting
* AC stopped working
* CNC machine vibration issue
* Laptop performance problem

#### Preventive Maintenance

Used for planned servicing to avoid future failures.

Examples:

* Monthly AC servicing
* Printer routine maintenance
* Quarterly generator inspection

---

## 🔄 Maintenance Workflow

### Corrective Maintenance Flow

1. A request is created for faulty equipment
2. Equipment selection auto-fills category and team
3. Request starts in **New** state
4. Technician assigns themselves
5. Work progresses to **In Progress**
6. After completion, request moves to **Repaired**
7. If repair is not feasible, request moves to **Scrap**

### Preventive Maintenance Flow

1. A preventive request is created
2. A scheduled date is assigned
3. Request appears in the calendar view
4. Technician performs planned maintenance

---

## 🖥️ User Interface Features

### Kanban Board

* Primary interface for technicians
* Displays maintenance requests by status
* Supports drag-and-drop between stages
* Shows assigned technician and request state

### Calendar View

* Displays all scheduled preventive maintenance
* Helps technicians plan upcoming work
* Allows creation of requests directly from the calendar

---

## ⚡ Smart System Features

### Equipment Maintenance Button

* Shows number of open requests per equipment
* Clicking it displays only related requests

### Scrap Handling

* Requests moved to Scrap indicate unusable equipment
* Equipment is logically considered retired
* Supports better asset lifecycle decisions

---

## 📊 Reporting & Visibility

The system allows maintenance activity analysis using built-in Odoo views:

* Requests per equipment
* Requests per maintenance team
* Current workload status

These insights help improve planning and efficiency.

---

## 🛠 Tools & Technologies Used

* Odoo Community Edition
* Maintenance Module
* PostgreSQL (default Odoo database)
* Web-based UI (Kanban, Calendar)

---
