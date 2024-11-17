# 595. Big Countries

## Table: World

| Column Name | Type    |
|-------------|---------|
| name        | varchar |
| continent   | varchar |
| area        | int     |
| population  | int     |
| gdp         | bigint  |

- `name` is the primary key (column with unique values) for this table.
- Each row provides information about the `name` of a country, the continent it belongs to, its `area`, `population`, and `GDP`.

---

## Problem Statement

A country is considered **big** if:
1. It has an area of at least **three million** (`3000000 km²`), OR
2. It has a population of at least **twenty-five million** (`25000000`).

Write a query to find the **name**, **population**, and **area** of the big countries.

### Example Input:
| name        | continent | area    | population | gdp          |
|-------------|-----------|---------|------------|--------------|
| Afghanistan | Asia      | 652230  | 25500100   | 20343000000  |
| Albania     | Europe    | 28748   | 2831741    | 12960000000  |
| Algeria     | Africa    | 2381741 | 37100000   | 188681000000 |
| Andorra     | Europe    | 468     | 78115      | 3712000000   |
| Angola      | Africa    | 1246700 | 20609294   | 100990000000 |

### Expected Output:
| name        | population | area    |
|-------------|------------|---------|
| Afghanistan | 25500100   | 652230  |
| Algeria     | 37100000   | 2381741 |

---

### Explanation:
- Afghanistan qualifies as a big country because its population exceeds **25 million**.
- Algeria qualifies because its population exceeds **25 million**, and its area is close to the **3 million** threshold.
- Other countries do not meet either criterion.

---

### Difficulty: Easy
