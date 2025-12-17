## Title
Chemical Reaction Potency

## Slug
chemical-reaction-potency

## Difficulty
Easy

## Description
A chemist is experimenting with a volatile new compound. They have a rack of vials containing solutions with different molar concentrations. The exothermic heat released by reacting a solution is proportional to the square of its concentration. The experiment requires generating a precise amount of heat to catalyze the reaction without causing an explosion. The chemist needs to mix exactly three vials into the reactor to hit the target heat output.

Your task is to determine whether it is possible to choose three distinct chemical vials (at indices i < j < k) such that:

    conc_i^2 + conc_j^2 + conc_k^2 = reaction_heat

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
- First line: integer n — the number of chemical vials.
- Second line: n space-separated integers a1 a2 ... an — the concentration levels (can be negative, zero, or positive).
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
