## Title
Crystal Resonance

## Slug
crystal-resonance

## Difficulty
Medium

## Description
Crystals transmit vibrations. A Resonance Group is a set of crystals that vibrate together.

Two crystals a and b belong to the same Resonance Group if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of vibrations.
In other words, two crystals are in the same Resonance Group if they are mutually reachable.

Your task is to: Determine how many Resonance Groups exist in total.

## Examples

### 1

#### Input
5 6
1 2
2 3
3 1
3 4
4 5
5 4

#### Output
2

#### Explanation
The crystals form two distinct groups where round-trip traversal is possible within each group.
Crystals {1, 2, 3} form one Resonance Group.
Path: 1 -> 2 -> 3 -> 1.
Crystals {4, 5} form another Resonance Group.
Path: 4 -> 5 -> 4.
Total Resonance Groups: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 crystals and 1 one-way vibration.
Vibration: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Resonance Groups.

## Input Format
- The first line contains two integers n and m: the number of crystals and vibrations.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way vibration from crystal a to crystal b.

## Output Format
- Return one integer: the total number of Resonance Groups.

## Constraints
- 1 ≤ n ≤ 1e5
- 1 ≤ m ≤ 2e5
- 1 ≤ a, b ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, depth-first-search
