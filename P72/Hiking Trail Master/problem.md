## Title
Hiking Trail Master

## Slug
hiking-trail-master

## Difficulty
Hard

## Description
A hiker takes on a challenge. Starting at the Trailhead (1), they must reach the Lodge (n). Scenic spots are connected by trails.

The hiker must start at the Trailhead (labeled 1) and finish at the Lodge (labeled n). However, to stamp their pass at every scenic spot, the hiker must visit **every single spot exactly once** during the journey.

You are given the map of the spots and the directed trails connecting them. Your task is to calculate the total number of distinct valid paths the hiker can take to complete the hike. As the number of paths can be very large, print the answer modulo 1000000007.

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
There are two possible paths that visit every spot exactly once:
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
- The first line contains two integers n and m: the number of spots and the number of trails.
- The spots are numbered 1, 2, ..., n.
- The next m lines describe the trails. Each line has two integers a and b, indicating a one-way trail from spot a to spot b.

## Output Format
- Return one integer: the number of possible hike paths modulo 10^9+7.

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
