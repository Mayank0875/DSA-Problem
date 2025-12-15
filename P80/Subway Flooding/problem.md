## Title
Subway Flooding

## Slug
subway-flooding

## Difficulty
Medium

## Description
Water enters at the River Tunnel (node 1) and flows toward Central Station (node n).

The subway consists of $n$ platforms connected by $m$ two-way tracks.
The water is attempting to travel from the Tunnel (node 1) to Central Station (node $n$).

To prevent this, you can bulkhead specific tracks. Closing a bulkhead seals the track.

Your task is to calculate the **minimum number of tracks** that must be sealed to completely sever all routes between the Tunnel and Central Station.

## Examples

### 1

#### Input
4 5
1 2
1 3
2 3
3 4
1 4

#### Output
2

#### Explanation
The minimum is 2.

### 2

#### Input
3 3
1 2
2 3
1 3

#### Output
2

#### Explanation
We can bulkhead edges (1,3) and (2,3) to isolate node 3.

## Input Format
- The first line contains two integers $n$ and $m$: the number of platforms and tracks.
- The next $m$ lines describe the tracks. Each line contains two integers $a$ and $b$, indicating a track between platform $a$ and platform $b$.

## Output Format
- Return one integer: the minimum number of tracks that need to be sealed.

## Constraints
- 1 ≤ n ≤ 500
- 1 ≤ m ≤ 1000
- 1 ≤ a, b ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph
