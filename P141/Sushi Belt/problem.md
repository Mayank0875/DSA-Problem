## Title
Sushi Belt

## Slug
sushi-belt

## Difficulty
Medium

## Description
A sushi conveyor belt has plates. Some have sushi ('1'). The chef can place a new plate $d$ spots ahead of an existing one.

The system is represented by a binary string `s` of length $n$. A '1' represents an sushi state, and '0' represents an empty state. The arrangement is **circular**, meaning the last element is connected back to the first.

You want to transform the system so that all elements become sushi. You have a special placement that allows you to perform an operation. In one operation, you can choose a shift amount $d$ ($1 \le d \le n$). This operation spreads the sushi state cyclically to the right by $d$ positions. Specifically, if an element at index $i$ is sushi, the element at index $(i+d) \% n$ also becomes sushi (if it wasn't already).

The cost of choosing shift $d$ is $d$ effort. You can perform this operation any number of times with different $d$. Note that once an element becomes sushi, it remains sushi.

Determine the **minimum total cost** to make all elements sushi.

## Examples

### 1

#### Input
1
1

#### Output
0

#### Explanation
The element is already sushi. No operations are needed.

### 2

#### Input
3
101

#### Output
1

#### Explanation
The configuration is "101". The elements are at indices 0, 1, 2. Index 1 is empty.
Cyclic shift by $d=1$:
Original: 1 0 1
Shifted (Right by 1): 1 1 0
Combined (OR): 1 1 1
All are sushi. Cost = 1.

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

