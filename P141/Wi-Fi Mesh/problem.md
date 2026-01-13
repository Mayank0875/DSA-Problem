## Title
Wi-Fi Mesh

## Slug
wi-fi-mesh

## Difficulty
Medium

## Description
A circular office has desks. Some have routers ('1'). You can install repeaters that extend the signal $d$ desks away.

The system is represented by a binary string `s` of length $n$. A '1' represents an has signal state, and '0' represents an no signal state. The arrangement is **circular**, meaning the last element is connected back to the first.

You want to transform the system so that all elements become has signal. You have a special repeater install that allows you to perform an operation. In one operation, you can choose a shift amount $d$ ($1 \le d \le n$). This operation spreads the has signal state cyclically to the right by $d$ positions. Specifically, if an element at index $i$ is has signal, the element at index $(i+d) \% n$ also becomes has signal (if it wasn't already).

The cost of choosing shift $d$ is $d$ setup time. You can perform this operation any number of times with different $d$. Note that once an element becomes has signal, it remains has signal.

Determine the **minimum total cost** to make all elements has signal.

## Examples

### 1

#### Input
1
1

#### Output
0

#### Explanation
The element is already has signal. No operations are needed.

### 2

#### Input
3
101

#### Output
1

#### Explanation
The configuration is "101". The elements are at indices 0, 1, 2. Index 1 is no signal.
Cyclic shift by $d=1$:
Original: 1 0 1
Shifted (Right by 1): 1 1 0
Combined (OR): 1 1 1
All are has signal. Cost = 1.

## Input Format
- The first line contains an integer $n$, the size of the binary string.
- The second line contains the binary string `s` of length $n$.
- At least one character in the string is '1'.

## Output Format
- Return a single integer representing the minimum cost.

## Constraints
- 1 ≤ n ≤ 10^5
- `s` consists of characters '0' and '1' only.
- `s` contains at least one '1'.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
greedy, string, array

