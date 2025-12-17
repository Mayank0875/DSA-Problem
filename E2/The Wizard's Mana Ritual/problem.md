## Title
The Wizard's Mana Ritual

## Slug
wizards-mana-ritual

## Difficulty
Easy

## Description
In the Academy of Arcane Arts, an apprentice wizard is attempting to cast a Level 9 Fireball. This spell requires a precise amount of magical energy. The apprentice has a pouch full of mana crystals, each vibrating at a different resonance frequency. The magical output of a crystal is equal to the square of its frequency. The spell will only stabilize if the apprentice consumes exactly three crystals whose combined output matches the spell's energy cost perfectly.

Your task is to determine whether it is possible to choose three distinct mana crystals (at indices i < j < k) such that:

    freq_i^2 + freq_j^2 + freq_k^2 = target_mana

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
- First line: integer n — the number of mana crystals.
- Second line: n space-separated integers a1 a2 ... an — the resonance frequencies (can be negative, zero, or positive).
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
