## Title

The Twin Artifacts

## Slug

the-twin-artifacts

## Difficulty

Easy

## Description

A museum is organizing a "Twin Artifacts" exhibition. For the display to be aesthetically pleasing, every type of artifact in the collection must appear exactly twice.
You are given an array of integers representing the artifact IDs currently in the collection. You can perform two types of operations:
1. **Acquire**: Add a new artifact of an existing ID (cost: 1).
2. **Discard**: Remove an existing artifact from the collection (cost: 1).

Your task is to determine the minimum number of operations required so that every artifact ID present in the final collection has a frequency of exactly 2.

## Examples

### 1

#### Input

5
1 1 1 2 3

#### Output

3

#### Explanation

- ID 1: Count is 3. Remove one to make count 2 (Cost 1).
- ID 2: Count is 1. Add one to make count 2 (Cost 1).
- ID 3: Count is 1. Add one to make count 2 (Cost 1).
Total cost: 1 + 1 + 1 = 3.
    
### 2

#### Input

4
10 10 20 20

#### Output

0

#### Explanation

Both ID 10 and ID 20 already appear exactly twice. No operations are needed.

## Input Format  

- The first line contains an integer $n$ ($1 \le n \le 10^5$), the number of artifacts.
- The second line contains $n$ space-separated integers $a_i$ ($1 \le a_i \le 10^9$), representing the artifact IDs.

## Output Format  

- Return a single integer representing the minimum operations required.
  

## Constraints  

- 1 ≤ n ≤ 1e5
- 1 ≤ a_i ≤ 1e9

## Time Limit

2 second

## Memory Limit

256 MB

## Tags

greedy, array

## Company
facebook