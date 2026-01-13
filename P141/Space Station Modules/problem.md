## Title
Space Station Modules

## Slug
space-station-modules

## Difficulty
Medium

## Description
A space station is a ring of modules. Some are pressurized ('1'). Air can be pumped through a hose of length $d$ to pressurize another.

The system is represented by a binary string `s` of length $n$. A '1' represents an pressurized state, and '0' represents an vacuum state. The arrangement is **circular**, meaning the last element is connected back to the first.

You want to transform the system so that all elements become pressurized. You have a special air hose that allows you to perform an operation. In one operation, you can choose a shift amount $d$ ($1 \le d \le n$). This operation spreads the pressurized state cyclically to the right by $d$ positions. Specifically, if an element at index $i$ is pressurized, the element at index $(i+d) \% n$ also becomes pressurized (if it wasn't already).

The cost of choosing shift $d$ is $d$ oxygen units. You can perform this operation any number of times with different $d$. Note that once an element becomes pressurized, it remains pressurized.

Determine the **minimum total cost** to make all elements pressurized.

## Examples

### 1

#### Input
1
1

#### Output
0

#### Explanation
The element is already pressurized. No operations are needed.

### 2

#### Input
3
101

#### Output
1

#### Explanation
The configuration is "101". The elements are at indices 0, 1, 2. Index 1 is vacuum.
Cyclic shift by $d=1$:
Original: 1 0 1
Shifted (Right by 1): 1 1 0
Combined (OR): 1 1 1
All are pressurized. Cost = 1.

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

