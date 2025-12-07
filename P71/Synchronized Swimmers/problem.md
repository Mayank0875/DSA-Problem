## Title
Synchronized Swimmers

## Slug
synchronized-swimmers

## Difficulty
Medium

## Description
Swimmers hold hands in formations. Formations are always closed rings.

There are n swimmers.
Rings have at least 2 swimmers.
Each swimmer is confirmed holding one person's hand.

Your task is to analyze this partial data and determine the minimum and maximum number of separate rings that could possibly exist, consistent with the given records.

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
These could be 3 separate rings of 2 swimmers each.
Minimum:
Since we only know one neighbor per swimmer, these pairs could actually be segments of a bigger ring. All swimmers can be arranged into one single ring:
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
- The first line contains an integer n, the number of swimmers.
- The second line contains n space-separated integers a1, a2, ..., an, where ai is the neighbor remembered by the i-th swimmer.

## Output Format
- Return two integers: the minimum number of rings and the maximum number of rings.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ ai ≤ 2e5
- ai ≠ i
- The input guarantees that a valid configuration of rings exists.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, depth-first-search, connected-components
