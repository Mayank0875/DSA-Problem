## Title

Warehouse Inventory Check

## Slug

warehouse-inventory-check

## Difficulty

Easy

## Description

You are managing a warehouse. All product SKUs are stored in a sorted master list. A worker scans a product with a `target` SKU, and your system must instantly check if this product is in the master list. Create a function that takes the sorted list of SKUs and the target SKU. It must efficiently confirm if the product exists in the inventory. You must write an algorithm with O(log n) runtime complexity.

## Examples

### 1

#### Input

6 8
[2, 5, 7, 8, 11, 12]


#### Output

1

#### Explanation

The target ID 8 is found in the list of grimoire IDs.

### 2

#### Input

6 6
[2, 5, 7, 8, 11, 12]

#### Output

0

#### Explanation

The target ID 6 is not found in the list.

## Input Format

- The first line contains an integers n and target , the number of grimoires and the ID of the grimoire to find. 
- The second line contains n space-separated integers representing the sorted grimoire IDs.

## Output Format

- Return 1 if the target is found, and 0 otherwise.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ grimoire_id, target ≤ 10^9
- The grimoire IDs are sorted in non-decreasing order.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, array, searching