## Title
TV Commercial Slots

## Slug
tv-commercial-slots

## Difficulty
Medium

## Description
An advertiser buys airtime slots. Each slot is defined by a start second and end second within an hour.

Available are list of slots, each defined by a start and an end, represented as a pair `[s, e]`.

Ads cannot overlap. The end time of one ad must be strictly less than the start time of the next to account for transitions. Specifically, to transition from slot `[a, b]` to a subsequent slot `[c, d]`, the e of the first slot must be **strictly less than** the s of the second slot (i.e., `b < c`).

You can select slots in any order you like to form a valid campaign. Your goal is to determine the maximum number of slots that can be included in a single campaign.

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
The longest campaign is `[1, 2] -> [3, 4]`. You cannot include `[2, 3]` because `2` (end of first) is not strictly less than `2` (start of second).

### 2

#### Input
3
1 2
7 8
4 5

#### Output
3

#### Explanation
The slots can be reordered to form the campaign `[1, 2] -> [4, 5] -> [7, 8]`. All transitions satisfy `end < start`.

## Input Format
- The first line contains an integer `n`, the number of available slots.
- The next `n` lines each contain two integers, representing the `s` and `e` of an slot.

## Output Format
- Return a single integer representing the maximum length of the campaign.

## Constraints
- 1 ≤ n ≤ 1000
- -1000 ≤ s < e ≤ 1000

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, dynamic-programming, greedy, sorting
