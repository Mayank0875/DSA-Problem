## Title
Laser Security System

## Slug
laser-security-system

## Difficulty
Medium

## Description
Mirrors in a circle reflect lasers. Some have beams ('1'). You can align a mirror to split the beam to a target $d$ spots away.

The system is represented by a binary string `s` of length $n$. A '1' represents an beaming state, and '0' represents an dark state. The arrangement is **circular**, meaning the last element is connected back to the first.

You want to transform the system so that all elements become beaming. You have a special alignment that allows you to perform an operation. In one operation, you can choose a shift amount $d$ ($1 \le d \le n$). This operation spreads the beaming state cyclically to the right by $d$ positions. Specifically, if an element at index $i$ is beaming, the element at index $(i+d) \% n$ also becomes beaming (if it wasn't already).

The cost of choosing shift $d$ is $d$ precision. You can perform this operation any number of times with different $d$. Note that once an element becomes beaming, it remains beaming.

Determine the **minimum total cost** to make all elements beaming.

## Examples

### 1

#### Input
1
1

#### Output
0

#### Explanation
The element is already beaming. No operations are needed.

### 2

#### Input
3
101

#### Output
1

#### Explanation
The configuration is "101". The elements are at indices 0, 1, 2. Index 1 is dark.
Cyclic shift by $d=1$:
Original: 1 0 1
Shifted (Right by 1): 1 1 0
Combined (OR): 1 1 1
All are beaming. Cost = 1.

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

