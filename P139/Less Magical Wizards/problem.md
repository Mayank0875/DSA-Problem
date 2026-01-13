## Title
Less Magical Wizards

## Slug
less-magical-wizards

## Difficulty
Medium

## Description
A magical academy ranks wizards.

You have a list of $n$ wizards. Each wizard has two main properties: **mana pool** and **spell power**. You are given a 2D integer array `properties` where `properties[i] = [mana pool_i, spell power_i]` represents the attributes of the $i$-th wizard.

A wizard is considered **less magical** if there exists another wizard that has **both** strictly greater mana pool and strictly greater spell power.

More formally, the $i$-th wizard is less magical if there exists an index $j$ such that `mana pool_j > mana pool_i` and `spell power_j > spell power_i`.

Your task is to return the number of less magical wizards.

## Examples

### 1

#### Input
3
5 5
6 3
3 6

#### Output
0

#### Explanation
No wizard has strictly greater mana pool and spell power than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first wizard (2, 2) is less magical because the second wizard (3, 3) has strictly greater mana pool and spell power.

## Input Format
- The first line contains an integer $n$, the number of wizards.
- The next $n$ lines each contain two space-separated integers, representing the mana pool and spell power of a wizard.

## Output Format
- Return a single integer representing the number of less magical wizards.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ mana pool, spell power ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
