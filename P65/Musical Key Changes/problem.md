## Title
Musical Key Changes

## Slug
musical-key-changes

## Difficulty
Medium

## Description
Keys can modulate to others. A Harmonic Circle is a set of keys that can modulate to each other.

Two keys a and b belong to the same Circle if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of modulations.
In other words, two keys are in the same Circle if they are mutually reachable.

Your task is to: Determine how many Circles exist in total.

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
The keys form two distinct groups where round-trip traversal is possible within each group.
Keys {1, 2, 3} form one Circle.
Path: 1 -> 2 -> 3 -> 1.
Keys {4, 5} form another Circle.
Path: 4 -> 5 -> 4.
Total Circles: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 keys and 1 one-way modulation.
Modulation: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Circles.

## Input Format
- The first line contains two integers n and m: the number of keys and modulations.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way modulation from key a to key b.

## Output Format
- Return one integer: the total number of Circles.

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
