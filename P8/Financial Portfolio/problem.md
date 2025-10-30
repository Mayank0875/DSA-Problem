## Title

Financial Portfolio

## Slug

financial-portfolio

## Difficulty

Medium

## Description

An investor has N different assets in their portfolio, with values `A[1], ..., A[N]`. The investor wants to "balance" the portfolio by liquidating exactly one asset and using the funds to buy a new asset. The new asset can have any value between 1 and 10⁹. The "balance factor" of the portfolio is the greatest common divisor (GCD) of all asset values. What is the maximum balance factor the investor can achieve?

## Examples

### 1

#### Input

3 
[7, 6, 8]

#### Output

2

#### Explanation

If the investor sells the asset worth 7 and buys a new one worth 4, the portfolio becomes [4, 6, 8]. The GCD (balance factor) is 2.

### 2

#### Input

2
[100, 100]

#### Output

100

#### Explanation

The investor can sell an asset worth 100 and buy a new one also worth 100.

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