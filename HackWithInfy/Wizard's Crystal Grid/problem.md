## Title

Space Station Energy Link

## Slug

space-station-energy-link

## Difficulty

Medium

## Description

Two parallel space stations, Alpha and Beta, each contain n modules arranged in a line.
Station Alpha has an array a representing the energy level of each module.
Station Beta has an array b representing the energy level of each module.

Inside each station, adjacent modules are already connected by internal corridors.

You must build inter-station power cables connecting some modules of Alpha to some modules of Beta.

The cost to build a cable between module i of Alpha and module j of Beta is:
absolute value of (a[i] - b[j]).

Fault-tolerance requirement:
The final network must remain fully connected even if any single module is removed (from either Alpha or Beta).
If one module fails and disappears along with all its internal and external cables, the remaining modules must still form a single connected network.

Your task is to calculate the minimum total cost required to build such a set of inter-station cables.

## Examples

### 1

#### Input

3
1 10 1
20 4 25

#### Output

31

#### Explanation

It's optimal to connect four pairs of computers:

computer 1 from the first row with computer 2 from the second row: cost |1−4|=3 ;
computer 3 from the first row with computer 2 from the second row: cost |1−4|=3 ;
computer 2 from the first row with computer 1 from the second row: cost |10−20|=10;
computer 2 from the first row with computer 3 from the second row: cost |10−25|=15 ;
In total, 3+3+10+15=31 .
    
### 2

#### Input

4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output

1999999998

#### Explanation

It's optimal to connect 1 from the first row with 1 from the second row, and 4 from the first row with 4 from the second row.

## Input Format  

- The first line contains an integer $n$, the number of modules in each station.
- The second line contains $n$ integers representing the energy levels of station Alpha.
- The third line contains $n$ integers representing the energy levels of station Beta.

## Output Format  

- Return a single integer representing the minimum total cost to make the network fault-tolerant.

## Constraints  

- 3 ≤ n ≤ 1e5
- 1 ≤ a_i, b_i ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

graph, greedy