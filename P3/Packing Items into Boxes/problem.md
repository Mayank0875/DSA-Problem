## Title

Packing Items into Boxes

## Slug

packing-items-into-boxes

## Difficulty

Easy

## Description

You are working in a warehouse and need to pack items into delivery boxes. Each box can hold either one or two items. However, there's a strict weight limit, x, for each box. You are given the weights of n items that need to be packed. Your goal is to use the minimum possible number of boxes to pack all the items while adhering to the weight constraint. Find the minimum number of boxes required.

## Examples

### 1

#### Input

4 10
[7, 2, 3, 9]

#### Output

3

#### Explanation

One optimal way to pack is:
    - Box 1: Item with weight 2 and item with weight 7 (Total weight 9 <= 10)
    - Box 2: Item with weight 3 (Total weight 3 <= 10)
    - Box 3: Item with weight 9 (Total weight 9 <= 10)
This requires 3 boxes.

### 2

#### Input

5 5
[2, 2, 2, 3, 4]

#### Output

3

#### Explanation

One optimal way is:
    - Box 1: Item with weight 2 and item with weight 3 (Total weight 5 <= 5)
    - Box 2: Item with weight 2 and item with weight 2 (Total weight 4 <= 5)
    - Box 3: Item with weight 4 (Total weight 4 <= 5)
This requires 3 boxes.

## Input Format

- The first line contains two integers n and x: the number of items and the maximum allowed weight per box.
- The second line contains n integers p_1, p_2, ..., p_n: the weight of each item.

## Output Format

- Return a single integer: the minimum number of boxes required.

## Constraints

- 1 ≤ n ≤ 1e5
- 1 ≤ x ≤ 1e9
- 1 ≤ p_i ≤ x