## Title
Magic Ritual

## Slug
magic-ritual

## Difficulty
Medium

## Description
A wizard draws a rune circle. Magic flows through focal points. A closed loop is required for the spell.

A "magic circle" occurs when mana moves from a crystal, through a sequence of leylines, and returns to the starting crystal without traversing the same leyline twice in immediate succession. The "length" of such a magic circle is the number of leylines it contains.

Small, tight circles are more potent. Find the number of crystals in the smallest circle.

Given the layout of the ritual site, determine the length of the shortest magic circle.

## Examples

### 1

#### Input
5 6
1 2
1 3
2 4
2 5
3 4
4 5

#### Output
3

#### Explanation
There are several magic circles in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest magic circle has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no magic circles in this network.

## Input Format
- The first line contains two integers n and m: the number of crystals and the number of leylines.
- The crystals are numbered 1, 2, ..., n.
- The next m lines describe the leylines. Each line contains two integers u and v, indicating a connection between crystal u and crystal v.
- The graph is undirected. There is at most one leyline between any two crystals.

## Output Format
- Return one integer: the length of the shortest magic circle. If there are no magic circles, print `-1`.

## Constraints
- 1 ≤ n ≤ 2500
- 1 ≤ m ≤ 5000
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, breadth-first-search
