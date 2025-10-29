## Title

Unique Ingredients Inventory Check

## Slug

unique-ingredients-inventory-check

## Difficulty

Easy

## Description

A chef is checking the inventory of ingredients in the pantry. Each ingredient type is assigned a unique numerical code. The inventory list might contain multiple entries for the same ingredient if it was restocked or recorded multiple times. The chef needs to know the number of different types of ingredients currently available. Given the complete list of ingredient codes from the inventory, calculate the count of unique ingredient types.

## Examples

### 1

#### Input

5
[2, 3, 2, 2, 3]

#### Output

2

#### Explanation

The ingredient codes are 2, 3, 2, 2, 3. The unique codes are 2 and 3. There are 2 distinct ingredient types.

### 2

#### Input

8
[10, 5, 10, 2, 5, 10, 5, 2]

#### Output

3

#### Explanation

The unique codes are 10, 5, and 2. There are 3 distinct ingredient types.

## Input Format

- The first line contains an integer n: the total number of ingredient entries in the list.
- The second line contains $n$ integers x_1, x_2, ...., x_n: the ingredient identification codes.

## Output Format

- Return a single integer: the count of distinct ingredient codes.

## Constraints

- 1 ≤ n ≤ 1e5
- 1 ≤ x_i ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

sorting, set, counting, inventory