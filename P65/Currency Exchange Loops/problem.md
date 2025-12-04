## Title
Currency Exchange Loops

## Slug
currency-exchange-loops

## Difficulty
Medium

## Description
N currencies can be exchanged in one direction (e.g., USD -> EUR). An Arbitrage Loop is a set of currencies where you can convert from any one to any other.

Two currencies a and b belong to the same Loop if and only if: It is possible to move from a to b, and it is also possible to move from b to a using the network of exchange rates.
In other words, two currencies are in the same Loop if they are mutually reachable.

Your task is to: Determine how many Loops exist in total.

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
The currencies form two distinct groups where round-trip traversal is possible within each group.
Currencies {1, 2, 3} form one Loop.
Path: 1 -> 2 -> 3 -> 1.
Currencies {4, 5} form another Loop.
Path: 4 -> 5 -> 4.
Total Loops: 2.

### 2

#### Input
2 1
1 2

#### Output
2

#### Explanation
There are 2 currencies and 1 one-way exchange.
Exchange: 1 -> 2.
One can go from 1 to 2, but not back. They form separate Loops.

## Input Format
- The first line contains two integers n and m: the number of currencies and exchange rates.
- The following m lines describe the connections. Each line has two integers a and b, indicating a one-way exchange from currency a to currency b.

## Output Format
- Return one integer: the total number of Loops.

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
