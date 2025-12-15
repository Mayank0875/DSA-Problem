## Title

The Kingdom's Alliance

## Slug

the-kingdoms-alliance

## Difficulty

Medium

## Description

In the grand kingdom of Aethelgard, there are n cities connected by n-1 roads, forming a tree structure. The King wants to strengthen the kingdom's economy by forming trade alliances between neighboring cities. 

An alliance is formed between two cities connected by a road. However, due to bureaucratic constraints, each city can be part of at most one alliance. The King wants to maximize the total number of alliances formed to ensure prosperity across the land.

Your task is to calculate the maximum number of trade alliances (pairs of cities) that can be formed.

## Examples

### 1

#### Input

5
1 2
1 3
3 4
3 5

#### Output

2

#### Explanation

One optimal set of alliances is (1, 2) and (3, 4). City 5 remains independent. This gives a total of 2 alliances.
    
### 2

#### Input

4
1 2
2 3
3 4

#### Output

2

#### Explanation

We can form alliances (1, 2) and (3, 4), giving a total of 2.
  

## Input Format  

- The first line contains an integer n, the number of cities.
- The next n-1 lines each contain two integers u and v, representing a road between city u and city v.

## Output Format  

- Return a single integer representing the maximum number of alliances.
  

## Constraints  

- 1 ≤ n ≤ 2e5
- 1 ≤ a, b ≤ n

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

tree, dynamic-programming, depth-first-search, hackwithinfy

## Companies
infosys