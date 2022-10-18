# SQL API Pattern

## Intent

Provide a stable, evolvable interface to relational data stored in a data warehouse.

## Problem

Raw data is stored in tables in the data warehouse.
These tables consist of typed columns defined by the table schema.

Changes to the table schema such as dropping columns or changing the type of a column will cause failures in queries referencing those columns.

### Example

Consider this table.

|receipt_timestamp (TIMESTAMP)|id (STRING)|succeeded (INT)|
|-|-|-|
|2022-01-01 12:34:56.789|"384764"|1|
|2022-01-01 23:45:50.123|"246743"|0|

The data source populating this table changes so that the `succeeded` column is a boolean value.
How can we make this new data available to consumers without co-ordinated changes?
Specifically:
- without breaking existing consumer queries?
- without changing the data pipeline that populates the table?

## Solution



## Example

## Checklist

