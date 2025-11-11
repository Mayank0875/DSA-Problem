## Title

Synthetic Sequence

## Slug

synthetic-sequence

## Difficulty

Easy

## Description

A researcher needs to synthesize a new sequence of DNA fragments! The lab has the original fragment and must create exactly n additional copies before the experiment begins. There are two synthetic generators available.
The first generator takes x seconds to produce one fragment (from the original or another copy), and the second generator takes y seconds. The researchers can use either generator or both simultaneously. 
Help the researcher determine the minimum amount of time required to produce at least n new copies of the fragment, starting with just the original.


## Examples

### 1

#### Input

5 1 2

#### Output

4

#### Explanation

We need 5 copies. Assume generator 1 takes 1s, generator 2 takes 2s.
    1. Use generator 1 on the original (1s elapsed). Now we have 2 fragments. Need 4 more.
    2. Use generator 1 on original, generator 2 on copy (2s elapsed total, 1s more). Generator 1 finishes. Now have 3 fragments. Need 3 more.
    3. Use generator 1 on original (3s elapsed total, 1s more). Generator 2 finishes its first copy. Now have 4 fragments. Need 2 more.
    4. Use generator 1 on original, generator 2 on a copy (4s elapsed total, 1s more). Generator 1 finishes. Now have 5 fragments. Need 1 more. Generator 2 finishes. Now have 6 fragments. We have enough copies.
Minimum time is 4 seconds.

### 2

#### Input

4 1 1

#### Output

3

#### Explanation

Need 4 copies. Both generators take 1s.
    1. Use generator 1 on original (1s). Have 2 fragments. Need 3 more.
    2. Use generator 1 and 2 on the available fragments (2s). Have 4 fragments. Need 1 more.
    3. Use generator 1 and 2 again (3s). Have 6 fragments. We have enough.
Minimum time is 3 seconds.
  
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