## Title
Card Game Deck

## Slug
card-game-deck

## Difficulty
Hard

## Description
A player builds piles from their hand. The 'power suit' of a pile is the suit ID that appears most often in that pile.

Yugi has a collection of $n$ cards, where each card is represented by an integer ID.

To prepare a strategy, Yugi must partition these cards into several non-empty piles. Every card from the original collection must belong to exactly one pile. From each pile, a "power suit" is extracted. The power suit is defined as the **mode** (most frequent element) of the cards in that pile. If a pile has multiple cards tied for the most frequent appearance, any one of them can be chosen as the power suit.

Yugi collects all the extracted power suits to form a final multiset. Your task is to calculate how many distinct final multisets can be created using this process. Two multisets are considered different if the frequency of any ID differs between them.

## Examples

### 1

#### Input
3
1 2 3

#### Output
7

#### Explanation
Any non-empty subset of {1, 2, 3} can be achieved, for a total of 7 multisets.

### 2

#### Input
3
1 2 2

#### Output
4

#### Explanation
We can generate 4 different multisets:
1. Partition into {1, 2, 2} -> power suit is 2 -> Result {2}.
2. Partition into {1, 2}, {2} -> power suits 1, 2 or 2, 2 -> Result {1, 2} or {2, 2}. (Wait, if {1, 2} mode can be 1 or 2. If we pick 2, result is {2, 2}).
3. Partition into {1}, {2, 2} -> power suits 1, 2 -> Result {1, 2}.
4. Partition into {1}, {2}, {2} -> power suits 1, 2, 2 -> Result {1, 2, 2}.
Total distinct multisets: {2}, {2, 2}, {1, 2}, {1, 2, 2}.

## Input Format
- The first line contains an integer $n$, the number of cards.
- The second line contains $n$ space-separated integers representing the card IDs.

## Output Format
- Return a single integer representing the number of different multisets of power suits possible, modulo $998244353$.

## Constraints
- 1 ≤ n ≤ 5000
- 1 ≤ ID ≤ n

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
dynamic-programming, math, combinatorics
