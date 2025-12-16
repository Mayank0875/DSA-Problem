## Title
Wireless Network

## Slug
wireless-network

## Difficulty
Medium

## Description
Routers have different signal strengths. To jam the area, a set of rogue routers must output more than half the total signal power.

Your task is to count the number of **jamming setss**. A jamming set is considered valid if it satisfies two specific criteria:
1.  **Signal Jam:** The total signal strength of the jamming set is strictly greater than half of the total signal strength across all routers.
2.  **No Superfluous routers:** The jamming set is minimal. This means that removing **any one** router from the jamming set would cause the remaining total to drop to half or less of the total signal strength (losing the Signal Jam).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total signal strength is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total signal strength = 10. Half = 5.
Valid jamming setss: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of routers.
- The second line contains n integers: the signal strength of each router.

## Output Format
- Return one integer: the total number of valid jamming setss.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ signal strength ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
