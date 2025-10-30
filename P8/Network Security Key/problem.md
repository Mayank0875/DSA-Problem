## Title

Network Security Key

## Slug

network-security-key

## Difficulty

Medium

## Description

A secure network has N nodes. Each node `i` has a public key `A[i]`. The network's "security factor" is the greatest common divisor (GCD) of all N public keys. You are a security auditor and can update the public key of exactly one node. The new key can be any integer from 1 to 10⁹. What is the maximum possible security factor you can achieve for the network?

## Examples

### 1

#### Input

3 
[7, 6, 8]

#### Output

2

#### Explanation

If you update the key '7' to '4', the keys become [4, 6, 8]. The GCD (security factor) is 2.

### 2

#### Input

2
[100, 100]

#### Output

100

#### Explanation

You can update a key to its current value.

## Input Format

- First line: integer 'n' representing the number of elements written on the blackboard .  
- Second line: 'n' integers representing the elements that are written on blackboard.
- You will be given the array as an input to your function

## Output Format

- Return an integer representing the greatest common divisor after making your move.

## Constraints

- 1 ≤ n ≤ 10^5
- 1 ≤ arr[i] ≤ 10^9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

arrays, prefix sum, suffix sum, math