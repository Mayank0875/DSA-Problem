## Title
Magic Crystal Grid

## Slug
magic-crystal-grid

## Difficulty
Medium

## Description
A wizard places N magic crystals on the ground. These crystals resonate with each other if they are close enough. The resonance range is defined by a power level X (covering squared distance X). Find the minimum power level X needed to link all crystals into a single mana web.

Your task is to find the minimum integer value of X (squared distance limit) that ensures every crystal can communicate/connect with every other crystal, either directly or through a chain of intermediates.

## Examples

### 1

#### Input
4
1 3
5 4
7 2
6 1

#### Output
17

#### Explanation
The optimal strategy connects the crystals using links whose squared distances are at most 17.
For example, the squared distance between the points (1,3) and (5,4) is:
(1 - 5)² + (3 - 4)² = 16 + 1 = 17.
If the crystals can connect up to a squared distance of 17, the network becomes fully connected.

### 2

#### Input
3
0 0
0 10
10 0

#### Output
100

#### Explanation
We need to connect (0,0) to either (0,10) or (10,0). Both points are at a squared distance of 100 from the origin.
A squared distance of 100 is enough to form the path:
(0,10) <-> (0,0) <-> (10,0).

## Input Format
- The first line contains an integer N, the number of crystals.
- The next N lines each contain two integers x and y, representing the coordinates of a crystal.

## Output Format
- Return a single integer X, the minimum power level required to connect the network.

## Constraints
- 1 ≤ N ≤ 1000
- 1 ≤ x, y ≤ 25000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, binary-search
