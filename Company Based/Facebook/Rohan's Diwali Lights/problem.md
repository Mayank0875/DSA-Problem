## Title

Rohan's Diwali Lights

## Slug

rohans-diwali-lights

## Difficulty

Medium

## Description

It is the festival of Diwali, and Rohan is decorating his house with a circular strip of LED lights. The strip has $n$ lights, represented by a binary string $s$ of length $n$. A character '1' means the light is currently ON, and '0' means it is OFF.

Rohan wants all the lights to be ON. The strip is magical and allows him to perform an operation to spread the light. In one operation, he can choose a shift amount $d$ ($1 \le d \le n$). This creates a "shadow" of the current lighting pattern shifted cyclically to the right by $d$ positions. The new state of the strip is the combination of the old state and the shadow (if a light was ON in either the old state or the shadow, it becomes ON).

This operation costs $d$ rupees. Note that lights that are already ON remain ON. Rohan can perform this operation any number of times. Determine the minimum total cost (in rupees) Rohan must spend to turn all the lights ON.

## Examples

### 1

#### Input

1
1

#### Output

0

#### Explanation

The light is already ON. No operations are needed.
    
### 2

#### Input

3
101

#### Output

1

#### Explanation

The strip is "101". The lights are at indices 1, 2, 3 (1-based). Light at 2 is OFF.
Cyclic shift by $d=1$:
Original: 1 0 1
Shifted:  1 1 0 (Right cyclic shift of "101" by 1 is "110")
Combined: 1 1 1 (Bitwise OR)
All lights are ON. Cost = 1.
  

## Input Format  

- The first line contains an integer $n$, the size of the binary string.
- The second line contains the binary string $s$ of length $n$.
- At least one character in the string is '1'.

## Output Format  

- Return a single integer representing the minimum cost to turn all lights ON.
  

## Constraints  

- 1 ≤ n ≤ 1e5
- $s$ consists of characters '0' and '1' only.
- $s$ contains at least one '1'.

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

greedy, string