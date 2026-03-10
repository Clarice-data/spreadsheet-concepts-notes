# Key Concepts

CGS2512C — Spreadsheet Concepts & Practices | FSCJ Spring 2026

---

## Absolute vs. Relative References

| Reference | Behavior when copied |
|---|---|
| `A1` | Moves with the formula |
| `$A$1` | Locks both row and column |
| `$A1` | Locks column only |
| `A$1` | Locks row only |

> Use `$` when you need a formula to always point to the same cell —
> like a tax rate or conversion factor stored in one place.

---

## Format ≠ Value
Formatting a cell as currency, percentage, or date doesn't change what's
actually stored in it. Formulas see the raw number, not the display format.

> Example: A cell showing "$5.00" still contains 5. A cell showing "50%"
> contains 0.5.

---

## Tables (Ctrl+T)
Converting data to a Table makes everything better:
- Formulas auto-expand when you add new rows
- Filtering is built in
- Column references become readable names (e.g. `[@Sales]` instead of `C2`)
- PivotTables based on a Table update automatically

> Golden rule: If your data has headers and will grow over time, make it a Table.

---

## Data Validation
Used to control what can be entered in a cell:
- Drop-down lists (restrict to preset options)
- Number ranges (only allow values between X and Y)
- Date ranges
- Custom formulas

> Find it under: Data → Data Validation

---
*CGS2512C — Spring 2026*
