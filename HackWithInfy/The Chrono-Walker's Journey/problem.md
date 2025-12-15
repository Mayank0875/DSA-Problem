## Title

The Chrono-Walker's Journey

## Slug

the-chrono-walkers-journey

## Difficulty

Medium

## Description

It is the year 3055. Humans have found ancient Time Gates spread across multiple dimensions. You are a Chrono-Walker, and your job is to travel through these dimensions and reach the “Origin Point.”

There are n dimensions numbered from 1 to n.
    1. Dimension 1 is where your journey begins.
    2. Dimension n is your final destination.

Between some dimensions, there are one-way Time Gates that let you teleport forward. Because of strict time-travel rules, this network has no loops — you can never return to a previous dimension, so the system forms a directed acyclic graph.

Your task is to find how many different ways you can travel from dimension 1 to dimension n by following these one-way gates. Since the number of possible paths can be extremely large, return the count modulo 1000000007.

## Examples

### 1

#### Input

4 5
1 2
2 4
1 3
3 4
1 4


#### Output

3

#### Explanation

There are 3 distinct timelines (paths).
    
### 2

#### Input

4 5
1 2
3 4
2 3
1 3
2 4

#### Output

3

#### Explanation

There are 3 distinct timelines (paths).


## Input Format  

- The first line contains two integers n and m: the number of dimensions and the number of Time Gates.
- The next m lines each contain two integers u and v, representing a Time Gate from dimension u to dimension v.

## Output Format  

- Return a single integer: the number of ways to travel from dimension 1 to dimension n, modulo (1e9 + 7).
  

## Constraints  

- 1 ≤ n ≤ 1e5
- 1 ≤ m ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit

2 second

## Memory Limit

256 MB

## Tags
graph, dynamic-programming, hackwithinfy

## Companies
infosys