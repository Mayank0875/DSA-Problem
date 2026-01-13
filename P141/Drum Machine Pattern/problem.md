## Title
Drum Machine Pattern

## Slug
drum-machine-pattern

## Difficulty
Medium

## Description
A drum loop has $n$ beats. Some have a kick drum ('1'). You can add an echo effect that repeats the kick $d$ beats later.

The system is represented by a binary string `s` of length $n$. A '1' represents an beat state, and '0' represents an silent state. The arrangement is **circular**, meaning the last element is connected back to the first.

You want to transform the system so that all elements become beat. You have a special echo effect that allows you to perform an operation. In one operation, you can choose a shift amount $d$ ($1 \le d \le n$). This operation spreads the beat state cyclically to the right by $d$ positions. Specifically, if an element at index $i$ is beat, the element at index $(i+d) \% n$ also becomes beat (if it wasn't already).

The cost of choosing shift $d$ is $d$ CPU load. You can perform this operation any number of times with different $d$. Note that once an element becomes beat, it remains beat.

Determine the **minimum total cost** to make all elements beat.

## Examples

### 1

#### Input
1
1

#### Output
0

#### Explanation
The element is already beat. No operations are needed.

### 2

#### Input
3
101

#### Output
1

#### Explanation
The configuration is "101". The elements are at indices 0, 1, 2. Index 1 is silent.
Cyclic shift by $d=1$:
Original: 1 0 1
Shifted (Right by 1): 1 1 0
Combined (OR): 1 1 1
All are beat. Cost = 1.

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

