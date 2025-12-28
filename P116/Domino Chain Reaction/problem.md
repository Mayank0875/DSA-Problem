## Title
Domino Chain Reaction

## Slug
domino-chain-reaction

## Difficulty
Medium

## Description
You are setting up a trick with special dominoes. Each domino covers a range on the floor when it falls.

You possess a list of dominoes, each defined by a start point and an fall limit, represented as a pair `[start, limit]`.

To ensure a sequential trigger without jamming, the fall limit of the previous domino must be strictly less than the start point of the next. Specifically, to transition from domino `[a, b]` to a subsequent domino `[c, d]`, the limit of the first domino must be **strictly less than** the start of the second domino (i.e., `b < c`).

You can select dominoes in any order you like to form a valid chain reaction. Your goal is to determine the maximum number of dominoes that can be included in a single chain reaction.

## Examples

### 1

#### Input
3
1 2
2 3
3 4

#### Output
2

#### Explanation
The longest chain reaction is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The dominoes can be reordered to form the chain reaction `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available dominoes.
- The next `n` lines each contain two integers, representing the `start` and `limit` of an domino.

## Output Format
- Return a single integer representing the maximum length of the chain reaction.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ start < limit ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
