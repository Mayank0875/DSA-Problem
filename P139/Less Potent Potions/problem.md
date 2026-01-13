## Title
Less Potent Potions

## Slug
less-potent-potions

## Difficulty
Medium

## Description
An alchemist brews potions.

You have a list of $n$ potions. Each potion has two main properties: **duration** and **healing amount**. You are given a 2D integer array `properties` where `properties[i] = [duration_i, healing amount_i]` represents the attributes of the $i$-th potion.

A potion is considered **less potent** if there exists another potion that has **both** strictly greater duration and strictly greater healing amount.

More formally, the $i$-th potion is less potent if there exists an index $j$ such that `duration_j > duration_i` and `healing amount_j > healing amount_i`.

Your task is to return the number of less potent potions.

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
No potion has strictly greater duration and healing amount than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first potion (2, 2) is less potent because the second potion (3, 3) has strictly greater duration and healing amount.

## Input Format
- The first line contains an integer $n$, the number of potions.
- The next $n$ lines each contain two space-separated integers, representing the duration and healing amount of a potion.

## Output Format
- Return a single integer representing the number of less potent potions.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ duration, healing amount ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
