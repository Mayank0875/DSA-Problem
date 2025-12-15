## Title

The Prophetic Alliance

## Slug

the-prophetic-alliance

## Difficulty

Hard

## Description

In the mystical archipelago of Numeria, King Petya dreams of uniting his fractured kingdom. The world is made up of n islands, and some of them are connected by two-way bridges. At the moment, the islands form several disconnected regions (connected components).

The people of Numeria are deeply superstitious and believe in “Prophetic Numbers” — positive integers that contain only the digits 4 and 7 in their decimal form (for example: 4, 7, 47, 744). King Petya wants to build his new palace in a region whose total number of islands is exactly one of these Prophetic Numbers.

But the current regions may not have sizes that match these holy numbers. King Petya is allowed to build new bridges between different regions, merging them into larger ones. Merging k regions into a single region requires building k − 1 new bridges.

Your task is to determine the minimum number of extra bridges Petya needs to build to create at least one region whose size is a Prophetic Number. If this goal cannot be achieved, return -1.

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

The optimal way is to connect 4 with 3. we can also connect 4 with 1, 2 also.
    
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

There is no ways to connect.
  

## Input Format  

- The first line contains two integers n and m: the number of islands and the number of existing bridges.
- The next m lines each contain two integers u and v, representing a bridge between island u and island v. Note that u may be equal to v, and there may be multiple bridges connecting the same pair of islands.

## Output Format  

- Return a single integer: the minimum number of bridges to build. If no solution exists, print -1.
  

## Constraints  

- 1 ≤ n ≤ 1e5
- 1 ≤ m ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit

2 second

## Memory Limit

256 MB

## Tags
graph, dynamic-programming, hackwithinfy

## Companies
infosys