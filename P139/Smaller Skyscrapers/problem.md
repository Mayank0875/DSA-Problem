## Title
Smaller Skyscrapers

## Slug
smaller-skyscrapers

## Difficulty
Medium

## Description
An architect compares building designs.

You have a list of $n$ buildings. Each building has two main properties: **height** and **floor count**. You are given a 2D integer array `properties` where `properties[i] = [height_i, floor count_i]` represents the attributes of the $i$-th building.

A building is considered **smaller** if there exists another building that has **both** strictly greater height and strictly greater floor count.

More formally, the $i$-th building is smaller if there exists an index $j$ such that `height_j > height_i` and `floor count_j > floor count_i`.

Your task is to return the number of smaller buildings.

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
No building has strictly greater height and floor count than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first building (2, 2) is smaller because the second building (3, 3) has strictly greater height and floor count.

## Input Format
- The first line contains an integer $n$, the number of buildings.
- The next $n$ lines each contain two space-separated integers, representing the height and floor count of a building.

## Output Format
- Return a single integer representing the number of smaller buildings.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ height, floor count ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
