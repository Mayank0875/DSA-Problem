## Title

Pairing Socks from Laundry

## Slug

pairing-socks-laundry

## Difficulty

Easy

## Description

You're sorting laundry and need to pair up socks. For simplicity, each sock has a 'complexity' value (maybe size or color pattern represented numerically). You can pair two socks together only if their combined complexity doesn't exceed a limit `x`. You can also leave a sock unpaired. Each pair or unpaired sock needs its own 'slot' in the drawer. Given the complexity values of `n` socks, what is the minimum number of drawer slots needed to accommodate all socks, either paired or solo?

## Examples

### 1

#### Input

4 10
[7, 2, 3, 9]

#### Output

3

#### Explanation

One minimal arrangement:
    - Slot 1: Sock with complexity 2 and sock with complexity 7 (Total 9 <= 10)
    - Slot 2: Sock with complexity 3 (Total 3 <= 10)
    - Slot 3: Sock with complexity 9 (Total 9 <= 10)
This requires 3 slots.

### 2

#### Input

5 5
[2, 2, 2, 3, 4]

#### Output

3

#### Explanation

One minimal arrangement:
    - Slot 1: Sock with complexity 2 and sock with complexity 3 (Total 5 <= 5)
    - Slot 2: Two socks with complexity 2 (Total 4 <= 5)
    - Slot 3: Sock with complexity 4 (Total 4 <= 5)
This requires 3 slots.

## Input Format

- The first line contains two integers n and x: the number of socks and the maximum combined complexity per pair.
- The second line contains n integers p_1, p_2, ..., p_n: the complexity value of each sock.

## Output Format

- Return a single integer: the minimum number of drawer slots required.

## Constraints

- 1 ≤ n ≤ 1e5
- 1 ≤ x ≤ 1e9
- 1 ≤ p_i ≤ x

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

greedy, sorting, two pointers