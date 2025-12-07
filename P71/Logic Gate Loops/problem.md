## Title
Logic Gate Loops

## Slug
logic-gate-loops

## Difficulty
Medium

## Description
Gates are wired in feedback oscillators.

There are n gates.
Oscillators have at least 2 gates.
Each gate feeds into one other gate.

Your task is to analyze this partial data and determine the minimum and maximum number of separate oscillators that could possibly exist, consistent with the given records.

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
These could be 3 separate oscillators of 2 gates each.
Minimum:
Since we only know one neighbor per gate, these pairs could actually be segments of a bigger ring. All gates can be arranged into one single ring:
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
- The first line contains an integer n, the number of gates.
- The second line contains n space-separated integers a1, a2, ..., an, where ai is the neighbor remembered by the i-th gate.

## Output Format
- Return two integers: the minimum number of oscillators and the maximum number of oscillators.

## Constraints
- 1 ≤ n ≤ 2e5
- 1 ≤ ai ≤ 2e5
- ai ≠ i
- The input guarantees that a valid configuration of oscillators exists.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, depth-first-search, connected-components
