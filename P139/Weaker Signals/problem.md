## Title
Weaker Signals

## Slug
weaker-signals

## Difficulty
Medium

## Description
A telecom company analyzes tower signals.

You have a list of $n$ towers. Each tower has two main properties: **range** and **signal strength**. You are given a 2D integer array `properties` where `properties[i] = [range_i, signal strength_i]` represents the attributes of the $i$-th tower.

A tower is considered **weaker** if there exists another tower that has **both** strictly greater range and strictly greater signal strength.

More formally, the $i$-th tower is weaker if there exists an index $j$ such that `range_j > range_i` and `signal strength_j > signal strength_i`.

Your task is to return the number of weaker towers.

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
No tower has strictly greater range and signal strength than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first tower (2, 2) is weaker because the second tower (3, 3) has strictly greater range and signal strength.

## Input Format
- The first line contains an integer $n$, the number of towers.
- The next $n$ lines each contain two space-separated integers, representing the range and signal strength of a tower.

## Output Format
- Return a single integer representing the number of weaker towers.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ range, signal strength ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
