## Title
Cargo Ship Balance

## Slug
cargo-ship-balance

## Difficulty
Medium

## Description
A cargo ship carries containers of different weights. To tilt the ship to the starboard side, the weight on that side must exceed half the total cargo weight.

Your task is to count the number of **cargo setss**. A cargo set is considered valid if it satisfies two specific criteria:
1.  **Listing Force:** The total weight of the cargo set is strictly greater than half of the total weight across all containers.
2.  **No Superfluous containers:** The cargo set is minimal. This means that removing **any one** container from the cargo set would cause the remaining total to drop to half or less of the total weight (losing the Listing Force).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total weight is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total weight = 10. Half = 5.
Valid cargo setss: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of containers.
- The second line contains n integers: the weight of each container.

## Output Format
- Return one integer: the total number of valid cargo setss.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ weight ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
