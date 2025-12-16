## Title
Server Quorum

## Slug
server-quorum

## Difficulty
Medium

## Description
A distributed database runs on n servers, each with a different voting weight based on its uptime. To commit a transaction, a quorum (strict majority of total weight) is required.

Your task is to count the number of **quorumss**. A quorum is considered valid if it satisfies two specific criteria:
1.  **Consensus:** The total voting weight of the quorum is strictly greater than half of the total voting weight across all servers.
2.  **No Superfluous servers:** The quorum is minimal. This means that removing **any one** server from the quorum would cause the remaining total to drop to half or less of the total voting weight (losing the Consensus).

## Examples

### 1

#### Input
5
3 1 4 1 5

#### Output
4

#### Explanation
Total voting weight is 14. Half is 7. We need a sum > 7.
The group {5, 4, 1} (Sum 10) is **not** valid because removing 1 leaves 9, which is still > 7.
Valid groups are those where every member is critical.

### 2

#### Input
4
1 2 3 4

#### Output
3

#### Explanation
Total voting weight = 10. Half = 5.
Valid quorumss: {4, 2}, {4, 3}, {3, 2, 1}.

## Input Format
- The first line contains an integer n: the number of servers.
- The second line contains n integers: the voting weight of each server.

## Output Format
- Return one integer: the total number of valid quorumss.

## Constraints
- 1 ≤ n ≤ 60
- 1 ≤ voting weight ≤ 10^5

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
maths, dynamic-programming
