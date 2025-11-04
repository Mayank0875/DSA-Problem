## Title

Unpaired Inventory Item

## Slug

unpaired-inventory-item

## Difficulty

Medium

## Description

An automated warehouse stores items in pairs on a long, sorted conveyor belt. Each item has a product code. As the items pass a scanner, their codes are read. Every product code should appear twice in a row. One item is missing its partner and appears only once. Find the product code of this single item.

You must write an algorithm with O(log n) runtime complexity.

## Examples

### 1

#### Input

9 
[1, 1, 2, 3, 3, 4, 4, 8, 8]


#### Output

2

#### Explanation

In the sequence [1, 1, 2, 3, 3, 4, 4, 8, 8], the number 2 appears only once.

### 2

#### Input

7 
[3, 3, 7, 7, 10, 11, 11]

#### Output

10

#### Explanation

In the sequence [3, 3, 7, 7, 10, 11, 11], the number 10 appears only once.

## Input Format

- The first line contains an odd integer n, the total number of items.
- The second line contains n space-separated integers representing the sorted product codes.

## Output Format

- Return a single integer: the product code that appears only once.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ stone_value ≤ 10^9
- The array is sorted.
- Every element appears twice except for one.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, array