## Title
Space Station Modules

## Slug
space-station-modules

## Difficulty
Medium

## Description
Engineers connect `n` modules to `m` docking ports.

However, not every module is compatible with every port due to connector type.
You are given a list of `k` compatible pairs, where a specific module can work with a specific port.

Your task is to determine the maximum number of connections that can be formed simultaneously. Each module and each port can be assigned to at most one connection.

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
There are 3 modules and 2 ports.
Possible valid matching could be:
- module 1 with port 2
- module 2 with port 1
Total = 2.

### 2

#### Input
2 2 1
1 1

#### Output
1

#### Explanation
Only module 1 and port 1 are compatible. The maximum number of operational connections is 1.

## Input Format
- The first line contains three integers `n`, `m`, and `k`: the number of modules, ports, and compatible pairs.
- The modules are numbered `1` to `n` and the ports are numbered `1` to `m`.
- The next `k` lines describe the compatible pairs. Each line contains two integers `a` and `b`, indicating that module `a` and port `b` are compatible.

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
