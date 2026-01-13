## Title
Weaker Drills

## Slug
weaker-drills

## Difficulty
Medium

## Description
A construction worker compares tools.

You have a list of $n$ drills. Each drill has two main properties: **RPM** and **torque**. You are given a 2D integer array `properties` where `properties[i] = [RPM_i, torque_i]` represents the attributes of the $i$-th drill.

A drill is considered **weaker** if there exists another drill that has **both** strictly greater RPM and strictly greater torque.

More formally, the $i$-th drill is weaker if there exists an index $j$ such that `RPM_j > RPM_i` and `torque_j > torque_i`.

Your task is to return the number of weaker drills.

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
No drill has strictly greater RPM and torque than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first drill (2, 2) is weaker because the second drill (3, 3) has strictly greater RPM and torque.

## Input Format
- The first line contains an integer $n$, the number of drills.
- The next $n$ lines each contain two space-separated integers, representing the RPM and torque of a drill.

## Output Format
- Return a single integer representing the number of weaker drills.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ RPM, torque ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
