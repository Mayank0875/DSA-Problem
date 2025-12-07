## Title

Cosmic Data Relay

## Slug

cosmic-data-relay

## Difficulty

Hard

## Description

In the distant future, humanity has established a vast interstellar network of communication buoys. You are a network engineer aboard the Starship Aethelgard, stationed at the edge of the galaxy. Your mission is to transmit a critical data packet containing the coordinates of a newly discovered habitable planet back to Earth.

The network consists of n buoys, numbered 1 to n. Buoy 1 is your current location (the source), and buoy n is the Earth station (the destination). There are m one-way data links connecting these buoys. Each link has a specific bandwidth capacity, measured in terabytes per second (TB/s), which limits the rate at which data can be sent through it.

Multiple links can exist between the same two buoys, and their capacities stack. Your goal is to determine the maximum total data throughput that can be achieved from your location to Earth using the available network connections.

## Examples

### 1

#### Input

4 5
1 2 3
2 4 2
1 3 4
3 4 5
4 1 3

#### Output

6

#### Explanation
There are two main paths to transmit data from node 1 to node 4:
1 → 2 → 4 (capacity limited by link 2 → 4 with capacity 2).
1 → 3 → 4 (capacity limited by link 1 → 3 with capacity 4).
Total max flow is 2 + 4 = 6. The link 4 → 1 is ignored because it flows backward from the destination.
    
### 2

#### Input

3 2
1 2 5
2 3 5

#### Output

5

#### Explanation

A single path 1 → 2 → 3 exists with a bottleneck capacity of 5.
  

## Input Format  

- The first line contains two integers n and m: the number of buoys and the number of connections.
- The next $m$ lines describe the connections. Each line contains three integers u, v, and c, indicating a one-way link from buoy $u$ to buoy v with capacity c.

## Output Format  

- Return one integer: the maximum data throughput (max flow) from buoy 1 to buoy n.
  

## Constraints  

- 1 ≤ n ≤ 500
- 1 ≤ m ≤ 1000
- 1 ≤ a, b ≤ n
- 1 ≤ c ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

graph