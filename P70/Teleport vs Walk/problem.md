## Title
Teleport vs Walk

## Slug
teleport-vs-walk

## Difficulty
Medium

## Description
A Wizard teleports. An Apprentice walks. The Apprentice walks paths connecting runes that aren't teleport-linked.

The academy has n runes numbered from 1 to n.
The Teleport Circle connects specific pairs of runes with direct blinks.
The Stone Path is constructed based on a unique rule:
A direct walk exists between two runes if and only if there is no blink connecting them.

Moving between any two connected runes takes exactly 1 hour on either network.
Two casters, The Wizard and The Apprentice, depart from rune 1 at the same time, heading for rune n.

1. The Wizard travels only using Teleport Circle.
2. The Apprentice travels only using Stone Path.

To ensure safety, they must never arrive at the same rune at the same time (except for the final rune n).
Your task is to compute the minimum number of hours required for **both** casters to reach rune n — specifically, the time when the slower caster arrives.
If either caster cannot reach rune n using their respective network, return -1.

## Examples

### 1

#### Input
4 2
1 3
3 4

#### Output
2

#### Explanation
The smallest possible time is 2. One takes the direct route (1 hour), the other takes a path of length 2.

### 2

#### Input
4 6
1 2
1 3
1 4
2 3
2 4
3 4

#### Output
-1

#### Explanation
The graph is fully connected for one network, meaning the complement network has no edges. The second caster cannot reach the destination.

## Input Format
- The first line contains two integers n and m, representing the number of runes and the number of blinks.
- The next m lines each contain two integers u and v, representing a blink between runes u and v.
- The graph is bidirectional. There is at most one blink between any pair of runes.

## Output Format
- Return a single integer representing the minimum hours required for the last caster to arrive. If it is impossible, return -1.

## Constraints
- 2 ≤ n ≤ 400
- 0 ≤ m ≤ n(n - 1)/2
- 1 ≤ u, v ≤ n
- u ≠ v

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, breadth-first-search
