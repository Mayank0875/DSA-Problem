## Title

Temporal Code

## Slug

temporal-code

## Difficulty

Easy

## Description

A time‑traveling programmer has a single original snippet of a temporal code and must create exactly **n** additional versions before the chronal reset begins. Two time‑shifting duplicators are available.
The first duplicator needs **x** seconds to duplicate one snippet (whether from the original or any copy), and the second needs **y** seconds. The programmer can operate either duplicator or both at the same time.  
Help determine the minimum amount of time required to produce at least **n** new versions of the code, starting with just the original snippet.

## Examples

### 1

#### Input

5 1 2

#### Output

4

#### Explanation

We need 5 copies. Assume duplicator 1 takes 1 s, duplicator 2 takes 2 s.
    1. Use duplicator 1 on the original (1 s elapsed). Now we have 2 snippets. Need 4 more.
    2. Use duplicator 1 on original, duplicator 2 on a copy (2 s elapsed total, 1 s more). Duplicator 1 finishes. Now have 3 snippets. Need 3 more.
    3. Use duplicator 1 on original (3 s elapsed total, 1 s more). Duplicator 2 finishes its first copy. Now have 4 snippets. Need 2 more.
    4. Use duplicator 1 on original, duplicator 2 on a copy (4 s elapsed total, 1 s more). Duplicator 1 finishes. Now have 5 snippets. Need 1 more. Duplicator 2 finishes. Now have 6 snippets. We have enough copies.
Minimum time is 4 seconds.

### 2

#### Input

4 1 1

#### Output

3

#### Explanation

Need 4 copies. Both duplicators take 1 s.
    1. Use duplicator 1 on original (1 s). Have 2 snippets. Need 3 more.
    2. Use duplicator 1 and 2 on the available snippets (2 s). Have 4 snippets. Need 1 more.
    3. Use duplicator 1 and 2 again (3 s). Have 6 snippets. We have enough.
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