## Title
Computer Peripheral Connect

## Slug
computer-peripheral-connect

## Difficulty
Medium

## Description
An office has `n` computers and `m` printers. IT needs to map them.

However, not every computer is compatible with every printer due to network access rights.
You are given a list of `k` compatible pairs, where a specific computer can work with a specific printer.

Your task is to determine the maximum number of connections that can be formed simultaneously. Each computer and each printer can be assigned to at most one connection.

## Examples

### 1

#### Input
3 2 4
1 1
1 2
2 1
3 1

#### Output
2

#### Explanation
There are 3 computers and 2 printers.
Possible valid matching could be:
- computer 1 with printer 2
- computer 2 with printer 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only computer 1 and printer 1 are compatible. The maximum number of operational connections is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of computers, printers, and compatible pairs.
- The computers are numbered `1` to `n` and the printers are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that computer `a` and printer `b` are compatible.

## Output Format
- Return one integer: the maximum number of pairs that can be formed.

## Constraints
- 1 ≤ n, m ≤ 500
- 1 ≤ k ≤ 1000
- 1 ≤ a ≤ n
- 1 ≤ b ≤ m

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
graph
