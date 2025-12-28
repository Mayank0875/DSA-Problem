## Title
Warehouse Inventory Check

## Slug
warehouse-inventory-check

## Difficulty
Easy

## Description
A warehouse manager is auditing a shipment. Each box has a unique tracking number. If a number appears twice, it indicates a scanning error or a duplicate shipment.

Your task is to determine if any tracking number appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The tracking number `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All tracking numbers are distinct.

## Input Format
- The first line contains a single integer n, the number of boxes.
- The second line contains n space-separated integers, representing the tracking numbers.

## Output Format
- Return `Yes` if any tracking number appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
