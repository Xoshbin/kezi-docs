---
title: POS Profiles
icon: heroicon-o-computer-desktop
order: 1
---


This guide explains how to configure Point of Sale (POS) profiles in your system. POS profiles define the behavior, hardware, and accounting settings for each POS station.

---

## What is a POS Profile?

A POS Profile serves as a configuration template for a specific Point of Sale station or type of operation (e.g., "Main Store Register", "Pop-up Shop", "Restaurant Bar"). It controls:

- **Stock Location**: Where inventory is deducted from.
- **Payment Methods**: Allowed payment types (Cash, Bank, etc.).
- **Accounting**: Default income accounts and journals.
- **Hardware**: Printer and scanner settings.
- **Features**: Receipt customization and other operational settings.

---

## Where to find it in the UI

Navigate to **POS → Configuration → POS Profiles**

---

## Creating a POS Profile

1. Navigate to **POS → Configuration → POS Profiles**.
2. Click **Create POS Profile**.

### Basic Information

- **Name**: A descriptive name for the profile (e.g., "Main Hall Register").
- **Type**: The type of operation (e.g., Retail, Restaurant).
- **Stock Location**: Select the warehouse source location. Stock will be deducted from here when orders are processed.

### Accounting Settings

- **Default Income Account**: The general ledger account where sales revenue will be recorded.
- **Default Payment Journal**: The journal used to record payments received (e.g., Cash Journal, Bank Journal).
- **Company**: The company this profile belongs to (for multi-company environments).

### Features & Settings

Depending on your configuration, you may have options to:
- **Enable/Disable Features**: Toggle specific POS functionalities.
- **Receipt Customization**: Configure header and footer text for printed receipts.
- **Hardware Setup**: Configure IP addresses for network printers or payment terminals.

---

## Best Practices

### 1. One Profile per Physical Station
It is recommended to create a unique profile for each physical POS terminal. This allows for:
- Detailed reporting per station.
- Specific hardware configuration (different printers).
- Easier troubleshooting.

### 2. Separate Stock Locations
If you have multiple stores or distinct areas (e.g., "Front Store" vs. "Back Warehouse"), assign specific stock locations to their respective POS profiles to verify inventory accurately.

### 3. Clear Naming Convention
Use clear and consistent names like "[Branch Name] - [Register Number]" (e.g., "Downtown - Reg 1") to easily identify sources of sales in reports.

---

## Related Documentation

- [POS Sessions](pos-sessions.md) - Learn how to open and close sessions using these profiles.
- [POS Terminal](pos-terminal.md) - User guide for the POS interface.
