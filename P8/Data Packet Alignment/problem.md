## Title

Data Packet Alignment

## Slug

data-packet-alignment

## Difficulty

Medium

## Description

A router is processing N data packets. Each packet `i` has a size of `A[i]` bytes. For optimal routing, all packets should ideally be multiples of a common "block size". You can modify the size of exactly one packet, setting its new size to any integer between 1 and 10⁹. Your goal is to find the largest possible "block size" (greatest common divisor) that all N packet sizes can share after your modification.

## Examples

### 1

#### Input

3 
[7, 6, 8]

#### Output

2

#### Explanation

If you modify the size 7 packet to be 4, the packet sizes become [4, 6, 8]. The greatest common divisor is 2, which is the maximum possible block size.

### 2

#### Input

2
[100, 100]

#### Output

100

#### Explanation

You can "modify" a packet to have its original size.

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