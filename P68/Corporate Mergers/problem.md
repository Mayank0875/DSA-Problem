## Title
Corporate Mergers

## Slug
corporate-mergers

## Difficulty
Hard

## Description
A conglomerate owns n subsidiary companies. Joint ventures link some companies. The CEO believes a conglomerate sector is most profitable if it contains a 'Lucky Count' of companies—composed only of 4s and 7s.

The CEO plans to force mergers. Merging k sectors requires signing k - 1 new contracts.

Your task is to determine the minimum number of extra contracts the CEO needs to build to create at least one sector whose size is a Lucky Count. If this goal cannot be achieved, return -1.

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
The optimal way is to connect company 4 with company 3. We can also connect 4 with 1 or 2. This creates a sector of size 4 (a Lucky Count).

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
There is no way to connect the companies to form a sector with a size equal to a Lucky Count.

## Input Format
- The first line contains two integers n and m: the number of companies and the number of existing contracts.
- The next m lines each contain two integers u and v, representing a joint venture between company u and company v. Note that u may be equal to v, and there may be multiple contracts connecting the same pair of companies.

## Output Format
- Return a single integer: the minimum number of contracts to build. If no solution exists, print -1.

## Constraints
- 1 ≤ n ≤ 1e5
- 1 ≤ m ≤ 2e5
- 1 ≤ u, v ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph, dynamic-programming

## Companies
infosys
