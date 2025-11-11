## Title

Spectral Array

## Slug

spectral-array

## Difficulty

Easy

## Description

A physicist is assembling a **spectral array** of light patterns. The lab has a single original pattern and needs to generate exactly **n** additional patterns before the experiment begins. There are two spectral emitters available.

The first emitter can produce a new pattern from any existing one in **x** seconds, and the second emitter can do the same in **y** seconds. The physicist may use either emitter alone or both simultaneously.

Determine the minimum amount of time required to obtain at least **n** new patterns, starting with only the original pattern.

## Examples

### 1

#### Input

5 1 2

#### Output

4

#### Explanation

We need 5 copies. Assume emitter 1 takes 1s, emitter 2 takes 2s.
    1. Use emitter 1 on the original (1s elapsed). Now we have 2 patterns. Need 4 more.
    2. Use emitter 1 on original, emitter 2 on a copy (2s elapsed total, 1s more). Emitter 1 finishes. Now have 3 patterns. Need 3 more.
    3. Use emitter 1 on original (3s elapsed total, 1s more). Emitter 2 finishes its first copy. Now have 4 patterns. Need 2 more.
    4. Use emitter 1 on original, emitter 2 on a copy (4s elapsed total, 1s more). Emitter 1 finishes. Now have 5 patterns. Need 1 more. Emitter 2 finishes. Now have 6 patterns. We have enough copies.
Minimum time is 4 seconds.

### 2

#### Input

4 1 1

#### Output

3

#### Explanation

Need 4 copies. Both emitters take 1s.
    1. Use emitter 1 on original (1s). Have 2 patterns. Need 3 more.
    2. Use emitter 1 and 2 on the available patterns (2s). Have 4 patterns. Need 1 more.
    3. Use emitter 1 and 2 again (3s). Have 6 patterns. We have enough.
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