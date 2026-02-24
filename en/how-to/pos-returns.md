---
title: POS Returns
icon: heroicon-o-arrow-uturn-left
order: 4
---

This guide explains how to manage product returns made at the Point of Sale terminal, including the approval workflow and how returns are integrated with inventory and accounting.

---

## What is a POS Return?

A POS Return records the process of a customer returning one or more items from a previously completed sale. It handles:

- **Refund issuance** to the customer (cash, bank, or original payment method)
- **Inventory restocking** (returning items to the warehouse)
- **Accounting entries** (credit note + payment reversal)

---

## Where to find it in the UI

Navigate to **POS → Operations → Returns**

---

## Return Statuses

| Status | Description |
|--------|-------------|
| **Draft** | Return has been created but not yet submitted |
| **Pending Approval** | Return is awaiting manager approval |
| **Approved** | Return has been approved and is ready to process |
| **Processing** | Return is currently being processed |
| **Completed** | Return has been fully processed with refund issued and stock updated |
| **Rejected** | Return was rejected by a manager |
| **Cancelled** | Return was cancelled before processing |

---

## Return Workflow

```
Draft → Pending Approval → Approved → Completed
                         ↘ Rejected
```

1. **Created** at the POS terminal or backend.
2. **Submitted** for manager approval (if the return policy requires it).
3. **Approved** (or rejected) by an authorized user.
4. **Processed** — automatically creates:
   - A **Credit Note** (negative invoice) in the accounting module
   - A **Payment Reversal** (outbound payment refund)
   - A **Stock Move** to restock returned items (if applicable)

---

## Return Details

Each POS Return contains:

### Header Info
- **Return Number**: Unique identifier (e.g., `RET-0001`)
- **Original Order**: The POS order the return is based on
- **Return Date**: When the return was initiated
- **Status**: Current workflow state
- **Refund Amount**: Total amount to be refunded
- **Refund Method**: How the customer is refunded (cash, bank, etc.)

### Return Lines
Each line corresponds to an item being returned:
- **Product**
- **Quantity Returned**
- **Unit Price** (from original order)
- **Line Refund Amount**
- **Condition**: good, opened, damaged, defective
- **Restock**: whether the item will be returned to inventory

### Accounting Integration
Once processed, the return links to:
- **Credit Note** — a negative invoice reversing the original sale
- **Payment Reversal** — an outbound payment confirming the refund
- **Stock Move** — records items returning to inventory

---

## Actions

From the **View** page of a return, authorized users can:

### Approve Return
- Available when status is **Pending Approval**
- Records the approving user and timestamp
- Moves status to **Approved**

### Reject Return
- Available when status is **Pending Approval**
- Requires a rejection reason
- The reason is appended to the return notes

### Process Return
- Available when status is **Approved**
- Triggers the complete processing pipeline:
  1. Creates a credit note (posted immediately)
  2. Creates a payment reversal (confirmed immediately)
  3. Creates stock moves for items marked for restocking

---

## Related Documentation

- [POS Orders](pos-orders.md) — View the original orders
- [POS Sessions](pos-sessions.md) — Manage cashier sessions
