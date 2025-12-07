## Title
Ice Skater Chains

## Slug
ice-skater-chains

## Difficulty
Medium

## Description
Skaters hold onto each other in chains/whips.

There are n skaters.
Chains connect at least 2 skaters.
Each skater holds one person's waist.

Your task is to analyze this partial data and determine the minimum and maximum number of separate chains that could possibly exist, consistent with the given records.

## Examples

### 1

#### Input
6
2 1 4 3 6 5

#### Output
1 3

#### Explanation
The records show the connections:
1 <-> 2,
3 <-> 4,
5 <-> 6.
Maximum:
These could be 3 separate chains of 2 skaters each.
Minimum:
Since we only know one neighbor per skater, these pairs could actually be segments of a bigger ring. All skaters can be arranged into one single ring:
1 - 2 - 3 - 4 - 5 - 6 - 1.

### 2

#### Input
6
2 3 1 5 6 4

#### Output
2 2

#### Explanation
Maximum: 2
Minimum: 2
(Two cycles of length 3 are formed, which are fixed).

## Input Format
- The first line contains an integer n, the number of skaters.
- The second line contains n space-separated integers a1, a2, ..., an, where ai is the neighbor remembered by the i-th skater.

## Output Format
- Return two integers: the minimum number of chains and the maximum number of chains.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ ai ≤ 2e5
- ai ≠ i
- The input guarantees that a valid configuration of chains exists.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, depth-first-search, connected-components
