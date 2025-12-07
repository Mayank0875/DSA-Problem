## Title
Flower Garland

## Slug
flower-garland

## Difficulty
Medium

## Description
Flowers are strung into garlands. Each flower is tied to two neighbors.

There are n flowers.
Garlands are loops of at least 2 flowers.
We can see one string tie per flower.

Your task is to analyze this partial data and determine the minimum and maximum number of separate garlands that could possibly exist, consistent with the given records.

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
These could be 3 separate garlands of 2 flowers each.
Minimum:
Since we only know one neighbor per flower, these pairs could actually be segments of a bigger ring. All flowers can be arranged into one single ring:
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
- The first line contains an integer n, the number of flowers.
- The second line contains n space-separated integers a1, a2, ..., an, where ai is the neighbor remembered by the i-th flower.

## Output Format
- Return two integers: the minimum number of garlands and the maximum number of garlands.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ ai ≤ 2e5
- ai ≠ i
- The input guarantees that a valid configuration of garlands exists.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, depth-first-search, connected-components
