## Title
Bank Wire Transfers

## Slug
bank-wire-transfers

## Difficulty
Medium

## Description
Banks allow wire transfers to specific partners. A Banking Bloc is a group of banks that can circulate funds among themselves.

Two banks a and b belong to the same Banking Bloc if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of channels.
In other words, two banks are in the same Banking Bloc if they are mutually reachable.

Your task is to: Determine how many Banking Blocs exist in total.

## Examples

### 1

#### Input
5 6
1 2
2 3
3 1
3 4
4 5
5 4

#### Output
2

#### Explanation
The banks form two distinct groups where round-trip traversal is possible within each group.
Banks {1, 2, 3} form one Banking Bloc.
Path: 1 -> 2 -> 3 -> 1.
Banks {4, 5} form another Banking Bloc.
Path: 4 -> 5 -> 4.
Total Banking Blocs: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 banks and 1 one-way channel.
Channel: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Banking Blocs.

## Input Format
- The first line contains two integers n and m: the number of banks and channels.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way channel from bank a to bank b.

## Output Format
- Return one integer: the total number of Banking Blocs.

## Constraints
- 1 ≤ n ≤ 1e5
- 1 ≤ m ≤ 2e5
- 1 ≤ a, b ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, depth-first-search
