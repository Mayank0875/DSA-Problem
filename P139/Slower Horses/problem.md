## Title
Slower Horses

## Slug
slower-horses

## Difficulty
Medium

## Description
A jockey compares racehorses.

You have a list of $n$ horses. Each horse has two main properties: **stamina** and **burst speed**. You are given a 2D integer array `properties` where `properties[i] = [stamina_i, burst speed_i]` represents the attributes of the $i$-th horse.

A horse is considered **slower** if there exists another horse that has **both** strictly greater stamina and strictly greater burst speed.

More formally, the $i$-th horse is slower if there exists an index $j$ such that `stamina_j > stamina_i` and `burst speed_j > burst speed_i`.

Your task is to return the number of slower horses.

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
No horse has strictly greater stamina and burst speed than another.

### 2

#### Input
2
2 2
3 3

#### Output
1

#### Explanation
The first horse (2, 2) is slower because the second horse (3, 3) has strictly greater stamina and burst speed.

## Input Format
- The first line contains an integer $n$, the number of horses.
- The next $n$ lines each contain two space-separated integers, representing the stamina and burst speed of a horse.

## Output Format
- Return a single integer representing the number of slower horses.

## Constraints
- 1 ≤ n ≤ 10^5
- 1 ≤ stamina, burst speed ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy, sorting
