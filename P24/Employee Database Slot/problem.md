## Title

Employee Database Slot

## Slug

employee-database-slot

## Difficulty

Easy

## Description

An employee database is sorted by employee ID number. A new employee with ID `target` is hired and must be inserted into the sorted list.

Your task is to determine the index where this new employee's record should be inserted.
The index should point to the first employee in the list with an ID greater than or equal to `target`.
If all current employee IDs are smaller, the new record is added at the end.


## Examples

### 1

#### Input

6 8
[2, 5, 7, 8, 11, 12]


#### Output

3

#### Explanation

The first product with an ID greater than or equal to 8 is at index 3.

### 2

#### Input

6 6
[2, 5, 7, 8, 11, 12]

#### Output

2

#### Explanation

No product has an ID equal to 6.
The first product with a larger ID (7) appears at index 2.

## Input Format

- The first line contains two integers n and target, where n = number of product IDs, and target = ID of the new product.
- The second line contains n space-separated integers — the sorted list of product IDs.

## Output Format

- Return a single integer — the index where the new product should be inserted.



## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ product_id, target ≤ 10^9
- The IDs are sorted in non-decreasing order.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, array, searching