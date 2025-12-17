## Title
Archaeological Counterweight

## Slug
archaeological-counterweight

## Difficulty
Easy

## Description
Indiana is exploring an ancient temple and encounters a sealed stone door. The door mechanism is controlled by a pressure plate system that responds to 'spiritual weight'. The archaeologist finds a pile of stone artifacts nearby, each inscribed with a sacred integer. The temple lore states that the spiritual weight of an artifact is the square of its inscribed number. To open the door without triggering a trap, Indiana must place exactly three artifacts on the altar such that their combined spiritual weight equals the door's locking value.

Your task is to determine whether it is possible to choose three distinct stone artifacts (at indices i < j < k) such that:

    num_i^2 + num_j^2 + num_k^2 = door_mechanism

If it is possible, print YES; otherwise, print NO.

## Examples

### 1
#### Input
5
1 2 2 3 4
9

#### Output
YES

#### Explanation
1^2 + 2^2 + 2^2 = 1 + 4 + 4 = 9.

### 2
#### Input
4
3 3 3 3
20

#### Output
NO

#### Explanation
Every square is 9; any sum of three squares is 27 which is not 20.

## Input Format
- First line: integer n — the number of stone artifacts.
- Second line: n space-separated integers a1 a2 ... an — the inscribed numbers (can be negative, zero, or positive).
- Third line: integer target — the target sum.

## Output Format
- Return true (YES) if there exist indices i < j < k with a[i]^2 + a[j]^2 + a[k]^2 = target, otherwise return false (NO).

## Constraints
- 3 ≤ n ≤ 2000
- -10^6 ≤ ai ≤ 10^6
- 0 ≤ target ≤ 3×10^12

## Time Limit
1 second

## Memory Limit
256 MB

## Tags 
two-pointers, sorting, array, maths
