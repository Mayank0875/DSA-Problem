## Title

Infinite Loopstorm

## Slug

infinite-loopstorm

## Difficulty

Easy

## Description

A massive loopstorm is raging, and the control center must generate exactly n additional energy loops before the storm subsides. The chief engineer has a single initial loop and can use two loop generators.
The first generator creates one loop in x seconds (it can work on the original loop or any already‑generated loop), and the second generator creates one loop in y seconds. Both generators may be used simultaneously or individually.  
Determine the minimum amount of time required to produce at least n new loops, starting with just the original loop.

## Examples

### 1

#### Input

5 1 2

#### Output

4

#### Explanation

We need 5 loops. Assume generator 1 takes 1 s, generator 2 takes 2 s.
    1. Use generator 1 on the original (1 s elapsed). Now we have 2 loops. Need 4 more.
    2. Use generator 1 on original, generator 2 on a loop (2 s elapsed total, 1 s more). Generator 1 finishes. Now have 3 loops. Need 3 more.
    3. Use generator 1 on original (3 s elapsed total, 1 s more). Generator 2 finishes its first loop. Now have 4 loops. Need 2 more.
    4. Use generator 1 on original, generator 2 on a loop (4 s elapsed total, 1 s more). Generator 1 finishes. Now have 5 loops. Need 1 more. Generator 2 finishes. Now have 6 loops. We have enough loops.
Minimum time is 4 seconds.

### 2

#### Input

4 1 1

#### Output

3

#### Explanation

Need 4 loops. Both generators take 1 s.
    1. Use generator 1 on original (1 s). Have 2 loops. Need 3 more.
    2. Use generator 1 and 2 on the available loops (2 s). Have 4 loops. Need 1 more.
    3. Use generator 1 and 2 again (3 s). Have 6 loops. We have enough.
Minimum time is 3 seconds.
  
## Input Format  

- Three space-separated integers n, x, and y.

## Output Format  

- Return single integer representing the minimum time in seconds required.
  

## Constraints  

- 1 ≤ n ≤ 1e8
- 1 ≤ x, y ≤ 10

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

binary-search, math, number-theory