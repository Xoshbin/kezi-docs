---
title: POS Orders
icon: heroicon-o-shopping-bag
order: 3
---


This guide explains how Point of Sale (POS) orders are created, managed, and processed in the system.

---

## What is a POS Order?

A POS Order connects a sale made at the terminal to the backend ERP. It records the products sold, quantities, customer details, and payments received. Unlike a standard Sales Order, a POS order is typically confirmed and paid immediately.

---

## Where to find it in the UI

Navigate to **POS → Operations → Orders**

---

## Order Details

Each POS Order contains the following key information:

### Header Info
- **Order Number**: Unique identifier (e.g., `POS-001-0012`).
- **Session**: The session during which the order was created.
- **Date**: Timestamp of the transaction.
- **Cashier**: The user who processed the order.
- **Customer**: The customer associated with the sale (optional).

### Lines
A list of products or services sold, including:
- **Product Name & SKU**
- **Quantity**
- **Unit Price**
- **Taxes** applied
- **Discounts** (line-level)

### Payments
Records of how the order was paid:
- **Payment Method**: Cash, Bank, Credit Card, etc.
- **Amount**: The amount paid.
- **Change**: Any change given back to the customer.

---

## Order Statuses

- **Draft**: Order is being created (rarely seen in backend unless customized).
- **Paid**: Order is completed and fully paid.
- **Posted/Invoiced**: Order has been converted to an invoice or posted to the ledger.
- **Cancelled**: Order was voided.

---

## Actions on Orders

From the Order list or detail view, you can perform several actions depending on your permissions:

### 1. Invoicing
If a customer requires a formal invoice for a POS transaction:
1. Open the POS Order.
2. Click **Create Invoice**.
3. The system will generate a draft Customer Invoice linked to this order.
4. Process the invoice as per standard accounting flows.

### 2. Explode / Return
To process a return:
1. Navigate to the original order.
2. Select **Return Products**.
3. Select the items and quantities to return.
4. This creates a new "Refund" order (negative quantities) to balance the stock and cash.

### 3. Reprint Receipt
You can reprint a receipt for any past order:
1. Open the Order.
2. Click **Print Receipt**.

---

## Reporting

POS Orders feed into several reports:
- **Sales Details**: Breakdown of sales by product or category.
- **Payment Report**: Summary of payments by method.
- **Tax Report**: Collected taxes from POS sales.

---

## Related Documentation

- [POS Terminal](pos-terminal.md) - How to create orders at the counter.
- [Customer Invoices](customer-invoices.md) - For B2B or formal invoicing.
