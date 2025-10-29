## Title

Counting Unique Product IDs Sold

## Slug

counting-unique-product-ids-sold

## Difficulty

Easy

## Description

An e-commerce platform analyzes its sales records. Each product has a unique numerical ID. The sales log contains the ID of every item sold. Since multiple units of the same product might be sold, a product ID can appear many times in the log. The platform wants to determine how many different types of products were sold during a specific period. Given the list of product IDs from the sales records, find the count of unique product IDs.

## Examples

### 1

#### Input

5
[2, 3, 2, 2, 3]

#### Output

2

#### Explanation

The product IDs sold are 2, 3, 2, 2, 3. The unique IDs are 2 and 3. The platform sold 2 distinct product types.

### 2

#### Input

8
[10, 5, 10, 2, 5, 10, 5, 2]

#### Output

3

#### Explanation

The unique IDs are 10, 5, and 2. The platform sold 3 distinct product types.

## Input Format

- The first line contains an integer n: the total number of items sold.
- The second line contains $n$ integers x_1, x_2, ...., x_n: the product identification codes.

## Output Format

- Return a single integer: the count of distinct product IDs.

## Constraints

- 1 ≤ n ≤ 1e5
- 1 ≤ x_i ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

sorting, set, counting, sales