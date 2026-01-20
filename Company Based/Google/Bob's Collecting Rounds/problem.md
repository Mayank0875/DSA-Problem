## Title

Bob's Collecting Rounds

## Slug

bobs-collecting-rounds

## Difficulty

Medium

## Description

Bob has a disorganized collection of $n$ rare items scattered on a shelf. Each item is marked with a unique identification number from $1$ to $n$. Currently, the items are arranged in a random order given by an array.

Bob wants to collect all the items in strictly increasing order of their identification numbers (starting from $1$, then $2$, up to $n$). He uses a specific strategy:
1. He walks along the shelf from left to right.
2. If he sees the next number he needs, he picks it up.
3. If he reaches the end of the shelf and hasn't collected all items, he returns to the start of the shelf and begins a new round (pass).

Your task is to calculate the total number of rounds Bob needs to make to collect all $n$ items.

## Examples

### 1

#### Input

5 
4 2 1 5 3

#### Output

3

#### Explanation

- **Round 1:** Bob walks from left to right. He needs 1. He finds 1. He now needs 2. He passes 5 and 3 (end of shelf).
- **Round 2:** Bob restarts. He sees 4, then finds 2. He now needs 3. He sees 1 (already taken), 5, then finds 3. He now needs 4.
- **Round 3:** Bob restarts. He finds 4 immediately. He now needs 5. He finds 5 later in the shelf.
Total rounds: 3.
    
### 2

#### Input

5
1 2 3 4 5

#### Output

1

#### Explanation

The items are already sorted. Bob collects 1, 2, 3, 4, and 5 in a single pass.
  

## Input Format  

- The first line contains an integer $n$, the number of items.
- The second line contains $n$ distinct space-separated integers, representing the arrangement of items on the shelf.

## Output Format  

- Return a single integer representing the total number of rounds required.
  

## Constraints  

- 1 ≤ n ≤ 1e5

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

greedy, array

## Company
google