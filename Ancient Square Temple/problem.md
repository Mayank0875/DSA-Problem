## Title

Ancient Square Temple

## Slug

ancient-square-temple

## Difficulty

Easy

## Description

One day, you are asked by the High Priest to rebuild the outer courtyard of the temple using as many tiles as possible so that the layout still forms a perfect square.

You are given x, the total number of tiles available.
Your task is to determine the maximum possible side length of the square courtyard that can be built using those tiles.

Formally, find the largest integer r such that:
r * r ≤ x

## Examples

### 1

#### Input

10

#### Output
3

#### Explanation
3² = 9 ≤ 10, 4² = 16 > 10    
    


### 2

#### Input

25 

#### Output

5

#### Explanation
5² = 25 ≤ 25, 6² = 36 > 25  
  

## Input Format  

- A single integer x  

## Output Format  

- Return single integer — the integer square root of x.  
  

## Constraints  

- 0 ≤ x ≤ 1e18 

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory