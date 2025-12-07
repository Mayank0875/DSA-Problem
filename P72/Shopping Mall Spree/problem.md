## Title
Shopping Mall Spree

## Slug
shopping-mall-spree

## Difficulty
Hard

## Description
A shopper moves through a mall. Starting at the Entrance (1), they must reach the Parking Lot (n). Stores are connected by walkways.

The shopper must start at the Entrance (labeled 1) and finish at the Parking Lot (labeled n). However, to visit every store for a sale, the shopper must visit **every single store exactly once** during the journey.

You are given the map of the stores and the directed walkways connecting them. Your task is to calculate the total number of distinct valid paths the shopper can take to complete the spree. As the number of paths can be very large, print the answer modulo 1000000007.

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
There are two possible paths that visit every store exactly once:
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
- The first line contains two integers n and m: the number of stores and the number of walkways.
- The stores are numbered 1, 2, ..., n.
- The next m lines describe the walkways. Each line has two integers a and b, indicating a one-way walkway from store a to store b.

## Output Format
- Return one integer: the number of possible spree paths modulo 10^9+7.

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
