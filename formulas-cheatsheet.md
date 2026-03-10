# Excel Formulas Cheat Sheet

CGS2512C — Spreadsheet Concepts & Practices | FSCJ Spring 2026

---

## Arithmetic & Basic
```excel
=SUM(A1:A10)
=AVERAGE(B1:B20)
=MIN(C1:C50)
=MAX(C1:C50)
=COUNT(A1:A10)        -- counts numbers only
=COUNTA(A1:A10)       -- counts non-empty cells
=COUNTIF(A1:A10, ">5")
=SUMIF(A1:A10, ">5", B1:B10)
```

## Logical
```excel
=IF(A1>90, "A", "Not A")
=IF(A1>90, "A", IF(A1>80, "B", IF(A1>70, "C", "D")))
=AND(A1>0, A1<100)    -- TRUE only if both conditions met
=OR(A1="Yes", A1="Maybe")
=NOT(A1="No")
```

## Lookup
```excel
=VLOOKUP(lookup_value, table_range, col_index, FALSE)
-- FALSE = exact match (almost always use this)
-- col_index = which column to return (1 = first column)

=INDEX(return_range, MATCH(lookup_value, lookup_range, 0))
-- more flexible than VLOOKUP, works in any direction
```

## Text
```excel
=LEFT(A1, 3)           -- first 3 characters
=RIGHT(A1, 4)          -- last 4 characters
=MID(A1, 2, 5)         -- 5 chars starting at position 2
=LEN(A1)               -- count characters
=TRIM(A1)              -- remove extra spaces
=UPPER(A1)  =LOWER(A1)  =PROPER(A1)
=A1&" "&B1             -- join text with &
=CONCATENATE(A1," ",B1)
```

---
*CGS2512C — Spring 2026*
