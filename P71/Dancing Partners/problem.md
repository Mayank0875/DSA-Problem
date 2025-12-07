## Title
Dancing Partners

## Slug
dancing-partners

## Difficulty
Medium

## Description
In a folk dance, n dancers form several circle dances. In a circle, everyone holds hands with two neighbors.

There are n dancers.
A circle must have at least 2 dancers.
Each dancer recalls holding the hand of exactly one person.

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
These could be 3 separate circles of 2 dancers each.
Minimum:
Since we only know one neighbor per dancer, these pairs could actually be segments of a bigger ring. All dancers can be arranged into one single ring:
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
- The first line contains an integer n, the number of dancers.
- The second line contains n space-separated integers a1, a2, ..., an, where ai is the neighbor remembered by the i-th dancer.

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
