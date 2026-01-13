## Title
Worse Microwaves

## Slug
worse-microwaves

## Difficulty
Medium

## Description
A kitchen appliance tester checks microwaves.

You have a list of $n$ microwaves. Each microwave has two main properties: **wattage** and **volume**. You are given a 2D integer array `properties` where `properties[i] = [wattage_i, volume_i]` represents the attributes of the $i$-th microwave.

A microwave is considered **worse** if there exists another microwave that has **both** strictly greater wattage and strictly greater volume.

More formally, the $i$-th microwave is worse if there exists an index $j$ such that `wattage_j > wattage_i` and `volume_j > volume_i`.

Your task is to return the number of worse microwaves.

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
No microwave has strictly greater wattage and volume than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first microwave (2, 2) is worse because the second microwave (3, 3) has strictly greater wattage and volume.

## Input Format
- The first line contains an integer $n$, the number of microwaves.
- The next $n$ lines each contain two space-separated integers, representing the wattage and volume of a microwave.

## Output Format
- Return a single integer representing the number of worse microwaves.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ wattage, volume ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
