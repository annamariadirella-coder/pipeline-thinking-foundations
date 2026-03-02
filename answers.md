# Scenario 1 — Online Orders CSV

## Source
- A daily CSV file containing online order data exported from the company’s e-commerce system.

## Problems
- Some rows are duplicated, which can lead to incorrect sales reporting.
- City names are inconsistent (e.g., berlin, Berlin, BERLIN).
- Some order amounts are missing.
- Some customer names contain extra spaces.

## Possible Transformations
- Remove duplicate rows based on order ID.
- Standardize city names (e.g., capitalize properly or convert to a consistent format).
- Handle missing amounts by either removing those rows or flagging them for review.
- Trim leading and trailing spaces from customer names.
- Validate that numeric fields (like amount) contain valid values.

## Expected Output
- A clean dataset with one row per order.
- Standardized city names.
- No unnecessary duplicates.
- Valid and consistent amount values.
- Clean customer name formatting.
