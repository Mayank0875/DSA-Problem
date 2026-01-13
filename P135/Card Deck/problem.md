## Title
Card Deck

## Slug
card-deck

## Difficulty
Medium

## Description
A dealer deals cards into hands.

The dealer has prepared $n$ cards arranged in a sequence. The $i$-th card has a value of $a_i$.

These cards need to be grouped into hands. Every hand must hold the exact same number of cards, denoted by $k$. The grouping happens sequentially:
- The first $k$ cards go into the first hand.
- The second $k$ cards go into the second hand.
- ...
- The last $k$ cards go into the $(n/k)$-th hand.

Since every hand must have exactly $k$ cards, this grouping is only possible if $n$ is divisible by $k$ ($1 \le k \le n$).

The dealer wants to choose a valid $k$ such that the **difference between the maximum total value and the minimum total value** of the hands is maximized. If there is only one hand (i.e., $k=n$), the difference is 0.

Your task is to calculate this maximum possible difference over all valid choices of $k$.

## Examples

### 1

#### Input
2
1 2

#### Output
1

#### Explanation
Possible values for $k$ are divisors of 2: 1, 2.
- $k=1$: hand 1 has sum 1, hand 2 has sum 2. Difference = $|2-1| = 1$.
- $k=2$: Only one hand with sum $1+2=3$. Difference = 0.
Max difference is 1.

### 2

#### Input
4
10 10 10 10

#### Output
0

#### Explanation
All cards are equal. Regardless of $k$, all hands will have the same sum. Difference is always 0.

## Input Format
- The first line contains one integer $n$ — the number of cards.
- The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ — the values of the cards.

## Output Format
- Return a single integer — the maximum absolute difference.

## Constraints
- 1 ≤ n ≤ 1.5 * 10^5
- 1 ≤ a[i] ≤ 10^9

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, math, number-theory


