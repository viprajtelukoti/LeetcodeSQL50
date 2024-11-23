
# 1683. Invalid Tweets

## Table: Tweets

| Column Name    | Type    |
|----------------|---------|
| tweet_id       | int     |
| content        | varchar |

- `tweet_id` is the primary key (unique identifier) for this table.
- This table contains all the tweets in a social media app.

---

## Problem Statement

Write a query to find the IDs of the **invalid tweets**. A tweet is considered invalid if the number of characters in its `content` is **strictly greater than 15**.

### Requirements:
- Return a single column:
  - `tweet_id`: the ID of the invalid tweets.
- The result can be returned in any order.

---

### Example Input:
| tweet_id | content                           |
|----------|-----------------------------------|
| 1        | Let us Code                       |
| 2        | More than fifteen chars are here! |

### Expected Output:
| tweet_id |
|----------|
| 2        |

---

### Explanation:
- Tweet 1 has a length of 11 characters, so it is valid.
- Tweet 2 has a length of 33 characters, so it is invalid.

---

### Difficulty: Easy
