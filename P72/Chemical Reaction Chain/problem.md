## Title
Chemical Reaction Chain

## Slug
chemical-reaction-chain

## Difficulty
Hard

## Description
A reaction synthesis starts with Molecule 1 and stabilizes at Molecule n. Intermediate molecular states are connected by reaction pathways.

The reaction must start at the Precursor (labeled 1) and finish at the Product (labeled n). However, to pass through every intermediate state for proper catalysis, the reaction must visit **every single molecule exactly once** during the journey.

You are given the map of the molecules and the directed pathways connecting them. Your task is to calculate the total number of distinct valid paths the reaction can take to complete the synthesis. As the number of paths can be very large, print the answer modulo 1000000007.

## Examples

### 1

#### Input
4 6
1 2
1 3
2 3
3 2
2 4
3 4

#### Output
2

#### Explanation
There are two possible paths that visit every molecule exactly once:
1 -> 2 -> 3 -> 4
1 -> 3 -> 2 -> 4

### 2

#### Input
2 1
1 2

#### Output
1

#### Explanation
The only valid path is 1 -> 2.

## Input Format
- The first line contains two integers n and m: the number of molecules and the number of pathways.
- The molecules are numbered 1, 2, ..., n.
- The next m lines describe the pathways. Each line has two integers a and b, indicating a one-way pathway from molecule a to molecule b.

## Output Format
- Return one integer: the number of possible synthesis paths modulo 10^9+7.

## Constraints
- 1 ≤ n ≤ 20
- 1 ≤ m ≤ n * n
- 1 ≤ a, b ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, dynamic-programming
