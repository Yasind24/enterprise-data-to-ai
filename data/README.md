# Synthetic seed data

All records are fictional. The fixture represents a snapshot for a demonstration, not a real utility's data or business rules.

`service_points.csv` has one row per service point. An account may have both electric and gas service points.

## Expected counts

- Active service points: **4**
- Distinct accounts with an active service point: **3**
- Distinct non-test accounts with an active service point: **2**

These counts demonstrate grain and filter differences. No definition is universally correct; business owners must decide what a metric should mean.

The file intentionally stays small so visitors can inspect every record and verify the results.
