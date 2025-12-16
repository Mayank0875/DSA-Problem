## Title
Social Media Influence

## Slug
social-media-influence

## Difficulty
Medium

## Description
Influencers have different follower counts. To start a viral trend, a group must have a combined follower count exceeding half the total followers of the entire network.

Your task is to count the number of **collabss**. A collab is considered valid if it satisfies two specific criteria:
1.  **Viral Mass:** The total followers of the collab is strictly greater than half of the total followers across all influencers.
2.  **No Superfluous influencers:** The collab is minimal. This means that removing **any one** influencer from the collab would cause the remaining total to drop to half or less of the total followers (losing the Viral Mass).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total followers is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total followers = 10. Half = 5.
Valid collabss: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of influencers.
- The second line contains n integers: the followers of each influencer.

## Output Format
- Return one integer: the total number of valid collabss.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ followers ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
