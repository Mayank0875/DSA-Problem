## Title
Magic Spell Chain

## Slug
magic-spell-chain

## Difficulty
Medium

## Description
A wizard must channel mana from the Source Crystal (node 1) to the Target Focus (node n).

The ritual circle has `n` runes and `m` directed energy flows. Energy flows may repeat between the same pair of runes and self-loops are allowed. A sequence of length `k` is a sequence of exactly `k` directed energy flows; runes and energy flows may be visited multiple times.

Given `n`, `m`, `k` and a list of the `m` directed energy flows (each flow given as two integers `u` `v` meaning a directed flow from `u` to `v`), compute the number of distinct sequences that start at rune 1 and end at rune `n` with length exactly `k`. Output the answer modulo 1000000007.

## Examples

### 1

#### Input
3 4 8
1 2
2 3
3 1
3 2

#### Output
2

#### Explanation
We have 3 runes. We want the number of directed sequences of length 8 from rune 1 to rune 3.
Valid length-8 sequences:
1 -> 2 -> 3 -> 1 -> 2 -> 3 -> 1 -> 2 -> 3
1 -> 2 -> 3 -> 2 -> 3 -> 1 -> 2 -> 3
There are 2 such sequences.

### 2

#### Input
3 4 2
1 2
2 3
3 1
3 2

#### Output
1

#### Explanation
Assuming the graph has energy flows 1->2 and 2->3, the only sequence of length 2 from rune 1 to rune 3 is:
1 -> 2 -> 3

## Input Format
- The first line contains three integers n, m, and k: the number of runes, energy flows, and the required sequence length.
- The next m lines describe the energy flows. Each line contains two integers u and v, indicating a directed flow from rune u to rune v.

## Output Format
- Return single integer: the number of sequences modulo 10^9+7.

## Constraints
- 1 ≤ n ≤ 100
- 1 ≤ m ≤ 10^5
- 1 ≤ k ≤ 10^18
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, dynamic-programming
