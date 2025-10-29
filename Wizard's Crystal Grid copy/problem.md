## Title

Collector's Missing Item

## Slug

collectors-missing-item

## Difficulty

Easy

## Description

A meticulous collector has a prized set of items, uniquely numbered sequentially from 1 to n. While doing inventory, the collector lists all the item numbers currently present. Unfortunately, one item seems to be missing! Given the total number of items the collector should have (n) and the list of numbers for the n-1 items currently present, can you identify the number of the missing item?

## Examples

### 1

#### Input

5 
[2, 3, 1, 5]

#### Output

4

#### Explanation

The collector should have items numbered 1, 2, 3, 4, and 5. The list contains 1, 2, 3, and 5. The missing item number is 4.
    
### 2

#### Input
3 
[1, 3]

#### Output

2

#### Explanation

The collector should have items 1, 2, and 3. The list contains 1 and 3. The missing item is 2.
  

## Input Format  

- The first line contains an integer n: the total number of items the collector should have.
- The second line contains n-1 integers: the numbers of the items present. Each number is distinct and between 1 and n (inclusive).

## Output Format  

- Return a single integer: the number of the missing item.
  

## Constraints  

- 1 ≤ n ≤ 1e5
- Each number in the input list is between 1 and n.
- All numbers in the input list are distinct.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

math, array