## Title
Mining Cart Route

## Slug
mining-cart-route

## Difficulty
Hard

## Description
A cart moves ore. Starting at the Deep Vein (1), it must reach the Surface (n). Caverns are connected by rails.

The cart must start at the Deep Vein (labeled 1) and finish at the Surface (labeled n). However, to collect ore samples from every cavern, the cart must visit **every single cavern exactly once** during the journey.

You are given the map of the caverns and the directed rails connecting them. Your task is to calculate the total number of distinct valid paths the cart can take to complete the haul. As the number of paths can be very large, print the answer modulo 1000000007.

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
There are two possible paths that visit every cavern exactly once:
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
- The first line contains two integers n and m: the number of caverns and the number of rails.
- The caverns are numbered 1, 2, ..., n.
- The next m lines describe the rails. Each line has two integers a and b, indicating a one-way rail from cavern a to cavern b.

## Output Format
- Return one integer: the number of possible haul paths modulo 10^9+7.

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
