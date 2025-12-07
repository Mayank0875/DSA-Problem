## Title
Wireless Mesh Links

## Slug
wireless-mesh-links

## Difficulty
Medium

## Description
A network of IoT devices forms a tree topology. To save power, devices are entering a dedicated link mode where they pair up with exactly one neighbor for high-speed transfer.

The structure is a tree with n devices and n-1 links.
A dedicated link is formed between two devices connected by a link.
However, each device can be part of at most one dedicated link.

Your task is to calculate the maximum number of dedicated links that can be formed.

## Examples

### 1

#### Input
5
1 2
1 3
3 4
3 5

#### Output
2

#### Explanation
One optimal set of dedicated links is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 dedicated links.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form dedicated links (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of devices.
- The next n-1 lines each contain two integers u and v, representing a link between device u and device v.

## Output Format
- Return a single integer representing the maximum number of dedicated links.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
