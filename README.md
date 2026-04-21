
# 🧾 SAP MM Procure-to-Pay (P2P) Simulation in Python

📌 *KIIT University | SAP Capstone Project 2026*
👩‍💻 **Author:** Saheli Patra
🎓 **Roll No:** 23051293
📦 **Module:** SAP MM (Materials Management)

---

## 📖 Project Overview

This project is a **complete simulation of the SAP Procure-to-Pay (P2P) cycle** implemented in Python.
It mimics real SAP transactions (T-Codes) and demonstrates how procurement and financial processes work in an enterprise system.

Instead of using SAP software, this project recreates the **end-to-end business workflow programmatically**, making it easier to understand the logic behind SAP MM operations.

📄 Source Code: 

---

## 🔄 What is Procure-to-Pay (P2P)?

P2P is a business process that covers everything from:

➡️ Requesting materials
➡️ Purchasing from vendors
➡️ Receiving goods
➡️ Verifying invoices
➡️ Making payments

This project simulates the **entire lifecycle step-by-step**.

---

## ⚙️ Features

✅ Full SAP MM workflow simulation
✅ Realistic T-Code mapping (ME51N, ME21N, MIGO, MIRO, etc.)
✅ Vendor & Material master data
✅ RFQ & quotation comparison
✅ Purchase Order creation & approval
✅ Goods Receipt with stock update
✅ Invoice verification (3-way matching)
✅ Automatic payment processing
✅ FI (Financial Accounting) document generation
✅ Complete audit trail

---

## 🏗️ Workflow (Step-by-Step)

### 1️⃣ Purchase Requisition (ME51N)

* Create request for material
* Approval using ME54N

### 2️⃣ RFQ & Quotation (ME41 / ME47 / ME49)

* Send RFQ to vendors
* Record quotations
* Select best vendor

### 3️⃣ Purchase Order (ME21N)

* Create PO from PR & RFQ
* Release using ME29N

### 4️⃣ Goods Receipt (MIGO)

* Receive goods
* Update inventory
* Generate FI document

### 5️⃣ Invoice Verification (MIRO)

* Perform **3-way matching**:

  * PO vs GR vs Invoice
* Handle variance & blocking

### 6️⃣ Vendor Payment (F110)

* Automatic payment run
* Vendor account clearing

---

## 🧠 Key Concepts Implemented

* 📊 **3-Way Matching** (PO, GR, Invoice)
* 💰 **Financial Accounting Entries (FI Docs)**
* 📦 **Inventory Management**
* 📉 **Price Comparison Logic**
* ⚠️ **Invoice Blocking (Tolerance Check)**
* 🔁 **End-to-End Audit Trail**

---

## 🗂️ Project Structure

```bash
sap_p2p_simulation.py   # Main simulation script
```

---

## ▶️ How to Run

### Step 1: Install Python

Make sure Python 3 is installed

### Step 2: Run the script

```bash
python sap_p2p_simulation.py
```

---

## 📌 Sample Output

The program prints each phase clearly like SAP screens:

```
PHASE 1 — Purchase Requisition
PHASE 2 — RFQ
PHASE 3 — Purchase Order
PHASE 4 — Goods Receipt
PHASE 5 — Invoice Verification
PHASE 6 — Payment
```

At the end, it shows a **complete P2P summary report**.

---

## 🎯 Learning Outcome

By working on this project, you can understand:

* How SAP MM works internally
* Real business procurement flow
* Integration between MM and FI modules
* Enterprise-level transaction handling

---

## 🚀 Future Improvements

* Add GUI (using Flask or Streamlit)
* Connect to real database
* Add multiple materials & vendors
* Create dashboard for analytics

---

