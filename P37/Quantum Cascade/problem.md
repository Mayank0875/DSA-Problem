## Title

Quantum Cascade

## Slug

quantum-cascade

## Difficulty

Easy

## Description

A research lab needs to generate more copies of a delicate quantum state! The lead scientist has the original state and must produce exactly n additional copies before the experiment begins. There are two quantum cascade devices available.  
The first device takes x seconds to clone one quantum state (from the original or another copy), and the second device takes y seconds. The scientists can use either device or both simultaneously.  
Help the lead scientist determine the minimum amount of time required to produce at least n new copies of the quantum state, starting with just the original.

## Examples

### 1

#### Input

5 1 2

#### Output

4

#### Explanation

We need 5 copies. Assume device 1 takes 1 s, device 2 takes 2 s.  
    1. Use device 1 on the original (1 s elapsed). Now we have 2 states. Need 4 more.  
    2. Use device 1 on original, device 2 on a copy (2 s elapsed total, 1 s more). Device 1 finishes. Now have 3 states. Need 3 more.  
    3. Use device 1 on original (3 s elapsed total, 1 s more). Device 2 finishes its first copy. Now have 4 states. Need 2 more.  
    4. Use device 1 on original, device 2 on a copy (4 s elapsed total, 1 s more). Device 1 finishes. Now have 5 states. Need 1 more. Device 2 finishes. Now have 6 states. We have enough copies.  
Minimum time is 4 seconds.

### 2

#### Input

4 1 1

#### Output

3

#### Explanation

Need 4 copies. Both devices take 1 s.  
    1. Use device 1 on original (1 s). Have 2 states. Need 3 more.  
    2. Use device 1 and 2 on the available states (2 s). Have 4 states. Need 1 more.  
    3. Use device 1 and 2 again (3 s). Have 6 states. We have enough.  
Minimum time is 3 seconds.
  
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