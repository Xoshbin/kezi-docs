---
title: POS Terminal
icon: heroicon-o-computer-desktop
order: 4
---


This guide explains how to use the Point of Sale (POS) Terminal interface for daily operations.

---

## Interface Overview

The POS Terminal is designed for speed and ease of use. It consists of three main areas:

1. **Product Grid (Center)**: Browse and search for products.
2. **Category Sidebar (Left)**: Filter products by category for quick access.
3. **Cart & Action Panel (Right)**: View selected items, manage customers, and process payments.

---

## Basic Workflow

### 1. Adding Items
- **Click**: Tap any product card in the grid to add it to the cart.
- **Search**: Type in the search bar (or press `F2`) to find products by name or SKU.
- **Scan**: Use a barcode scanner to instantly add items. If scanned again, the quantity increases.

### 2. Managing the Cart
- **Quantity**: Use the `+` and `-` buttons on a cart item to adjust quantity.
- **Remove**: Click the trash icon or decrease quantity to 0 to remove an item.
- **Discount**: Click the tag icon on an item to apply a line-level discount (percentage or fixed amount).
- **Clear Cart**: Click the trash icon at the top of the cart (or press `F8`) to remove all items.

### 3. Selecting a Customer
- Click the **Customer** button in the cart panel.
- Search for an existing customer or create a new one.
- Assigning a customer is optional for walk-in clients but required for invoicing or loyalty points.

### 4. Payment
1. Click **Confirm & Pay** (or press `F4`).
2. Select the **Payment Method** (Cash, Card, etc.).
3. Enter the **Amount Tendered** (for Cash).
    - Use slight shortcut buttons for common amounts (e.g., $10, $20, Exact).
4. The system calculates **Change Due**.
5. Click **Validate** to complete the sale.

### 5. Completion
- A success screen appears with the change due.
- **Print Receipt**: Click to print.
- **New Order**: Click `New Order` (or press `ESC`) to start the next transaction.

---

## Global Order Discount
You can apply a discount to the entire order:
1. Click **Add Order Discount** in the totals section.
2. Enter the percentage.
3. Apply to deduct from the total.

---

## Keyboard Shortcuts

Power users can navigate functionality quickly using keyboard shortcuts:

| Key | Action |
| :--- | :--- |
| **F2** | Focus Search Bar |
| **F4** | Open Payment Modal |
| **F8** | Clear Cart |
| **F9** | Toggle Order History |
| **F10** | Close Session |
| **Esc** | Close Modals / New Order |

---

## Offline Mode

The POS is designed to work offline. If the internet connection is lost:
- The status indicator turns **Offline**.
- You can continue to process orders.
- Orders are saved locally in the browser.
- When connection is restored, the POS automatically syncs all stored orders to the server.

---

## Order History

Need to check a recent sale?
- Click the **History** icon (clock) or press `F9`.
- View the list of recent orders processed in this session.
- You can reprint receipts from this panel.

---

## Related Documentation

- [POS Sessions](pos-sessions.md) - Opening and closing your shift.
- [POS Orders](pos-orders.md) - Backend management of orders.
