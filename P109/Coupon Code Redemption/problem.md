## Title
Coupon Code Redemption

## Slug
coupon-code-redemption

## Difficulty
Easy

## Description
A marketing system processes used coupons. Duplicate coupon codes in the 'used' list indicate a redemption exploit.

Your task is to determine if any coupon code appears at least twice in the list.

## Examples

### 1

#### Input
4
1 2 3 1

#### Output
Yes

#### Explanation
The coupon code `1` appears twice.

### 2

#### Input
4
1 2 3 4

#### Output
No

#### Explanation
All coupon codes are distinct.

## Input Format
- The first line contains a single integer n, the number of redemptions.
- The second line contains n space-separated integers, representing the coupon codes.

## Output Format
- Return `Yes` if any coupon code appears at least twice, otherwise `No`.

## Constraints
- 1 ≤ n ≤ 10^5
- -10^9 ≤ values ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
sorting, array, hash-table
