## Title
Ancient Stone Circles

## Slug
ancient-stone-circles

## Difficulty
Medium

## Description
Archaeologists found n standing stones. Ancient texts say the stones were arranged in perfect circular formations. Each stone has markings pointing to exactly one neighbor in the circle.

There are n stones.
Every stone must belong to a circle of at least 2 stones.
Currently, for every stone, we found exactly one marking pointing to a neighbor.

Your task is to analyze this partial data and determine the minimum and maximum number of separate circles that could possibly exist, consistent with the given records.

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
These could be 3 separate circles of 2 stones each.
Minimum:
Since we only know one neighbor per stone, these pairs could actually be segments of a bigger ring. All stones can be arranged into one single ring:
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
- The first line contains an integer n, the number of stones.
- The second line contains n space-separated integers a1, a2, ..., an, where ai is the neighbor remembered by the i-th stone.

## Output Format
- Return two integers: the minimum number of circles and the maximum number of circles.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ ai ≤ 2e5
- ai ≠ i
- The input guarantees that a valid configuration of circles exists.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, depth-first-search, connected-components
