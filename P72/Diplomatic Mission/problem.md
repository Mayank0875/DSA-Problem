## Title
Diplomatic Mission

## Slug
diplomatic-mission

## Difficulty
Hard

## Description
A diplomat visits embassies in a capital city. Starting at Embassy 1, they must reach the UN Building (n). Travel is via one-way diplomatic lanes.

The diplomat must start at the Home Embassy (labeled 1) and finish at the UN Building (labeled n). However, to sign treaties with every nation represented, the diplomat must visit **every single embassy exactly once** during the journey.

You are given the map of the embassies and the directed lanes connecting them. Your task is to calculate the total number of distinct valid paths the diplomat can take to complete the mission. As the number of paths can be very large, print the answer modulo 1000000007.

## Examples

### 1

#### Input
4 6
1 2
1 3
2 3
3 2
2 4
3 4

#### Output
2

#### Explanation
There are two possible paths that visit every embassy exactly once:
1 -> 2 -> 3 -> 4
1 -> 3 -> 2 -> 4

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
The only valid path is 1 -> 2.

## Input Format
- The first line contains two integers n and m: the number of embassies and the number of lanes.
- The embassies are numbered 1, 2, ..., n.
- The next m lines describe the lanes. Each line has two integers a and b, indicating a one-way lane from embassy a to embassy b.

## Output Format
- Return one integer: the number of possible mission paths modulo 10^9+7.

## Constraints
- 1 ≤ n ≤ 20
- 1 ≤ m ≤ n * n
- 1 ≤ a, b ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, dynamic-programming
