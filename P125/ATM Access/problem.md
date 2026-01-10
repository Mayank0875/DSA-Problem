## Title
ATM Access

## Slug
atm-access

## Difficulty
Medium

## Description
A bank wants to ensure all shops on a high street are within walking distance of an ATM location.

There are $n$ shops and $m$ ATMs positioned at specific coordinates along a high street.

The bank manager plans to establish a service range. All ATMs will operate with the same walking distance $r$. A ATM at location $x$ with walking distance $r$ covers the interval $[x - r, x + r]$.

For the system to be effective, every shop must be covered by at least one ATM.

Your task is to determine the **minimum non-negative integer walking distance $r$** required to ensure that all $n$ shops are within the range of at least one ATM.

## Examples

### 1

#### Input
3 2
-2 2 4
-3 0

#### Output
4

#### Explanation
shops are at -2, 2, 4. ATMs are at -3, 0.
With walking distance 4:
- ATM at -3 covers [-7, 1]. Covers shop at -2.
- ATM at 0 covers [-4, 4]. Covers shops at -2, 2, 4.
All shops covered. Minimum walking distance is 4.

### 2

#### Input
5 3
1 5 10 14 17
4 11 15

#### Output
3

#### Explanation
With walking distance 3:
- ATM at 4 covers [1, 7]. Covers shops 1, 5.
- ATM at 11 covers [8, 14]. Covers shops 10, 14.
- ATM at 15 covers [12, 18]. Covers shop 17.

## Input Format
- The first line contains two integers $n$ and $m$ — the number of shops and ATMs.
- The second line contains $n$ integers representing the coordinates of the shops. The coordinates are sorted in non-decreasing order.
- The third line contains $m$ integers representing the coordinates of the ATMs. The coordinates are sorted in non-decreasing order.

## Output Format
- Return a single integer — the minimal walking distance $r$ required.

## Constraints
- 1 ≤ n, m ≤ 10^5
- -10^9 ≤ coordinates ≤ 10^9
- The input arrays are sorted in non-decreasing order.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
binary-search, two-pointers, array, math
