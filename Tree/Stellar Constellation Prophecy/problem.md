## Title

Stellar Constellation Prophecy

## Slug

stellar-constellation-prophecy

## Difficulty

Hard

## Description

In the Andromeda galaxy, ancient astronomers believe in the power of **Prophetic Numbers**—positive integers that contain only the digits **4** and **7** in their decimal representation (e.g., 4, 7, 47, 744).

The galaxy consists of $n$ stars connected by $m$ bidirectional cosmic links. A group of stars connected to each other (directly or indirectly) forms a **constellation**. Currently, the galaxy is divided into several disjoint constellations.

The astronomers want to witness a cosmic event that only occurs when a single constellation has a size equal to a **Prophetic Number**. If no such constellation exists, they can artificially create links between stars of different constellations to merge them. Creating one link merges two constellations into one.

Your task is to determine the **minimum number of new links** required to form a constellation with a size equal to a Prophetic Number. If it is impossible, return -1.

## Examples

### 1

#### Input

4 3
1 2
2 3
1 3


#### Output

1

#### Explanation

Only 1 links needed.
    
### 2

#### Input

5 4
1 2
3 4
4 5
3 5


#### Output

-1

#### Explanation

There is no way.
  

## Input Format  

- The first line contains two integers $n$ and $m$.
- The next $m$ lines each contain two integers $u$ and $v$, representing a link between star $u$ and star $v$.

## Output Format  

- Return single integer the minimum number of links to add. If a Prophetic constellation already exists, print 0. If it is impossible, print -1.

## Constraints  

- 1 ≤ n, m ≤ 2e5
- 1 ≤ u, v ≤ 2e5

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

graph