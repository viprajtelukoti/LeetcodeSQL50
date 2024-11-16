# Recyclable and Low Fat Products

## Table: Products

| Column Name | Type    |
|-------------|---------|
| product_id  | int     |
| low_fats    | enum    |
| recyclable  | enum    |

- `product_id` is the primary key (column with unique values) for this table.
- `low_fats` is an ENUM (category) of type ('Y', 'N') where 'Y' means this product is low fat and 'N' means it is not.
- `recyclable` is an ENUM (category) of type ('Y', 'N') where 'Y' means this product is recyclable and 'N' means it is not.

---

## Problem Statement

Write a query to find the IDs of products that are **both low fat and recyclable**.

### Example Input:
| product_id  | low_fats | recyclable |
|-------------|----------|------------|
| 0           | Y        | N          |
| 1           | Y        | Y          |
| 2           | N        | Y          |
| 3           | Y        | Y          |
| 4           | N        | N          |

### Expected Output:
| product_id  |
|-------------|
| 1           |
| 3           |

---

### Explanation:
Only products `1` and `3` have both `low_fats = 'Y'` and `recyclable = 'Y'`.

---

### Difficulty: Easy
