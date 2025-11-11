## Title

Chrono Pattern

## Slug

chrono-pattern

## Difficulty

Easy

## Description

A chronomancer must generate exactly **n** additional temporal patterns before the hourglass runs out. He starts with a single original pattern and has two magical forges at his disposal.  
The first forge can produce a copy of any existing pattern in **x** seconds, and the second forge does the same in **y** seconds. The forges may be used independently or simultaneously, and each can copy from either the original pattern or any copy already created.  

Help the chronomancer determine the minimum amount of time required to have at least **n** new patterns, starting with just the original one.

## Examples

### 1

#### Input

5 1 2

#### Output

4

#### Explanation

We need 5 copies. Assume forge 1 takes 1 s, forge 2 takes 2 s.
    1. Use forge 1 on the original (1 s elapsed). Now we have 2 patterns. Need 4 more.
    2. Use forge 1 on original, forge 2 on a copy (2 s elapsed total, 1 s more). Forge 1 finishes. Now have 3 patterns. Need 3 more.
    3. Use forge 1 on original (3 s elapsed total, 1 s more). Forge 2 finishes its first copy. Now have 4 patterns. Need 2 more.
    4. Use forge 1 on original, forge 2 on a copy (4 s elapsed total, 1 s more). Forge 1 finishes. Now have 5 patterns. Need 1 more. Forge 2 finishes. Now have 6 patterns. We have enough copies.
Minimum time is 4 seconds.

### 2

#### Input

4 1 1

#### Output

3

#### Explanation

Need 4 copies. Both forges take 1 s.
    1. Use forge 1 on original (1 s). Have 2 patterns. Need 3 more.
    2. Use forge 1 and 2 on the available patterns (2 s). Have 4 patterns. Need 1 more.
    3. Use forge 1 and 2 again (3 s). Have 6 patterns. We have enough.
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