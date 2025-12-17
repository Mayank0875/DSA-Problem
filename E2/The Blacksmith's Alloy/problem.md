## Title
The Blacksmith's Alloy

## Slug
blacksmiths-alloy

## Difficulty
Easy

## Description
A legendary blacksmith is forging a blade for the King. The strength of the final alloy depends on the materials used. The blacksmith has a crate of metal ingots, each stamped with a purity rating. The magical properties of the forge dictate that the final strength of the alloy is the sum of the squares of the purity ratings of the ingredients. To forge the 'Sword of Destiny', the blacksmith must throw exactly three distinct ingots into the furnace to achieve the prophesied alloy strength.

Your task is to determine whether it is possible to choose three distinct metal ingots (at indices i < j < k) such that:

    purity_i^2 + purity_j^2 + purity_k^2 = alloy_strength

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
- First line: integer n — the number of metal ingots.
- Second line: n space-separated integers a1 a2 ... an — the purity ratings (can be negative, zero, or positive).
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
