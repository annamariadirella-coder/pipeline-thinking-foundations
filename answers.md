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

# Scenario 2 — School Attendance Export

## Source
- Two attendance export files generated weekly from two different school systems (likely CSV or Excel files).

## Problems
- Different column names for the same information (e.g., student_name vs name).
- Some class names are missing.
- Dates are written in different formats.
- Some students appear more than once on the same day.
- Data comes from two separate systems, which may create inconsistencies.

## Possible Transformations
- Standardize column names (e.g., rename student_name and name to a unified column such as student_name).
- Merge the two datasets into a single unified attendance table.
- Normalize date formats into a consistent format (e.g., YYYY-MM-DD).
- Remove duplicate records for the same student on the same date.
- Handle missing class names by filling them if possible or flagging them for review.
- Validate data consistency across both systems.

## Expected Output
- A single consolidated attendance dataset.
- Consistent column naming.
- Standardized date format.
- One record per student per day.
- No unnecessary duplicates.
- Clearly handled or flagged missing class information.

# Scenario 3 — Hospital Appointments Data

## Source
- Appointment data coming from three different sources:
  - A web booking system.
  - A receptionist-managed spreadsheet.
  - An internal database export.

## Problems
- Different field names for the same concept (e.g., patient_id vs customer_id).
- Appointment status values are inconsistent (e.g., done, Done, finished).
- Some rows are missing doctor names.
- Duplicate appointments may exist across systems.
- Data structure may vary depending on the source system.

## Possible Transformations
- Map and standardize field names (e.g., unify patient_id and customer_id into patient_id).
- Normalize appointment status values into a consistent set (e.g., Completed, Cancelled, Scheduled).
- Merge all three datasets into a unified appointments table.
- Remove duplicate appointments using a combination of patient ID, date, and time.
- Handle missing doctor names by flagging incomplete records or enriching from another source.
- Validate data consistency and integrity.

## Expected Output
- A single consolidated appointments dataset.
- Consistent field naming.
- Standardized appointment status values.
- No duplicate appointments.
- Complete or clearly flagged records for missing information.
- A clean structure ready for reporting or analytics.
