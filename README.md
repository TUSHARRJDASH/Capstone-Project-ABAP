# Capstone-Project-ABAP
# 📊 Custom Sales Order ALV Report (SAP ABAP)

## 🚀 Overview

This project is a **Custom SAP ABAP ALV Report** developed to display **Sales Order data** in an interactive and user-friendly format.

The report integrates data from multiple SAP SD tables and presents it using the **ALV Grid Display**, enabling business users to analyze sales orders efficiently.

---

## 🎯 Objective

To design and implement a **custom ALV report** that:

* Combines **Sales Order header, item, and customer data**
* Provides **interactive filtering and sorting**
* Enables **drill-down navigation to VA03**
* Improves decision-making with **real-time insights**

---

## 🏗️ System Architecture

```
User Input (Selection Screen)
        ↓
ABAP Program (SE38)
        ↓
Database Tables (VBAK, VBAP, KNA1, VBUK)
        ↓
Internal Table Processing
        ↓
ALV Grid Display
```

---

## 🧩 Features

* 🔍 **Selection Screen Filters**

  * Sales Organization
  * Customer
  * Date Range

* 📊 **Interactive ALV Grid**

  * Sorting & Filtering
  * Column customization
  * Zebra layout

* 🚦 **Traffic Light Indicator**

  * 🟢 Green → Completed/Open
  * 🟡 Yellow → In Process
  * 🔴 Red → Blocked

* 🔗 **Drill-down Navigation**

  * Double-click → Opens **VA03 (Display Sales Order)**

* ➕ **Totals & Aggregation**

  * Automatic sum for Net Value

---

## 🛠️ Tech Stack

| Component | Technology                    |
| --------- | ----------------------------- |
| Language  | ABAP                          |
| Module    | SAP SD (Sales & Distribution) |
| ALV Tool  | REUSE_ALV_GRID_DISPLAY        |
| Tables    | VBAK, VBAP, KNA1, VBUK        |
| IDE       | SAP ABAP Workbench (SE38)     |

---

## 🗃️ Database Tables

| Table | Description        |
| ----- | ------------------ |
| VBAK  | Sales Order Header |
| VBAP  | Sales Order Item   |
| KNA1  | Customer Master    |
| VBUK  | Sales Order Status |

---

## ⚙️ Program Flow

```
START-OF-SELECTION
   ↓
FETCH_DATA
   ↓
PROCESS_DATA (Traffic Light Logic)
   ↓
DISPLAY_ALV
   ↓
USER_COMMAND (Drill-down VA03)
```

---

## 🧠 Key Learnings

* Modular ABAP programming using **FORM routines**
* Efficient data handling using **JOIN operations**
* Implementation of **interactive ALV reports**
* Use of **callback functions** for enhanced UI
* Understanding SAP SD data structure and flow

---

## 🔮 Future Enhancements

* 📥 Export report to Excel
* 📧 Email report functionality
* 📊 Add graphical dashboard
* 🌐 Convert to SAP Fiori app

---
---

## 👨‍💻 Author

**Tushar Ranjan Dash**
Roll No: 2304132
Batch: SAP ABAP 2027

---

## 📚 References

* SAP Help Portal
* ABAP Keyword Documentation
* SAP SD Tables (VBAK, VBAP, KNA1, VBUK)
* KIIT Capstone Project Guidelines

---

## ⭐ Acknowledgment

This project was developed as part of the **KIIT SAP ABAP Capstone Project** to demonstrate real-world enterprise reporting using SAP ABAP.

---
