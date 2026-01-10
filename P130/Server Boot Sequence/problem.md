## Title
Server Boot Sequence

## Slug
server-boot-sequence

## Difficulty
Medium

## Description
A cluster of servers is booting up. Servers are indexed 1 to n. The system is considered 'stable' if servers 1 through k are all online without gaps.

There is a sequence of $n$ servers indexed from $1$ to $n$. Initially, all servers are **offline**.

You boot up the servers one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you boot up the server at the position `sequence[i-1]`.

A state is called **stable** if, after performing $k$ steps, exactly the first $k$ servers (indices $1$ to $k$) are online and all other servers are offline.

Your task is to calculate how many times the system becomes **stable** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "00100" (Not stable)
- Step 2 (index 2): "01100" (Not stable)
- Step 3 (index 4): "01110" (Not stable)
- Step 4 (index 1): "11110" (stable: first 4 are online)
- Step 5 (index 5): "11111" (stable: first 5 are online)
Total stable states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "0001" (Not stable)
- Step 2 (index 1): "1001" (Not stable)
- Step 3 (index 2): "1101" (Not stable)
- Step 4 (index 3): "1111" (stable)
Total stable states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was stable.

## Constraints
- 1 ≤ n ≤ 10^4
- `sequence` is a permutation of numbers from $1$ to $n$.

## Time Limit
2 second

## Memory Limit
256 MB

## Tags
array, greedy

## Company
google
