# 584. Find Customer Referee

## Table: Customer

| Column Name | Type    |
|-------------|---------|
| id          | int     |
| name        | varchar |
| referee_id  | int     |

- `id` is the primary key column for this table.
- Each row of this table indicates the `id` of a customer, their `name`, and the `id` of the customer who referred them.

---

## Problem Statement

Write a query to find the **names of customers who are not referred by the customer with `id = 2`.**

### Example Input:
| id | name | referee_id |
|----|------|------------|
| 1  | Will | null       |
| 2  | Jane | null       |
| 3  | Alex | 2          |
| 4  | Bill | null       |
| 5  | Zack | 1          |
| 6  | Mark | 2          |

### Expected Output:
| name |
|------|
| Will |
| Jane |
| Bill |
| Zack |

---

### Explanation:
- Customers `Alex` and `Mark` are referred by the customer with `id = 2`, so they are excluded.
- All other customers (`Will`, `Jane`, `Bill`, and `Zack`) either have no referee or are referred by someone else.

---

### Difficulty: Easy
