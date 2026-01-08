## Title
Cargo Loading

## Slug
cargo-loading

## Difficulty
Hard

## Description
A crane loads containers. It lifts a standard box (1 unit) or a heavy double box (2 units).

The operator starts at slot 0 and wishes to reach slot $n$. On each move, The operator can load forward either **1 slot** or **2 slots**.

Your task is to calculate the total number of distinct ways to reach exactly slot $n$. Since the distance $n$ can be extremely large, return the answer modulo $10^9 + 7$.

## Examples

### 1

#### Input
2

#### Output
2

#### Explanation
There are two ways to reach slot 2:
1. 1 slot + 1 slot
2. 2 slots

### 2

#### Input
3

#### Output
3

#### Explanation
There are three ways:
1. 1 + 1 + 1
2. 1 + 2
3. 2 + 1

## Input Format
- The only input line has an integer $n$ — the target slot.

## Output Format
- Return a single integer: the number of ways modulo $10^9 + 7$.

## Constraints
- 1 ≤ n ≤ 10^18

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math

