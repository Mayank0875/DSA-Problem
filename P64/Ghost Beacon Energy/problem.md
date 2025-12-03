## Title
Ghost Beacon Energy

## Slug
ghost-beacon-energy

## Difficulty
Medium

## Description
Paranormal investigators place N beacons to trap a ghost. The beacons form a barrier if connected. Connection requires spectral energy X equal to squared distance. Find the minimum energy X to seal the perimeter.

Your task is to find the minimum integer value of X (squared distance limit) that ensures every beacon can communicate/connect with every other beacon, either directly or through a chain of intermediates.

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
The optimal strategy connects the beacons using links whose squared distances are at most 17.
For example, the squared distance between the points (1,3) and (5,4) is:
(1 - 5)² + (3 - 4)² = 16 + 1 = 17.
If the beacons can connect up to a squared distance of 17, the network becomes fully connected.

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
- The first line contains an integer N, the number of beacons.
- The next N lines each contain two integers x and y, representing the coordinates of a beacon.

## Output Format
- Return a single integer X, the minimum spectral energy required to connect the network.

## Constraints
- 1 ≤ N ≤ 1000
- 1 ≤ x, y ≤ 25000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, binary-search
