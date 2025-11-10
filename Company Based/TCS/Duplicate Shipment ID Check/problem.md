## Title

Duplicate Shipment ID Check

## Slug

duplicate-shipment-id-check

## Difficulty

Easy

## Description

A warehouse has just received a large shipment of items. Each item is supposed to have a unique integer ID. However, errors can happen during packing, leading to duplicate IDs in the shipment.

Your job is to write a program that quickly checks the list of item IDs. If any ID appears more than once in the list, the shipment must be flagged for review. You will be given an array of integers representing the item IDs. Determine if any ID appears at least twice.

## Examples

### 1

#### Input

4 
[1, 2, 3, 1]

#### Output

Yes

#### Explanation

The ID `1` appears twice (at the first and last positions).
    
### 2

#### Input

4 
[1, 2, 3, 4]

#### Output

No

#### Explanation

All item IDs in the list are distinct.
  

## Input Format  

- The first line contains a single integer n, the number of items in the shipment.
- The second line contains n space-separated integers, representing the item IDs.

## Output Format  

- Return `Yes` if any item ID appears at least twice in the array,Otherwise `No`.

## Constraints  

- 1 ≤ n ≤ 1e5
- -1e9 ≤ text[i] ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

sorting, array