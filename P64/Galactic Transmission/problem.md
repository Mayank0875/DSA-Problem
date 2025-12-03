## Title

Galactic Transmission

## Slug

galactic-transmission

## Difficulty

Medium

## Description

In a distant galaxy, the Interstellar Alliance operates N space stations placed at different coordinates on a 2D plane. To keep the galaxy safe, all stations must be able to relay urgent messages to each other.

A message can be transmitted directly between two stations if their transceivers are powerful enough. If direct transmission is not possible, the message can still reach its destination by passing through other stations.

All stations will be equipped with identical transceivers. If the Alliance spends X credits, each station receives a transceiver that can transmit signals up to a distance equal to the square root of X. This means two stations can communicate directly if the squared distance between them is at most X.

Your task is to find the minimum integer value of X that ensures every station can communicate with every other station, either directly or through a chain of intermediate stations.

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

The optimal strategy connects the stations using links whose squared distances are at most 17.
For example, the squared distance between the points (1,3) and (5,4) is:

(1 - 5)² + (3 - 4)² = 16 + 1 = 17

So, if the stations can communicate up to a squared distance of 17 (which corresponds to a distance of square root of 17), then the entire network becomes fully connected.
    
### 2

#### Input

3 
0 0
0 10
10 0

#### Output

100

#### Explanation

We need to connect (0,0) to either (0,10) or (10,0). Both points are at a squared distance of 100 from the origin. Once one of them is connected, the other either needs a much larger range to connect directly, or it can use the same range by connecting through the origin. A squared distance of 100 is enough to form the path:
(0,10) <-> (0,0) <-> (10,0)
  

## Input Format  

- The first line contains an integer $N$, the number of space stations.
- The next $N$ lines each contain two integers $x$ and $y$, representing the coordinates of a station.

## Output Format  

- Return a single integer $X$, the minimum cost required to connect the network.
  

## Constraints  

- 1 ≤ N ≤ 1000
- 1 ≤ x, y ≤ 25000

## Time Limit

2 second

## Memory Limit

256 MB

## Tags
graph, binary-search

## Companies
infosys