## Title
Teleporter Calibration

## Slug
teleporter-calibration

## Difficulty
Medium

## Description
Teleport pads are linked. Technicians need to calibrate the link between two pads by standing on them simultaneously. Each pad is used once.

The structure is a tree with n pads and n-1 links.
A calibration is formed between two pads connected by a link.
However, each pad can be part of at most one calibration.

Your task is to calculate the maximum number of calibrations that can be formed.

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
One optimal set of calibrations is (1, 2) and (3, 4). Node 5 remains unpaired. This gives a total of 2 calibrations.

### 2

#### Input
4
1 2
2 3
3 4

#### Output
2

#### Explanation
We can form calibrations (1, 2) and (3, 4), giving a total of 2.

## Input Format
- The first line contains an integer n, the number of pads.
- The next n-1 lines each contain two integers u and v, representing a link between pad u and pad v.

## Output Format
- Return a single integer representing the maximum number of calibrations.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, graph
