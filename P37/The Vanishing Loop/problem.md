## Title

The Vanishing Loop

## Slug

the-vanishing-loop

## Difficulty

Easy

## Description

A mysterious loop in the ancient codebase is about to vanish unless it is duplicated enough times before the system reboot. The original loop is present, and you must create exactly **n** additional copies of it before the reboot occurs. Two magical duplicators are at your disposal.
The first duplicator can copy a loop (either the original or any existing copy) in **x** seconds, while the second one needs **y** seconds. You may use either duplicator alone or both of them simultaneously.
Determine the minimum amount of time required to have at least **n** new copies of the loop, starting with only the original.

## Examples

### 1

#### Input

5 1 2

#### Output

4

#### Explanation

We need 5 copies. Assume duplicator 1 takes 1s, duplicator 2 takes 2s.
    1. Use duplicator 1 on the original (1s elapsed). Now we have 2 loops. Need 4 more.
    2. Use duplicator 1 on original, duplicator 2 on a copy (2s elapsed total, 1s more). Duplicator 1 finishes. Now have 3 loops. Need 3 more.
    3. Use duplicator 1 on original (3s elapsed total, 1s more). Duplicator 2 finishes its first copy. Now have 4 loops. Need 2 more.
    4. Use duplicator 1 on original, duplicator 2 on a copy (4s elapsed total, 1s more). Duplicator 1 finishes. Now have 5 loops. Need 1 more. Duplicator 2 finishes. Now have 6 loops. We have enough copies.
Minimum time is 4 seconds.

### 2

#### Input

4 1 1

#### Output

3

#### Explanation

Need 4 copies. Both duplicators take 1s.
    1. Use duplicator 1 on original (1s). Have 2 loops. Need 3 more.
    2. Use duplicator 1 and 2 on the available loops (2s). Have 4 loops. Need 1 more.
    3. Use duplicator 1 and 2 again (3s). Have 6 loops. We have enough.
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