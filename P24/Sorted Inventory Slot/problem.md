## Title

Sorted Inventory Slot

## Slug

sorted-inventory-slot

## Difficulty

Easy

## Description

A warehouse inventory is sorted by item serial numbers. A new item with a `target` serial number arrives and must be placed in its correct slot to maintain the sorted order.

Your task is to find the index where this new item should be placed.
The index should point to the first slot containing an item with a serial number greater than or equal to the new item's.
If all items have smaller numbers, it goes at the end.


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