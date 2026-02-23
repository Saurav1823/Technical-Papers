# Aggregations and Filters in Database Queries

## Introduction

Aggregations and filters are important concepts in database queries. They are used to summarize data and retrieve specific records based on conditions.

These operations help in analyzing data and generating meaningful insights from large datasets.

---

## Aggregation in Queries

Aggregation is used to perform calculations on multiple rows of data and return a single summarized value.

Aggregation functions are commonly used in reporting and data analysis.

---

## Common Aggregate Functions

- COUNT – Returns the number of records
- SUM – Returns the total of a numeric column
- AVG – Returns the average value
- MIN – Returns the smallest value
- MAX – Returns the largest value

---

## Importance of Aggregation

Aggregation helps in:

- Summarizing large datasets
- Generating reports
- Performing statistical analysis
- Supporting decision-making

It converts detailed data into meaningful summary information.

---

## GROUP BY Clause

The GROUP BY clause is used with aggregation functions to group rows that have the same values in specified columns.

### Key Points

- Divides data into groups
- Applies aggregate function to each group
- Used for category-wise analysis

---

## Filters in Queries

Filters are used to retrieve only the records that satisfy specific conditions.

Filtering helps in narrowing down large datasets to relevant information.

---

## WHERE Clause

The WHERE clause is used to filter records before aggregation.

### Key Points

- Applies conditions to rows
- Reduces dataset size
- Used with comparison and logical operators

---

## HAVING Clause

The HAVING clause is used to filter grouped data after aggregation.

### Key Points

- Used with GROUP BY
- Filters aggregated results
- Applied after aggregation process

---

## Difference Between WHERE and HAVING

- WHERE filters rows before grouping
- HAVING filters groups after aggregation
- WHERE cannot use aggregate functions directly
- HAVING is used with aggregate functions

---

## Advantages of Using Aggregations and Filters

- Efficient data analysis
- Simplifies complex datasets
- Improves query performance
- Supports business intelligence reporting

---

