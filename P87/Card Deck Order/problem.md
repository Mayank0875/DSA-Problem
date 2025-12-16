## Title
Card Deck Order

## Slug
card-deck-order

## Difficulty
Medium

## Description
A magician wants to perform a trick. The Red cards (0) must come before the Black cards (1) in the deck.

We can represent the arrangement as a binary string `deck` of length `n`, consisting of '0's (Red cards) and '1's (Black cards). A string is considered **sorted** if all '0's appear before all '1's.

You possess a specific technique to organize them. In one operation, you can:
1. Choose any substring of `deck`.
2. Choose a positive integer `k`.
3. Cyclically shift the chosen substring to the left by `k` positions.

For example, shifting the substring `1011` of string `0101100` by 2 positions results in `0111000`.

Your task is to calculate the **minimum number of operations** required to make the string `deck` sorted (i.e., all Red cardss precede all Black cardss).

## Examples

### 1

#### Input
01010101

#### Output
3

#### Explanation
We need to move the Red cardss (0) that appear after Black cardss (1).
There are three distinct groups of '0's appearing after the first '1'.
1. The '0' at index 2.
2. The '0' at index 4.
3. The '0' at index 6.
Each group requires one operation to effectively move to the correct side.

### 2

#### Input
11001010001

#### Output
3

#### Explanation
There are three distinct groups of '0's (Red cards) that appear after the first '1' (Black cards):
1. The group `00` at indices 2-3.
2. The group `0` at index 5.
3. The group `000` at indices 7-9.
Each group requires one operation.

## Input Format
- The first line contains a single string `deck` consisting only of characters '0' and '1'.

## Output Format
- Return a single integer representing the minimum number of operations required.

## Constraints
- 1 ≤ deck.length ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
string, greedy
