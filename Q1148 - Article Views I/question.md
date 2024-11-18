# 1148. Article Views I

## Table: Views

| Column Name   | Type    |
|---------------|---------|
| article_id    | int     |
| author_id     | int     |
| viewer_id     | int     |
| view_date     | date    |

- This table does not have a primary key (i.e., duplicate rows are possible).
- Each row indicates that a `viewer` viewed an article written by an `author` on a specific `view_date`.
- **Note**: If `author_id` equals `viewer_id`, it means the author viewed their own article.

---

## Problem Statement

Write a query to find the **authors** who viewed at least one of their own articles.

### Requirements:
- Return a single column:
  - `id`: the `author_id` of authors who viewed their own articles.
- Sort the results in ascending order by `id`.

---

### Example Input:
| article_id | author_id | viewer_id | view_date  |
|------------|-----------|-----------|------------|
| 1          | 3         | 5         | 2019-08-01 |
| 1          | 3         | 6         | 2019-08-02 |
| 2          | 7         | 7         | 2019-08-01 |
| 2          | 7         | 6         | 2019-08-02 |
| 4          | 7         | 1         | 2019-07-22 |
| 3          | 4         | 4         | 2019-07-21 |
| 3          | 4         | 4         | 2019-07-21 |

### Expected Output:
| id   |
|------|
| 4    |
| 7    |

---

### Explanation:
- Author `7` viewed their own article on `2019-08-01`.
- Author `4` viewed their own article on `2019-07-21`.
- Author `3` did not view their own articles, so they are excluded.

---

### Difficulty: Easy
