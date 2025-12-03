## Title

Space Station Energy Link

## Slug

space-station-energy-link

## Difficulty

Medium

## Description

Two parallel space stations, Alpha and Beta, are drifting in orbit. Each station consists of a row of $n$ modules. The modules in station Alpha have energy levels represented by an array $a$, and station Beta's modules have energy levels represented by an array $b$. Within each station, adjacent modules are already connected by internal corridors.

To ensure the survival of the crew, you must build inter-station power cables connecting modules from Alpha to modules from Beta. The cost to build a cable between the $i$-th module of Alpha and the $j$-th module of Beta is the absolute difference of their energy levels: $|a_i - b_j|$.

The final network must be **fault-tolerant**. This means that if any single module in either station malfunctions and is removed (along with its internal and external connections), the remaining modules must still be connected as a single network. Your task is to calculate the minimum total cost required to build such a set of cables.

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