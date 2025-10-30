## Title

Supply Chain Standardization

## Slug

supply-chain-standardization

## Difficulty

Medium

## Description

A company has N factories. Each factory `i` produces `A[i]` units per day. The company wants to standardize its shipping containers. This requires finding the largest possible container size (a GCD) that can perfectly fit the daily production of all factories. The company can afford to upgrade exactly one factory, changing its production `A[i]` to any new value between 1 and 10⁹. What is the maximum container size (GCD) possible?

## Examples

### 1

#### Input

3 
[7, 6, 8]

#### Output

2

#### Explanation

If the factory producing 7 units is upgraded to produce 4 units, the production levels [4, 6, 8] allow for a standard container size of 2.

### 2

#### Input

2
[100, 100]

#### Output

100

#### Explanation

An "upgrade" can result in the same production level.

## Input Format

- First line: integer 'n' representing the number of elements written on the blackboard .  
- Second line: 'n' integers representing the elements that are written on blackboard.
- You will be given the array as an input to your function

## Output Format

- Return an integer representing the greatest common divisor after making your move.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ arr[i] ≤ 10^9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, prefix sum, suffix sum, math