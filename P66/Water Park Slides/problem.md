## Title
Water Park Slides

## Slug
water-park-slides

## Difficulty
Medium

## Description
Two water slides need connecting tubes for maintenance access.

Two parallel slides, Slide 1 and Slide 2, each contain n sections arranged in a line.
Slide 1 has an array `a` representing the water flow of each section.
Slide 2 has an array `b` representing the water flow of each section.

Inside each slide, adjacent sections are already connected by internal tubes.

You must establish inter-slide access tunnels connecting some sections of Slide 1 to some sections of Slide 2.

The cost to create a tunnel between section i of Slide 1 and section j of Slide 2 is:
absolute value of (a[i] - b[j]).

**Fault-tolerance requirement:**
The final network must remain fully connected even if any single section is removed (from either Slide 1 or Slide 2).
If one section fails and disappears along with all its connections, the remaining sections must still form a single connected network.

Your task is to calculate the minimum total cost required to build such a set of connections.

## Examples

### 1

#### Input
3
1 10 1
20 4 25

#### Output
31

#### Explanation
It's optimal to connect four pairs of sections:
1. section 1 from Slide 1 with section 2 from Slide 2: cost |1-4| = 3.
2. section 3 from Slide 1 with section 2 from Slide 2: cost |1-4| = 3.
3. section 2 from Slide 1 with section 1 from Slide 2: cost |10-20| = 10.
4. section 2 from Slide 1 with section 3 from Slide 2: cost |10-25| = 15.
Total cost: 3 + 3 + 10 + 15 = 31.

### 2

#### Input
4
1 1 1 1
1000000000 1000000000 1000000000 1000000000

#### Output
1999999998

#### Explanation
It is optimal to connect the first section of Slide 1 with the first of Slide 2, and the last section of Slide 1 with the last of Slide 2, satisfying the connectivity conditions efficiently given the values.

## Input Format
- The first line contains an integer n, the number of sections in each slide.
- The second line contains n integers representing the water flows of Slide 1.
- The third line contains n integers representing the water flows of Slide 2.

## Output Format
- Return a single integer representing the minimum total cost to make the network fault-tolerant.

## Constraints
- 3 ≤ n ≤ 10^5
- 1 ≤ a[i], b[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, greedy, math
