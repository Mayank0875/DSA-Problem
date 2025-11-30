## Title

Warehouse Box Shuffling

## Slug

warehouse-box-shuffling

## Difficulty

Medium

## Description

You are working in a warehouse managing a conveyor belt represented by an array of numbers. Each number is an item ID. However, the ID `0` represents an empty spot, not an item. Your task is to reorganize the conveyor belt. You must move all the empty spots (the zeros) to the end of the belt. The actual items (non-zero IDs) must stay in their original relative order. You must do this by modifying the belt in-place, without using a second conveyor belt (no extra array). This ensures the items are grouped together at the front for processing.

## Examples

### 1

#### Input

5 
[0, 1, 0, 3, 12]

#### Output

[1, 3, 12, 0, 0]

#### Explanation

The items 1, 3, and 12 are moved to the front while maintaining their relative order. The two empty spots (0s) are moved to the end.
    
### 2

#### Input

1
[0]

#### Output

[0]

#### Explanation

The belt only has one empty spot, which is already at the end.
  

## Input Format  

- The first line contains a single integer n, the number of positions on the conveyor belt.
- The second line contains n space-separated integers, nums_i, representing the item IDs or empty spots at each position.

## Output Format  

- Return array containing the n integers in their modified order.
  

## Constraints  

- 1 ≤ n ≤ 1e4
- -1e9 ≤ value[i] ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

array

## Companies
infosys