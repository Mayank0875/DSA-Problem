## Title

Logic Paradox

## Slug

logic-paradox

## Difficulty

Easy

## Description

A mysterious paradoxical device can duplicate logical statements! The chief logician has the original statement and must produce exactly n additional copies before the paradox resolves. There are two paradox‑duplicators available.  
The first duplicator takes x seconds to copy one statement (from the original or any existing copy), and the second duplicator takes y seconds. The logicians may use either duplicator or both simultaneously.  
Help the chief logician determine the minimum amount of time required to produce at least n new copies of the statement, starting with just the original.

## Examples

### 1

#### Input

5 1 2

#### Output

4

#### Explanation

We need 5 copies. Assume duplicator 1 takes 1 s, duplicator 2 takes 2 s.  
1. Use duplicator 1 on the original (1 s elapsed). Now we have 2 statements. Need 4 more.  
2. Use duplicator 1 on the original, duplicator 2 on a copy (2 s elapsed total, 1 s more). Duplicator 1 finishes. Now have 3 statements. Need 3 more.  
3. Use duplicator 1 on the original (3 s elapsed total, 1 s more). Duplicator 2 finishes its first copy. Now have 4 statements. Need 2 more.  
4. Use duplicator 1 on the original, duplicator 2 on a copy (4 s elapsed total, 1 s more). Duplicator 1 finishes. Now have 5 statements. Need 1 more. Duplicator 2 finishes. Now have 6 statements. We have enough copies.  
Minimum time is 4 seconds.

### 2

#### Input

4 1 1

#### Output

3

#### Explanation

Need 4 copies. Both duplicators take 1 s.  
1. Use duplicator 1 on the original (1 s). Have 2 statements. Need 3 more.  
2. Use duplicator 1 and 2 on the available statements (2 s). Have 4 statements. Need 1 more.  
3. Use duplicator 1 and 2 again (3 s). Have 6 statements. We have enough.  
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