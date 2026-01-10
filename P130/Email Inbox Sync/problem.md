## Title
Email Inbox Sync

## Slug
email-inbox-sync

## Difficulty
Medium

## Description
Emails are downloaded. The inbox is 'up-to-date' for the week if emails 1 to k are all present.

There is a sequence of $n$ emails indexed from $1$ to $n$. Initially, all emails are **missing**.

You sync the emails one by one in a specific order given by an array `sequence`. In the $i$-th step (1-indexed), you sync the email at the position `sequence[i-1]`.

A state is called **up-to-date** if, after performing $k$ steps, exactly the first $k$ emails (indices $1$ to $k$) are downloaded and all other emails are missing.

Your task is to calculate how many times the system becomes **up-to-date** during the entire process.

## Examples

### 1

#### Input
5
3 2 4 1 5

#### Output
2

#### Explanation
- Step 1 (index 3): "xxexx" (Not up-to-date)
- Step 2 (index 2): "xeexx" (Not up-to-date)
- Step 3 (index 4): "xeeex" (Not up-to-date)
- Step 4 (index 1): "eeeex" (up-to-date: first 4 are downloaded)
- Step 5 (index 5): "eeeee" (up-to-date: first 5 are downloaded)
Total up-to-date states: 2.

### 2

#### Input
4
4 1 2 3

#### Output
1

#### Explanation
- Step 1 (index 4): "xxxe" (Not up-to-date)
- Step 2 (index 1): "exxe" (Not up-to-date)
- Step 3 (index 2): "eexe" (Not up-to-date)
- Step 4 (index 3): "eeee" (up-to-date)
Total up-to-date states: 1.

## Input Format
- The first line contains an integer $n$.
- The second line contains $n$ space-separated integers representing the array `sequence`.

## Output Format
- Return a single integer representing the number of times the state was up-to-date.

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
