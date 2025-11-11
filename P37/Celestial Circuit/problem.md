## Title

Celestial Circuit

## Slug

celestial-circuit

## Difficulty

Easy

## Description

An interstellar engineer must produce exactly n additional copies of a crucial star‑map before the spacecraft departs. The original map is already available, and two quantum replicators can be used.  
The first replicator creates one copy in x seconds (it can copy from the original or any existing copy), and the second replicator creates one copy in y seconds. The engineer may operate either replicator alone or both simultaneously.  
Determine the minimum amount of time required to have at least n new copies of the star‑map, starting with just the original.

## Examples

### 1

#### Input

5 1 2

#### Output

4

#### Explanation

We need 5 copies. Assume replicator 1 takes 1 s, replicator 2 takes 2 s.  
    1. Use replicator 1 on the original (1 s elapsed). Now we have 2 maps. Need 4 more.  
    2. Use replicator 1 on the original, replicator 2 on a copy (2 s elapsed total, 1 s more). Replicator 1 finishes. Now have 3 maps. Need 3 more.  
    3. Use replicator 1 on the original (3 s elapsed total, 1 s more). Replicator 2 finishes its first copy. Now have 4 maps. Need 2 more.  
    4. Use replicator 1 on the original, replicator 2 on a copy (4 s elapsed total, 1 s more). Replicator 1 finishes. Now have 5 maps. Need 1 more. Replicator 2 finishes. Now have 6 maps. We have enough copies.  
Minimum time is 4 seconds.

### 2

#### Input

4 1 1

#### Output

3

#### Explanation

Need 4 copies. Both replicators take 1 s.  
    1. Use replicator 1 on the original (1 s). Have 2 maps. Need 3 more.  
    2. Use replicator 1 and 2 on the available maps (2 s). Have 4 maps. Need 1 more.  
    3. Use replicator 1 and 2 again (3 s). Have 6 maps. We have enough.  
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