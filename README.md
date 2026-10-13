# Campus Bakery POS

A lightweight, desktop-friendly Computer-Based Food Ordering and Point-of-Sale (POS) terminal developed as an individual practical examination project for IT 415. The system allows cashiers to manage orders, validate cash payments, calculate change, and print itemized digital receipts without database or login dependencies.

---

## Menu Catalog & Pricing

| Item # | Product Name | Unit Price (PHP) |
|---|---|---|
| 1 | Pandesal (pack of 5) | ₱25.00 |
| 2 | Ensaymada | ₱20.00 |
| 3 | Spanish Bread | ₱15.00 |
| 4 | Chocolate Cupcake | ₱30.00 |
| 5 | Loaf Bread | ₱55.00 |
| 6 | Brewed Coffee (cup) | ₱25.00 |

---

## Key Features

1. **Product Display:** Renders all six bakery catalog items in a responsive desktop card grid with formatted prices.
2. **Shopping Cart Management:** Adds items to the cart, tracks quantity per product, and prevents duplicate line items.
3. **Quantity Controls:** Real-time increment (`+`) and decrement (`-`) buttons; automatically removes items when reduced to zero, plus a manual remove (`×`) option.
4. **Automatic Order Calculations:** Computes individual line subtotals ($\text{Price} \times \text{Quantity}$) and total bill dynamically.
5. **Cash Payment Validation:**
   - Blocks empty carts from checkout.
   - Rejects blank, non-numeric, or negative tender amounts with clear feedback (`"Please enter a valid payment amount."`).
   - Flags insufficient cash and indicates the exact total needed (`"Insufficient payment. Please enter at least ₱[Total Due]."`).
6. **Change Computation:** Accurate real-time calculation ($\text{Change} = \text{Amount Paid} - \text{Total Due}$) to two decimal places.
7. **Digital Receipt Generation:** Prints an itemized receipt featuring an auto-incrementing transaction reference (`Ref #: TXN-XXXX`), timestamp, breakdown of purchased items, grand total, tender, and change.
8. **Transaction Reset:** Provides a **Start New Order** button that flushes active memory, unlocks inputs, and resets displays for the next customer.

---

## Technology Stack

- **Markup:** HTML5 (Semantic document structure)
- **Styling:** CSS3 (Flexbox and Grid layout for desktop terminals)
- **Scripting:** Vanilla JavaScript (ES6+, in-memory state management, DOM manipulation)
- **Dependencies:** None (Zero external libraries, frameworks, or databases)
- **Version Control:** Git & GitHub

---

## Instructions to Run

1. Clone the repository:
   ```bash
   git clone [https://github.com/](https://github.com/)<YOUR_USERNAME>/CampusBakeryPOS.git
