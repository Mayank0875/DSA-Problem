## Title
Music Melody

## Slug
music-melody

## Difficulty
Medium

## Description
Composers use repetition. A loop occurs when a sequence of notes returns to the tonic.

A "melodic loop" occurs when a theme moves from a note, through a sequence of intervals, and returns to the starting note without traversing the same interval twice in immediate succession. The "length" of such a melodic loop is the number of intervals it contains.

Short loops are catchy. Find the length of the shortest repeating phrase.

Given the layout of the composition, determine the length of the shortest melodic loop.

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
There are several melodic loops in this network:
1-2-4-3-1 (length 4)
2-4-5-2 (length 3)
1-2-5-4-3-1 (length 5)
The shortest melodic loop has a length of 3.

### 2

#### Input
4 3
1 2
2 3
3 4

#### Output
-1

#### Explanation
The connections form a straight line (1-2-3-4). There are no melodic loops in this network.

## Input Format
- The first line contains two integers n and m: the number of notes and the number of intervals.
- The notes are numbered 1, 2, ..., n.
- The next m lines describe the intervals. Each line contains two integers u and v, indicating a connection between note u and note v.
- The graph is undirected. There is at most one interval between any two notes.

## Output Format
- Return one integer: the length of the shortest melodic loop. If there are no melodic loops, print `-1`.

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
