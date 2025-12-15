## Title
Cargo Ship Loading

## Slug
cargo-ship-loading

## Difficulty
Hard

## Description
A port master loads containers onto a convoy of `k` ships. There are `n` containers lined up on the dock with specific weights. The containers must be loaded in the order they appear. The 'instability' of a ship is the square of the total weight it carries.

You must partition the sequence of containers into exactly `k` non-empty contiguous shipments.
Each shipment corresponds to a ship.
The "instability" for a ship is calculated as the **square of the sum** of the weights of the containers in that shipment.

Your goal is to minimize the total instability (the sum of the instability values of all `k` shipments).

## Examples

### 1

#### Input
8 3
2 3 1 2 2 3 4 1

#### Output
110

#### Explanation
We partition the containers into 3 shipments: `[2, 3, 1]`, `[2, 2, 3]`, and `[4, 1]`.
The sums are 6, 7, 5.
The total instability is $6^2 + 7^2 + 5^2 = 36 + 49 + 25 = 110$.

### 2

#### Input
5 1
1 2 3 4 5

#### Output
225

#### Explanation
Only 1 shipment is allowed, containing all containers. Sum = 15. instability = $15^2 = 225$.

## Input Format
- The first line contains two integers `n` and `k`: the number of containers and the required number of shipments.
- The second line contains `n` integers representing the weights of each container.

## Output Format
- Return one integer: the minimum total instability.

## Constraints
- 1 ≤ k ≤ n ≤ 3000
- 1 ≤ value ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, array
