## Title

Ferris Wheel Gondolas

## Slug

ferris-wheel-gondolas

## Difficulty

Easy

## Description

A group of children wants to ride a Ferris wheel. There are several gondolas available. Each gondola can hold one or two children. Importantly, the total weight of the children in a single gondola cannot exceed a maximum weight limit, x. Given the weights of all the children, your task is to determine the minimum number of gondolas needed to accommodate all of them.

## Examples

### 1

#### Input

4 10 
[7, 2, 3, 9]

#### Output

3

#### Explanation

One way to achieve the minimum is:
    - Gondola 1: Child with weight 2 and child with weight 7 (Total weight 9 <= 10)
    - Gondola 2: Child with weight 3 (Total weight 3 <= 10)
    - Gondola 3: Child with weight 9 (Total weight 9 <= 10)
This requires 3 gondolas.
    
### 2

#### Input

5 5 
[2, 2, 2, 3, 4]

#### Output

3

#### Explanation

One way is:
    - Gondola 1: Child with weight 2 and child with weight 3 (Total weight 5 <= 5)
    - Gondola 2: Child with weight 2 and child with weight 2 (Total weight 4 <= 5)
    - Gondola 3: Child with weight 4 (Total weight 4 <= 5)
This requires 3 gondolas.
  

## Input Format  

- The first line contains two integers n and x: the number of children and the maximum allowed weight per gondola.
- The second line contains n integers p_1, p_2, ..., p_n: the weight of each child.

## Output Format  

- Return a single integer: the minimum number of gondolas required.
  

## Constraints  

- 1 ≤ n ≤ 1e5
- 1 ≤ x ≤ 1e9
- 1 ≤ p_i ≤ x

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

greedy, sorting, two pointers