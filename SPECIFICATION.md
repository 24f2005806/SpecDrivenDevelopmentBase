# CSV Export Feature Specification

## Goal

Provide an endpoint that exports reports as CSV.

## Endpoint

GET /reports/export

## Requirements

1. Export reports in CSV format.
2. Support existing filters.
3. Support existing sorting.
4. Exclude internal_id.
5. Exclude owner_email.
6. Follow RFC4180 CSV rules.
7. Return downloadable file.
8. Content-Type must be text/csv.

## Acceptance Criteria

- CSV downloads successfully.
- Internal fields never appear.
- Commas, quotes and newlines are handled correctly.
- Existing filters work exactly as in /reports.