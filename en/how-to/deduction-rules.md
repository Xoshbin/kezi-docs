---
title: Managing Deduction Rules
icon: heroicon-o-variable
---

# How-to: Manage Deduction Rules

Deduction rules allow you to automate the calculation of taxes, social security, and other employee contributions during the payroll process.

### What are Deduction Rules?

In plain English, a deduction rule is an instruction for the system to automatically take away a specific amount from an employee's gross salary. These can be:
- **Percentage**: A portion of the gross salary (e.g., 5% for Social Security).
- **Fixed Amount**: A specific dollar or dinar amount (e.g., $50 for a specific fund).

---

### Step 1: Accessing Deduction Rules

1. Navigate to **Human Resources → Deduction Rules**.
2. Here you will see a list of all existing rules and their current status.

---

### Step 2: Creating a New Rule

1. Click **New Deduction Rule**.
2. **Name**: Give the rule a clear name (e.g., "Income Tax").
3. **Code**: (Optional) Use a unique code if you need to map this to specific accounting reports.
4. **Deduction Type**:
    - Choose **Percentage** to calculate based on a percentage of the total salary.
    - Choose **Fixed Amount** to deduct a set value regardless of the salary amount.
5. **Value/Amount**: Enter the percentage (e.g., 0.05 for 5%) or the fixed amount.
6. **Liability Account**: Select the accounting account where these deducted funds should be recorded until they are paid to the authority.
7. **Is Statutory**: Check this if the deduction is required by law (e.g., government taxes).
8. **Is Active**: Ensure this is checked for the rule to be applied in the next payroll run.

---

### Step 3: How Rules are Applied

When you [Process Payroll](process-payroll.md), the system automatically:
1. Fetches all **Active** deduction rules for your company.
2. Calculates the amount based on the employee's gross salary.
3. subtracts the total from the Gross Salary to reach the **Net Salary**.
4. Creates a corresponding liability in your accounting records.

---

### Troubleshooting & FAQs

**Q: Why isn't a rule being applied to my payroll?**
A: Ensure the rule is marked as **Active**. Also, remember that rules only apply to payrolls created *after* the rule was activated.

**Q: Can I have different rules for different employees?**
A: Currently, rules are applied company-wide. If you need specific deductions for one employee, you can add them manually as an adjustment on their payroll record.

---

### Related Resources
- [How-to: Process Payroll](process-payroll.md)
- [Explanation: Payroll Workflows](../explanation/payroll-workflows.md)
- [Reference: Payroll Statuses and Accounting](../reference/payroll-statuses-and-accounting.md)
